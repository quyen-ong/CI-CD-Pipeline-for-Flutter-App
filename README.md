This repository contains the necessary files to set up a containerized development environment that supports Flutter web applications.

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
