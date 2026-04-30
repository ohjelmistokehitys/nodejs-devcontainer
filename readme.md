# Development container for Node.js

This repository provides a [development container](https://code.visualstudio.com/docs/remote/containers) that includes all the necessary tools and dependencies for using Node.js and related technologies. The container is configured to work with Visual Studio Code's Remote Containers extension, allowing you to develop and run tests in a consistent environment without worrying about local setup issues. This container works both in local development using Docker and in [GitHub Codespaces](https://github.com/features/codespaces), which provides a cloud-based development environment.

To use the development container locally, you need to have [Docker](https://www.docker.com/get-started) installed on your machine and the [Visual Studio Code Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension installed. You can also open the development container in GitHub Codespaces by following [this guide](https://docs.github.com/en/codespaces/developing-in-a-codespace/creating-a-codespace-for-a-repository#creating-a-codespace).


## What's included in the repository

* `.npmrc` - Configuration file for npm, specifying the package registry and other settings.
    * Sets the `min-release-age` to 7 days to avoid installing packages that have been released very recently, which can help prevent issues with supply chain attacks and unstable packages.
    * Sets the `ignore-scripts` to true to prevent npm from running any lifecycle scripts defined in the packages, which can enhance security by avoiding the execution of potentially harmful scripts during installation.
* `.devcontainer/` - Directory containing the configuration files for the development container.
* `.github/workflows/node-ci.yml` - GitHub Actions workflow for continuous integration, which runs tests and checks for vulnerabilities on every push and pull request.
* `agents.md` - Instructions for using AI agents in the context of the course assignment.


## About the material

This repository was created by Teemu Havulinna and is licensed under [Creative Commons BY-NC-SA](https://creativecommons.org/licenses/by-nc-sa/4.0/).

Language models and AI tools such as GitHub Copilot and ChatGPT were used in creating this repository.
