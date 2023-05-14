# git_workflow_demo

This is meant to be a demo to get your feet when using git for version control. This guide requires no previous experience with git or version control.

# References

[GitHub Git cheat sheet](https://education.github.com/git-cheat-sheet-education.pdf)

[Gitlab Git cheat sheet](https://about.gitlab.com/images/press/git-cheat-sheet.pdf)

# Overview

## Introduction to Version Control Systems:
- Version control allows you to track changes made to files over time, providing a history of modifications.
- Benefits include the ability to collaborate effectively, revert to previous versions, and manage conflicts.
- Example: Imagine working on a project with multiple team members. Version control enables everyone to work on their tasks independently and later merge their changes seamlessly.

## Introduction to Git:
- Git is a distributed version control system designed for speed, efficiency, and collaboration.
- Unlike centralized systems, Git stores a complete copy of the repository on each user's local machine.
- Users can work offline, commit changes locally, and later synchronize with remote repositories.
- Example: Suppose you're developing a web application. Git allows you to track changes, experiment with new features, and collaborate with other developers effectively.

## Installing Git:
- Participants should visit the official Git website (https://git-scm.com/) to download and install Git for their respective operating systems.
- Installation options vary across platforms, but typically include downloading an installer and following the provided instructions.
- Explain any additional configurations, such as configuring the default text editor and setting up SSH keys for secure authentication.

## Configuring Git:
- After installing Git, participants need to configure their name and email address using the following commands:
    - `git config --global user.name "Your Name"`
    - `git config --global user.email "your.email@example.com"`
- These configurations ensure that commits are attributed to the correct author.

## Initializing a Repository:
- To create a new Git repository, navigate to the desired project directory in the command line and run `git init`.
- This initializes an empty Git repository, creating a hidden `.git` folder to store the project's history and metadata.
- Example: Open a command prompt, navigate to a project folder (e.g., `cd myproject`), and run `git init` to create a repository for that project.

## Basic Git Workflow:
- `git add`: Use this command to stage changes and prepare files for committing. For example, `git add file1.txt` stages `file1.txt` for the next commit.
- `git commit`: Record changes to the repository. Each commit represents a snapshot of the project at a specific point in time. Example: `git commit -m "Added new feature"`.
- `git status`: Check the status of the repository, displaying modified files, staged changes, and other information.
- `git log`: View the commit history, showing information such as commit hash, author, date, and commit message.

## Branching and Merging:
- Branches are independent lines of development. Use `git branch` to create, list, and delete branches. For example, `git branch feature-branch` creates a new branch called "feature-branch".
- Switch between branches using `git checkout`. For instance, `git checkout feature-branch` moves to the "feature-branch" branch.
- Merging integrates changes from one branch into another. Use `git merge` to merge branches. Example: `git merge feature-branch` merges the changes from "feature-branch" into the current branch.

## Remote Repositories and Collaborative Workflow:
- Remote repositories are copies of a repository hosted on a server, enabling collaboration with others.
- Clone a remote repository using `git clone`. For instance, `git clone https://github.com/user/repo.git` downloads a remote repository to the local machine.
- Use `git push` to upload local commits to a remote repository

## Resolving Conflicts:
- Discuss the common scenarios where conflicts occur: Conflicts happen when two or more people make conflicting changes to the same file or lines of code.
- Show how to resolve conflicts by manually editing conflicting files and using Git's conflict resolution tools: When conflicts arise, Git highlights the conflicting areas, and you can manually edit the files to resolve conflicts. Git also provides commands like `git mergetool` to help with conflict resolution.

## Additional Git Features:
- Gitignore - Ignoring files in the repository: Create a .gitignore file to specify files or patterns that Git should ignore.
- Git stash - Temporarily saving and applying changes: Use `git stash` to save changes that you're not ready to commit, allowing you to switch branches or work on something else.
- Git branch management - Renaming and deleting branches: Show how to rename branches using `git branch -m` and delete branches using `git branch -d`.
- Git tags - Assigning meaningful names to specific commits: Demonstrate how to create lightweight tags (`git tag`) or annotated tags (`git tag -a`) to mark specific points in the commit history.

## Best Practices and Resources:
- Share some Git best practices, such as:
    - Writing descriptive commit messages: Explain the importance of clear and meaningful commit messages to improve collaboration and code understanding.
    - Regularly committing changes: Encourage frequent commits to create a more granular history of the project's progress.
- Provide recommended resources, like documentation, tutorials, and cheat sheets, for further learning: Mention official Git documentation, online tutorials, video courses, and interactive Git platforms like GitHub and GitLab.
