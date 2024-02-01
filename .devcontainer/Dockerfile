FROM mcr.microsoft.com/devcontainers/base:ubuntu

ARG USERNAME=vscode
ARG USER_UID=1000
ARG USER_GID=${USER_UID}

ENV HOME=/home/${USERNAME}

# Apt
RUN apt-get update
RUN apt-get install -y wget \
    xz-utils \
    git \
    curl \
    file \
    unzip \
    zip \
    openjdk-17-jdk-headless --no-install-recommends \
    ninja-build \
    clang \
    cmake \
    pkg-config

RUN apt-get autoremove -y \
    && apt-get clean -y \
    && rm -rf /var/lib/apt/lists/*

# RUN groupadd --gid ${USER_GID} ${USERNAME}
#    && useradd -s /bin/bash --uid ${USER_UID} --gid ${USER_GID} -m ${USERNAME}
RUN echo ${USERNAME} ALL=\(root\) NOPASSWD:ALL > /etc/sudoers.d/${USERNAME} \
    && chmod 0440 /etc/sudoers.d/${USERNAME} \
    && su ${USERNAME} \
    && cd $HOME

# Android SDK
# Parameters
ENV ANDROID_SDK_TOOLS_VERSION=11076708
ENV ANDROID_PLATFORM_VERSION=33
ENV ANDROID_BUILD_TOOLS_VERSION=33.0.0
ENV ANDROID_HOME=${HOME}/android-sdk-linux
ENV ANDROID_SDK_ROOT="$ANDROID_HOME"
ENV PATH=${PATH}:${ANDROID_HOME}/cmdline-tools/cmdline-tools/bin:${ANDROID_HOME}/platform-tools:${ANDROID_HOME}/emulator

# Commands
RUN curl -C - --output android-sdk-tools.zip https://dl.google.com/android/repository/commandlinetools-linux-${ANDROID_SDK_TOOLS_VERSION}_latest.zip \
&& mkdir -p ${ANDROID_HOME}/ \
&& unzip -q android-sdk-tools.zip -d ${ANDROID_HOME}/cmdline-tools/ \
&& rm android-sdk-tools.zip 
RUN yes | sdkmanager --licenses \
&& mkdir ${HOME}/.android \
&& touch $HOME/.android/repositories.cfg \
&& sdkmanager platform-tools \
&& sdkmanager emulator \
&& sdkmanager "platforms;android-${ANDROID_PLATFORM_VERSION}" "build-tools;$ANDROID_BUILD_TOOLS_VERSION" \
&& sdkmanager --install "cmdline-tools;latest"
# create emulator android	
RUN sdkmanager "system-images;android-${ANDROID_PLATFORM_VERSION};google_apis;x86_64"
# RUN avdmanager create avd -n Android${ANDROID_PLATFORM_VERSION} -k "system-images;android-${ANDROID_PLATFORM_VERSION};google_apis;x86_64"

# Flutter
RUN git clone -b master https://github.com/flutter/flutter.git /sdk/flutter
RUN ./sdk/flutter/bin/flutter --version
ENV PATH="/sdk/flutter/bin:${PATH}"
RUN chmod -R 777 /sdk/flutter
RUN chown -R ${USERNAME} ${HOME}