# Source Code Version Control Tools
Version control is crucial in software development as it allows changes to be tracked, preserve previous code, and facillitate collaboration. Version control also helps maintain integrity by controlling permissions and access so that only authorized individuals can make modifications to the code. Since all changes are tracked, previous versions of code can be retrieved if the new code is causing issues. 

## Version Control System Used
For this project, [GitHub](https://github.com/) is used. One of the reasons GitHub was chosen is because it has a large community, making it easy to access support if needed and collaborate with others. About 100 million developers over the world use GitHub. Also, GitHub has many powerful tools, such as GitHub actions which is a continuous integration and continuous delivery (CI/CD) platform that allows you to automate your build, test, and deployment pipeline. 

## Respository Setup

## Common Commands and Usage
These are some commonly used commands in this project.

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone ssh://git@github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |
| `git commit -m "[commit message]"` | Commit changes |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout [branch name]` | Switch to a branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

## Collaboration Features

## Challenges and Solutions

## Conclusion
Using GitHub provides numerous benefits, such as collaboration and version control. There's no longer any issue with losing previous progress because GitHub allows you to easily retreive previous code. You can also compare old code and new code to find what changes are causing issues. GitHub also makes it easy to share your work by simply giving people access and sending a link. Additionally, Github has GitHub Actions which allows you to automate your build, test, and deployment pipeline.