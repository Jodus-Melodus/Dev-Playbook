# Docker
You can view some Docker templates [here](DockerTemplates.md).

## Setup Docker
### Install
1. Install [Docker](https://www.docker.com/).
2. Install the [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extention in VSCode.
3. Install the [Container Tools](https://marketplace.visualstudio.com/items?itemName=ms-azuretools.vscode-containers) extention in VSCode.
### Project Setup
1. Open your project in VSCode.
2. Ensure Docker is running.
3. Make a folder `.devcontainer` and a file in the folder `devcontainer.json`.
4. Paste this in the `devcontainer.json` file.
```json
{
    "name": "<your project name>",
    "build": {
        "dockerfile": "../Dockerfile"
    },
    "workspaceFolder": "/workspace",
    "mounts": [
        "source=${localWorkspaceFolder},target=/workspace,type=bind"
    ]
}
```
4. Create a `Dockerfile` in your main directory.
5. Paste this in the `Dockerfile` file. (Basic Docker template for C)
```Dockerfile
FROM ubuntu:24.04

RUN apt-get update && apt-get install -y \
    build-essential \
    cmake \
    gdb \
    git \
    && rm -rf /var/lib/apt/lists/*

WORKDIR /workspace

CMD [ "bash" ]
```
6. Save and close all editors.
### Opening VSCode in the container
1. Press `F1` and type `Dev Containers: Rebuild and Reopen in Container` and `enter`



