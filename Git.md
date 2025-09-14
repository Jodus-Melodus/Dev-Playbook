# Git
Frequently used Git commands.

# Table of Contents
- [Creating a local repository](#creating-a-local-repository)
- [Cloning a repository](#cloning-a-repository)
- [Committing and pushing](#committing-and-pushing)

## Creating a local repository
1. Create a new directory for your project and navigate into it.
2. Initialize the repository with the following command.
```bash
git init
```
3. Add files
```bash
git add .
```
4. Commit changes
```bash
git commit -m "init"
```
5. (Optional) Link to remote
   If you want to push to GitHub
```bash
git remote add origin <github path to your repository>
git push -u origin master
```
Replace `<github path to your repository>` with your GitHub path to the repository.
E.g. `https://github.com/your-username/your-repo.git`

## Cloning a repository
This will automatically connect a remote to the GitHub repository.
1. Navigate to the repository and click on the green Code button.
<img width="407" height="372" alt="image" src="https://github.com/user-attachments/assets/a5389d18-0045-484a-a98b-68a30ef7e810" />

2. Copy the repository link.
3. On your local machine, navigate to where you would like to clone and open a terminal by right-clicking and clicking on `Open in Terminal`.
4. Type the following command in your terminal.
```bash
git clone <the-link-to-the-repository-you-copied>
```

## Committing and pushing
1. Add all your files to the commit
```bash
git add .
```
2. Commit
```bash
git commit -m "<commit message>"
```
Replace `<commit message>` with your commit message
3. Push to the repository (if your repository is on GitHub)
```bash
git push
```
