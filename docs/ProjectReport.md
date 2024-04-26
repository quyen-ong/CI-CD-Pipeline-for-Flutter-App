# Continuous Integration and Continuous Deployment (CI/CD) Pipeline for Flutter Web Application

## Introduction

In modern software development, CI/CD pipelines play a crucial role in automating the build, test, and deployment processes. They ensure efficiency, reliability, and consistency in software delivery. CI/CD pipelines enable rapid iteration, integration of new features, and continuous improvement of applications.

## DevContainer Environment

The Flutter development environment is configured using Docker containers, providing a consistent and reproducible setup for development across different systems. This Docker-based environment includes the necessary dependencies and tools for Flutter development, ensuring that all team members have an identical development environment.

For more information read [DevContainer.md](https://github.com/quyen-ong/CI-CD-Pipeline-for-Flutter-App/blob/main/docs/DevContainer.md)

## Source Code Version Control Tools

The project utilizes GitHub for version control, enabling effective management of source code. The source code is organized into branches (e.g., main, feature branches) to facilitate collaborative development. Pull requests (PRs) are used to review and merge changes into the main branch, triggering automated tests and deployments through the CI/CD pipeline.

For more information read [VersionControl.md](https://github.com/quyen-ong/CI-CD-Pipeline-for-Flutter-App/blob/main/docs/VersionControl.md)

## CI/CD Pipeline Environment

The CI/CD pipeline is set up using GitHub Actions hosted on GitHub's cloud infrastructure. GitHub Actions are used for testing and deploying the Flutter application to GitHub Pages. The pipeline is triggered automatically on each push to the main branch and pull requests. The GitHub cloud environment provides scalability and reliability, although subject to certain usage limits such as concurrent job limitations and storage constraints.

For more information read [Pipeline.md](https://github.com/quyen-ong/CI-CD-Pipeline-for-Flutter-App/blob/main/docs/Pipeline.md)

## CI/CD Tools

GitHub Actions is selected as the primary CI/CD tool for this project. Key configurations include utilizing the `actions/checkout@v4` action for code checkout and `peaceiris/actions-gh-pages@v3` for deploying to GitHub Pages. These tools automate the build, test, and deployment processes. Configuration files (`yaml` files) are used to define workflows, specifying the sequence of steps to be executed during the CI/CD process.

## Deployment Environment

The Flutter application is deployed to GitHub Pages, providing a convenient way to showcase and share the application online. The deployment process involves building the Flutter web application and publishing the output to a designated branch (`gh-pages`) within the GitHub repository. Although automatic deployment upon code push is not functional due to configuration issues, the deployment action can be manually triggered to update the hosted site.

## Flutter Web Application

The Flutter web application is a drag and drop card game from [Flutter's game template](https://github.com/flutter/games/tree/main/templates/card). It is a game where you drag and drop cards into two circles. The application is thoroughly tested as part of the CI/CD pipeline to ensure quality and reliability. Testing includes unit tests, integration tests, and possibly end-to-end tests using frameworks like Flutter Driver or other tools.

## Conclusion

This project has demonstrated the importance of CI/CD pipelines in modern development practices, enabling faster feedback cycles and streamlined deployment processes. Lessons learned include the value of automated testing, the importance of robust deployment configurations, and the benefits of Docker-based development environments for consistency. Challenges encountered such as deployment automation issues highlight areas for improvement. Future enhancements to the pipeline and application can include further automation (e.g., automatic deployment triggers), enhanced testing strategies, and optimizations to improve build and deployment times.
