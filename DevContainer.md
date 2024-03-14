# DevContainer Environment
A DevContainer is a containerized development environment. It uses Docker containers to create a fully equipped development workspace with all the necessary tools, libraries, and runtimes pre-installed. This ensures consistency regardless of the developer's local machine setup, fixing the "it works on my computer" problem. DevContainers are especially useful for Flutter application development eliminates dependency issues. The DevContainer ensures that exact version and all the tools needed are available.

## Configuration
### To create the DevContainer:
  1. Create a [Docker](https://www.docker.com/) Account
      - This step needs to be done through the website to log in on the app
  2. Download Docker and log into Docker on the app
      - Keep Docker open because we will need it running to create a DevContainer
  3. Download and open [VS Code](https://code.visualstudio.com/download)
      - This will be the code editor we will use
  4. Click on the blue rectangle with 2 arrows on the bottom left corner to get to the option that will allow us to create a new DevContainer
  5. Click on `New Dev Container...`
  6. Search for and choose `Ubuntu` as the configuration template
      - Any of the other templates would work as well. We are using Ubuntu because it is the mode widely used Linux workstation platform.
  7. Click on `Additional Options...` > `jammy` to get to the features.
  8. Search for and check `Flutter` so that we won't need to manually setup Flutter into our DevContainer.
  9. Click on `OK` > `Trust @jarrodcolburn` to create the DevContainer.

## Integration with VS Code
VS Code provided a user-friendly interface to configure the DevContainer for Flutter application development. VS Code allowed for easy selection of the Flutter SDK.

## Usage
The DevContainer ensures that everyone working on this project has the same version of Flutter running on the same system. So, if there is a problem, then everyone working on the project will have the same problem and can work together to come up with a solution that can be used for everyone. Having the same version of Flutter allows everyone to have access to the same set of features that will have the same functions.
### To utilize this container image:
  1. create a [Docker](https://www.docker.com/) account and download Docker onto your desktop
  2. download [VS Code](https://code.visualstudio.com/download)
  3. download the Docker extension and the Dev Containers extension in VS Code
  4. open a folder in VS Code
  5. got to source control
  6. go to the `...` in the same bar as the text `source control`
  7. click clone and enter the link for this repo to clone: <https://github.com/quyen-ong/CSC-325.git>

### Flutter Development:
- `flutter --version `: shows current version of Flutter SDK
- `flutter run -d web-server`: runs the flutter app in a website
- `flutter --help --verbose`: view all commands that Flutter supports
- `flutter create appName`: create an app named 'appName'

## Challenges and Solutions
There was an issue with permissions after closing and reopening the DevContainer. To solve this issue: cd into the app folder and run `flutter pub upgrade`. The flutter command will solve the dependency issues causing the permissions error. You should not have to run `flutter pub upgrade` more than once.

## Conclusion
The DevContainer ensures that all the tools, libraries, and runtimes the project needs is there. This allows me to work on the project no matter what computer I have as long as I can use VS Code and access the git. Before this class, I didn't know Docker existed, so everything so far has been quite insightful. This includes learning about DevContainers, learning how to use GitHub, and using VS Code to create a Flutter App.