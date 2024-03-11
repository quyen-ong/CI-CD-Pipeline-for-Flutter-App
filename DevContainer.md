## DevContainer Environment
A DevContainer is a containerized development environment. It uses Docker containers to create a fully equipped development workspace with all the necessary tools, libraries, and runtimes pre-installed. This ensures consistency regardless of the developer's local machine setup, fixing the "it works on my computer" problem. DevContainers are especially useful for Flutter application development eliminates dependency issues. The DevContainer ensures that exact version and all the tools needed are available.

# Configuration
To create the DevContainer:
  1. Download VS Code
  2. Create a Docker Account
  3. Download Docker
  4. Log into Docker on the app
  5. Open VS Code
  6. Click on the blue rectangle with 2 arrows on the bottom left corner
  7. Click on 'New Dev Container...'
  8. Search for and choose 'Ubuntu'
  9. Click on 'Additional Options...'
  10. Click on 'jammy'
  11. Search for and check 'Flutter'
  12. Click on 'OK'
  13. Click on 'Trust @jarrodcolburn'

# Integration with VS Code
VS Code provided a user-friendly interface to configure the DevContainer for Flutter application development. VS Code allowed for easy selection of the Flutter SDK.

# Usage
To utilize this container image:
  1. create a Docker account and download Docker onto your desktop
  2. download VsCode
  3. download the Docker extension and the Dev Containers extension in VsCode
  4. open a folder in VsCode
  5. got to source control
  6. go to the '...' in the same bar as the text 'source control'
  7. click clone and enter the link for this repo to clone (https://github.com/quyen-ong/CSC-325.git)

# Challenges and Solutions
There was an issue with permissions. However, after running 'flutter pub upgrade', the problem was resolved.

# Conclusion
The DevContainer ensures that all the tools, libraries, and runtimes the project needs is there. This allows me to work on the project no matter what computer I have as long as I can use VS Code and access the git. Before this class, I didn't know Docker existed, so everything so far has been quite insightful. This includes learning about DevContainers, learning how to use GitHub, and using VS Code to create a Flutter App.