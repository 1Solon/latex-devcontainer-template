<div align="center">

## Latex Template

_My personal LateX report template_

</div>

<div align="center">

![GitHub Repo stars](https://img.shields.io/github/stars/1Solon/AS2-AES-Encryption?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/1Solon/AS2-AES-Encryption?style=for-the-badge)

</div>

## Usage

The template is made to be used with the DevContainer, to do so, open the project in Visual Studio Code and click the "Reopen in Container" button that appears in the bottom right corner of the window.

## Adding new libraries

You can add new libraries in two ways:

#### Manually (One-Time)

When inside the devcontainer, open the terminal and run the following command:

```bash
tlmgr install <package>
```

#### Automatically (Every Time)

First, navigate to [devcontainer.json](.devcontainer/devcontainer.json) and add the following line to the `postCreateCommand` array:

```json
"tlmgr install <package>"
```

Note that by default, the template installs `tex-gyre` so, you should be able to install any other package by just including it after it. For example:

```json
"tlmgr install tex-gyre <package>"
```

## Acknowledgements

This template uses [qmcgaw/latexdevcontainer](https://hub.docker.com/r/qmcgaw/latexdevcontainer/) as a base, please consider supporting them!