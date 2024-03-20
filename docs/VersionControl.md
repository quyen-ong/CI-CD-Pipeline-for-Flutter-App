# Source Code Version Control Tools
Version control is crucial in software development as it allows changes to be tracked, preserve previous code, and facillitate collaboration. Version control also helps maintain integrity by controlling permissions and access so that only authorized individuals can make modifications to the code. Since all changes are tracked, previous versions of code can be retrieved if the new code is causing issues. 

## Version Control System Used
For this project, [GitHub](https://github.com/) is used. One of the reasons GitHub was chosen is because it has a large community, making it easy to access support if needed and collaborate with others. About 100 million developers over the world use GitHub. Also, GitHub has many powerful tools, such as GitHub actions which is a continuous integration and continuous delivery (CI/CD) platform that allows you to automate your build, test, and deployment pipeline. 

## Respository Setup
The directory layout is organized as follows:

- `/.devcontainer`: Contains the recommended development environment configuration files. This ensures that all team members use a consistent environment, which reduces the "it works on my machine" problem.

- `/docs`: This directory hosts all project documentation, ensuring that design documents, setup instructions, and other important information are easily accessible and well-organized.

- `/app`: Houses the Flutter application source code. This separation ensures that the application code remains isolated from documentation and other non-app-related files, facilitating a clearer workflow and easier navigation.

- `/.github/workflows`: Contains the automated GitHub Actions definition files. These files define our continuous integration and delivery pipeline, automating tests, builds, and deployments based on predefined events and conditions.

- `/games`: Contains a few sample games from Flutter sourced from: https://github.com/flutter/games

This structured approach enhances the project’s navigability and scalability, aligning with Flutter's best practices and supporting our agile development methodologies.

## Common Commands and Usage
These are some commonly used commands in this project.

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |
| `git commit -m "[commit message]"` | Commit changes |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

## Collaboration Features
GitHub facilitates collaboration among team members through various features that streamline communication, code review, and conflict resolution:

1. **Pull Requests (PRs):** Pull requests are a fundamental feature of GitHub that enable developers to propose changes to a project's codebase. Team members can create a pull request to suggest modifications, additions, or fixes, which are then reviewed by other members of the team. PRs provide a structured way to discuss and collaborate on code changes before they are merged into the main branch.

2. **Code Reviews:** GitHub provides robust tools for conducting code reviews within pull requests. Team members can review the proposed changes line-by-line, leave comments, suggest improvements, and discuss any concerns directly within the GitHub interface. Code reviews help ensure code quality, adherence to coding standards, and knowledge sharing among team members.

3. **Branching and Merging:** GitHub allows developers to create branches within a repository, providing a way to work on features or fixes independently of the main codebase. Once changes are completed, they can be merged back into the main branch (e.g., master) through pull requests. GitHub offers features like branch protection rules to enforce review processes and prevent direct commits to certain branches, ensuring code stability and integrity.

4. **Issue Tracking:** GitHub's issue tracking system provides a centralized way to manage tasks, bugs, and feature requests within a project. Team members can create issues, assign them to individuals or teams, prioritize tasks, and track progress. Issues can be linked to pull requests, providing context and traceability between code changes and the underlying tasks or problems they address.

5. **Commenting and Discussion:** GitHub allows team members to leave comments on code, pull requests, and issues, facilitating discussion and collaboration. Comments can be used to provide feedback, ask questions, or clarify intentions, helping to ensure that everyone is on the same page and contributing effectively to the project.

6. **Conflict Resolution:** In collaborative environments, conflicts may arise when multiple team members make changes to the same file or code snippet simultaneously. GitHub provides tools for resolving conflicts during the merge process, including visual diff tools to highlight conflicting changes and options for manual resolution. Additionally, GitHub's branch protection rules and status checks can help prevent conflicts by ensuring that changes pass automated tests before they are merged.

Overall, GitHub's features for pull requests, code reviews, branching, issue tracking, commenting, and conflict resolution make it a powerful platform for facilitating collaboration among team members in software development projects. These tools help teams communicate effectively, ensure code quality, and streamline the development process.

## Challenges and Solutions
See the [project issues](https://github.com/quyen-ong/Dockerized-Flutter-App/issues) section for active and historical issues.

## Conclusion
Using GitHub provides numerous benefits, such as collaboration and version control. There's no longer any issue with losing previous progress because GitHub allows you to easily retreive previous code. You can also compare old code and new code to find what changes are causing issues. GitHub also makes it easy to share your work by simply giving people access and sending a link. Additionally, Github has GitHub Actions which allows you to automate your build, test, and deployment pipeline.