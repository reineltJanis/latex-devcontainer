# latex-devcontainer
Template for running sharelatex in a vscode devcontainer using Docker.

Only official images are used (sharelatex, mongodb, redis)

Allows to create and manipulate latex documents without the need to install any tex solution on your OS.

Instead the development / writing happens only in a virtualized Docker container.

## Requirements
- Docker or Docker Desktop
- Visual Studio Code
   - _Visual Studio Code Remote - Containers_ extension installed

## Getting started
1. Get the repo by cloning it via git or download as zip.
2. Opend the folder with VS Code.
3. A window will prompt if you want to run this solution in a devcontainer.
  If not, open the command palette (ctrl. + shift + P) to execute `> Remote-Containers: Rebuild and Reopen in Container`.
4. Take a look at the sample file and try to build it.
5. If your latex file requires additional packages, you can use the terminal with tlmgr to install them or modify in `.devcontainer/devconatiner.json` the `postCreateCommand` to point to your tex file. Once you have made this change you need to reopen the container.

> If you need other packages you can add their installation to the `.devcontainer/Dockerfile`.

