# Git

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
