This repository contains the necessary files to set up a containerized development environment that supports Flutter web applications.

# General Information
Docker
- platform to build, deploy, run, update, and manage containers

Containers
- executable software that has all the code, libraries, and dependencies to let you run the app anywhere
- resolves "it works on my computer"
- you can mess around in a container however you want and it won't mess up your computer
- Docker is the operating system for containers

Development container (dev container)
- a container you develop and run code in
 
Docker Image
- snapshot/blueprint of libraries and dependencies a container needs to run


# Instructions
To utilize this container image:
  1. create a Docker account and download Docker onto your desktop
  2. download VsCode
  3. download the Docker extension and the Dev Containers extension in VsCode
  4. open a folder in VsCode
  5. got to source control
  6. go to the '...' in the same bar as the text 'source control'
  7. click clone and enter the link for this repo to clone (https://github.com/quyen-ong/CSC-325.git)

To run the app:
  1. cd into the folder containing the app
  2. run 'flutter run -d web-server'

Troubleshoot:
- if there are permission errors run 'flutter pub upgrade'
