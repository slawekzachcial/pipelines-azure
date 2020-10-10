# Pipelines: Azure

This project implements a simple [Continuous Delivery
Pipeline](https://en.wikipedia.org/wiki/Continuous_delivery), based on [Azure
Pipelines](https://azure.microsoft.com/en-us/services/devops/pipelines/).

The repository is configured with [GitHub Pages](https://pages.github.com/).
The deployment consists of putting the content of the `main` branch into
`gh-pages` branch which publishes it to the [website](https://slawekzachcial.github.io/pipelines-azure/).

## Spell Check

The pipeline will check the spelling of all markdown files in this repository.

## Link Check

The pipeline will check the links of all markdown files in this repository.

## Release Creation

The pipeline, when run on `main` branch, will create a new Git tag and GitHub
release. A new release will be created only one does not exist yet for the given
commit.

## Release Deployment
The pipeline, when run on `main` branch, will deploy release by copying markdown
files into `gh-pages` branch.
