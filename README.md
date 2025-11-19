# Ops Knowledge Base

[![Deploy Hugo site to Pages](https://github.com/imfing/hextra-starter-template/actions/workflows/pages.yaml/badge.svg)](https://github.com/imfing/hextra-starter-template/actions/workflows/pages.yaml)

This repository is a personal knowledge base for DevOps and Ops-related topics. It's built with [Hugo](https://gohugo.io/) and the [Hextra theme](https://github.com/imfing/hextra).

## Content

This repository contains two main types of content:

-   **`/content/docs/technologies`**: This section is for reference material about different technologies. It contains "how-to" guides and reference material for the technology itself. For example, you can find information about AWS, Docker, or Kubernetes here.

-   **`/content/docs/playbooks`**: This section is for troubleshooting specific issues. It contains step-by-step guides to fix a problem. For example, a playbook might detail how to resolve a "container-oomkilled" error.

## Local Development

To run the site locally, you need [Hugo](https://gohugo.io/getting-started/installing/), [Go](https://golang.org/doc/install), and [Git](https://git-scm.com).

```shell
# Clone the repo
git clone https://github.com/gemini-cli-test/ops.git
cd ops

# Tidy modules and start the server
hugo mod tidy
hugo server
```

### Update Theme

To update the Hextra theme and other modules:

```shell
hugo mod get -u
hugo mod tidy
```

## Deployment

This site is set up to deploy automatically to GitHub Pages using the workflow in `.github/workflows/pages.yaml`.

## Credits

This site is built using the fantastic [Hextra theme](https://github.com/imfing/hextra) created by [imfing](https://github.com/imfing). The original starter template can be found [here](https://github.com/imfing/hextra-starter-template).