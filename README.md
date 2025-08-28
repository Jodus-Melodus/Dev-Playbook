# Git-and-terminal-guide

## Cloning a Git repository

1. Copy the repository URL
<img width="452" height="376" alt="image" src="https://github.com/user-attachments/assets/ea31c29b-53c9-47d7-b962-f778a8d17a3e" />

2. Navigate to the directory
Go to the directory to which you want to clone the repository.

4. Clone the repository
```bash
git clone <URL of the repository that you want to clone>
```

## Initializing a project with Docker
### 1. Create a .devcontainer folder
Inside your C++ project folder:
```bash
my_project/
 ├─ src/
 ├─ include/
 ├─ Dockerfile
 └─ .devcontainer/
       └─ devcontainer.json
```
### 2. Write devcontainer.json
```json
{
  "name": "C++ Clarity Container",
  "build": {
    "dockerfile": "Dockerfile"
  },
  "workspaceFolder": "/workspace",
  "mounts": [
    "source=${localWorkspaceFolder},target=/workspace,type=bind"
  ]
}
```
### 3. Open the project in VS Code
- Open the project folder in VS Code.
- Press F1 → type “Remote-Containers: Reopen in Container”
VS Code will:
- Build the Docker image (if it doesn’t exist)
- Mount your project folder
- Open a terminal inside the container automatically
