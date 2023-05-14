# Multi Feature Workflow Demo

## Overview

1. Set up the Demo Repository:
   - Create a new empty directory and navigate to it in the command line.
   - Initialize a new Git repository using the command `git init`.
   - Create a remote repository on a Git hosting platform (e.g., GitHub, GitLab) and obtain the repository URL.

2. Clone the Remote Repository:
   - Run the command `git clone <repository-url>` to clone the remote repository to your local machine.
   - Change your working directory to the cloned repository using `cd <repository-name>`.

3. Create and Switch to a Develop Branch:
   - Create a new branch called `develop` using `git branch develop`.
   - Switch to the `develop` branch using `git checkout develop`.

4. Add Collaborators:
   - Share the repository URL with the collaborators so they can clone it to their local machines.
   - Each collaborator should follow the steps 2 and 3 to clone the repository and switch to the `develop` branch.

5. Work on Individual Features:
   - Each collaborator should create a new branch for their feature using `git branch feature/<feature-name>`.
   - Switch to the new feature branch using `git checkout feature/<feature-name>`.
   - Make the necessary changes to implement the feature.
   - Stage and commit the changes using `git add` and `git commit`.

6. Regularly Update Feature Branch with Develop:
   - To ensure your feature branch has the most recent changes from the `develop` branch, regularly update your feature branch by merging `develop` into it.
   - Switch to your feature branch using `git checkout feature/<feature-name>`.
   - Pull the latest changes from the `develop` branch using `git pull origin develop`.
   - Resolve any merge conflicts, if any, that arise during the merge.

7. Push Feature Branch:
   - After updating your feature branch with the latest changes from `develop`, push your feature branch to the remote repository using `git push origin feature/<feature-name>`.

8. Review and Merge Features:
   - The team lead or a designated person can review the pushed feature branches.
   - Once the features are reviewed and approved, switch to the `develop` branch using `git checkout develop`.
   - Merge each feature branch into the `develop` branch using `git merge feature/<feature-name>`.
   - Resolve any merge conflicts if they arise.
   - Commit the merge changes.

9. Push the Develop Branch:
   - After merging all the features, push the `develop` branch to the remote repository using `git push origin develop`.

10. Repeat the Process for New Features:
    - Collaborators can repeat steps 5 to 9 to work on new features individually, regularly update their feature branches from `develop`, push their feature branches, review, and merge them into the `develop` branch.

By regularly updating your feature branch from the `develop` branch, you can incorporate the latest changes and minimize the chances of conflicts when merging the feature branch back into `develop`.

During the demo, participants can practice the process of updating their feature branches from `develop` using `git pull` and resolve any merge conflicts if they occur.

## Step By Step

1. Create a new remote repo in your git hosting platform of preference.

2. Create a new local directory for this demo

`mkdir git_demo`

3. Clone the repo into the new director and rename it. This is to simulate having multiple users but on one machine.

```bash
git clone git@github.com:<account>/demo_repo.git

mv demo_repo demo_repo1 # rename folder

cd demo_repo1

git config user.name "user1"
git config user.email "user1@example.com"
```

4. Repeat the above renaming it to demo_repo2, with the username user2 and email user2@example.com.

