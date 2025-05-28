# Minimal DevContainer Template

[![DevContainer](https://img.shields.io/badge/devcontainer-ready-blue)](https://code.visualstudio.com/docs/devcontainers/containers)
[![Docker](https://img.shields.io/badge/docker-ready-blue)](https://www.docker.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## Overview

This is a minimal, language-agnostic [DevContainer](https://containers.dev/) setup designed for fast startup and easy extension. It provides a Docker-based development environment configured for use with Visual Studio Code Remote - Containers.

> In this updated version, it integrates a custom Zsh shell setup feature, configurable with Oh My Zsh, Powerlevel10k, Meslo Nerd Fonts, plugins, and timezone support.

## Features

- Based on the official `mcr.microsoft.com/devcontainers/base:ubuntu` image
- Non-root `vscode` user for safe, consistent dev workflows
- Lightweight: includes only essential tools (git, curl, bash)
- VS Code Docker extension pre-installed
- Optional advanced shell configuration via the custom shell feature
- Clean starting point for building language-specific environments

## Usage

1. Clone or fork this repository:

   ```bash
   git clone git@github.com:jonmatum/devcontainer-minimal-template.git
   cd devcontainer-minimal-template
   ```

2. Open the folder in [Visual Studio Code](https://code.visualstudio.com/):

   - You will be prompted to reopen the folder in a Dev Container.

3. Customize the Dockerfile and `devcontainer.json` for your stack.

For example, to enable the custom shell feature:

```json
"features": {
  "ghcr.io/jonmatum/devcontainer-features/shell:latest": {
    "timezone": "America/Costa_Rica",
    "opinionated": true
  }
}
```

## File Structure

```
.devcontainer/
├── devcontainer.json
```

## Requirements

- [Docker](https://docs.docker.com/get-docker/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [Remote - Containers extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)

## License

This project is licensed under the [MIT License](LICENSE).

## More Resources

- [10 Reasons Why DevContainers Are Game Changers](https://jonmatum.github.io/slidev-devcontainers-simplified/)
- [DevContainers Official Documentation](https://containers.dev/)

---

```shell
echo 'Pura Vida & Happy Coding!';
```
