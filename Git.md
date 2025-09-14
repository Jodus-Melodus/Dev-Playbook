# Git
Frequently used Git commands.

# Table of Contents
- [Creating a repository](#creating-a-repository)
- [Cloning a repository](#cloning-a-repository)
- [Committing changes](#committing-changes)
- [Pushing commits](#pushing-commits)
- [Creating a remote](#creating-a-remote)
- [Glossary](#glossary)

## Creating a repository
1. Create a new directory for your project and navigate into it.
2. Initialize the repository with the following command.
   ```bash
   git init
   ```

## Cloning a repository
This will automatically connect a remote to the GitHub repository.
1. Copy the repository [URL](#repository-url-link).
2. On your local machine, you can navigate to where you would like to clone and open a terminal.
3. Run the following command:
   ```bash
   git clone <the-link-to-the-repository-you-copied>
   ```
   Replace `<the-link-to-the-repository-you-copied>` with the link you copied.


## Committing changes
1. Add all your files to the commit
   ```bash
   git add .
   ```
2. Commit
   ```bash
   git commit -m "<commit message>"
   ```
   Replace `<commit message>` with your commit message

## Pushing commits
1. If you don't have a remote linked to your GitHub repository. [Create a remote](#create-a-remote)
2. Push
   ```bash
   git push
   ```

## Creating a remote
1. Navigate to your repository
2. Add a remote
   ```bash
   git remote add <remote name> <url link to your repository>
   ```
   Replace `<remote name>` with your desired remote name. Usually, `origin`, if you are on your master branch.
   Replace `<url link to your repository>` with the [URL link](#repository-url-link) to your repository.
3. Push to GitHub
   ```bash
   git push -u <remote name> <branch name>
   ```
   The `-u` will make this remote the default for this branch.
   Replace `<remote name>` with the remote you just created. Usually, `origin`, if you are on your master branch.
   Replace `<branch name>` with the branch you want to push to. Usually, `master`.

# Glossary
This section provides visual context and explanations for specific terms and phrases used throughout the project. Each entry includes a screenshot and a brief breakdown to aid understanding.
## Repository URL link
You can copy the repository URL here:
<img width="417" height="380" alt="image" src="https://github.com/user-attachments/assets/d652584e-ed72-4ffc-982f-0125f8554475" />





