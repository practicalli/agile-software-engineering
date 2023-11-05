# Practicalli Software Engineering

```none
██████╗ ██████╗  █████╗  ██████╗████████╗██╗ ██████╗ █████╗ ██╗     ██╗     ██╗
██╔══██╗██╔══██╗██╔══██╗██╔════╝╚══██╔══╝██║██╔════╝██╔══██╗██║     ██║     ██║
██████╔╝██████╔╝███████║██║        ██║   ██║██║     ███████║██║     ██║     ██║
██╔═══╝ ██╔══██╗██╔══██║██║        ██║   ██║██║     ██╔══██║██║     ██║     ██║
██║     ██║  ██║██║  ██║╚██████╗   ██║   ██║╚██████╗██║  ██║███████╗███████╗██║
╚═╝     ╚═╝  ╚═╝╚═╝  ╚═╝ ╚═════╝   ╚═╝   ╚═╝ ╚═════╝╚═╝  ╚═╝╚══════╝╚══════╝╚═╝
```

## Book Overview

A practical guide to software development practices and tools.


## Book status

[![MegaLinter](https://github.com/practicalli/software-engineering/actions/workflows/megalinter.yaml/badge.svg)](https://github.com/practicalli/software-engineering/actions/workflows/megalinter.yaml)[![Publish Book](https://github.com/practicalli/software-engineering/actions/workflows/publish-book.yaml/badge.svg)](https://github.com/practicalli/software-engineering/actions/workflows/publish-book.yaml)
[![Publish Book](https://github.com/practicalli/software-engineering/actions/workflows/publish-book.yaml/badge.svg)](https://github.com/practicalli/software-engineering/actions/workflows/publish-book.yaml)
[![pages-build-deployment](https://github.com/practicalli/software-engineering/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/practicalli/software-engineering/actions/workflows/pages/pages-build-deployment)

[![Ideas & Issues](https://img.shields.io/github/issues/practicalli/software-engineering?label=content%20ideas%20and%20issues&logoColor=green&style=for-the-badge)](https://github.com/practicalli/software-engineering/issues)
[![Pull requests](https://img.shields.io/github/issues-pr/practicalli/software-engineering?style=for-the-badge)](https://github.com/practicalli/software-engineering/pulls)

![GitHub commit activity](https://img.shields.io/github/commit-activity/m/practicalli/software-engineering?style=for-the-badge)
![GitHub contributors](https://img.shields.io/github/contributors/practicalli/software-engineering?style=for-the-badge&label=github%20contributors)

## Creative commons license

<div style="width:95%; margin:auto;">
  <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a>
  This work is licensed under a Creative Commons Attribution 4.0 ShareAlike License (including images & stylesheets).
</div>

## Contributing

Issues and pull requests are most welcome although it is the maintainers discression as to if they are applicable.  Please detail issues as much as you can.  Pull requests are simpler to work with when they are specific to a page or at most a section.  The smaller the change the quicker it is to review and merge.

Please read the [detailed contributing section of the book](https://practical.li/software-engineering/introduction/contributing/) before raising an issue or pull request to avoid disapointment.

* [Current Issues](https://github.com/practicalli/software-engineering/issues)
* [Current pull requests](https://github.com/practicalli/software-engineering/pulls)

By submitting content ideas and corrections you are agreeing they can be used in any work by Practicalli under the [Creative Commons Attribution ShareAlike 4.0 International license](https://creativecommons.org/licenses/by-sa/4.0/).  Attribution will be detailed via [GitHub contributors](https://github.com/practicalli/software-engineering/graphs/contributors).

## Sponsor Practicalli

[![Sponsor practicalli-john](https://raw.githubusercontent.com/practicalli/graphic-design/live/buttons/practicalli-github-sponsors-button.png)](https://github.com/sponsors/practicalli-john/)

The majority of my work is focused on the [Practicalli series of books and videos](https://practical.li/) and an advisory role with several communities

Thank you to [Cognitect](https://www.cognitect.com/), [Nubank](https://nubank.com.br/) and a wide range of other [sponsors](https://github.com/sponsors/practicalli-john#sponsors) for your continued support


## GitHub Actions

The megalinter GitHub actions will run when a pull request is created,checking basic markdown syntax.

A review of the change will be carried out by the Practicalli team and the PR merged if the change is acceptable.

The Publish Book GitHub action will run when PR's are merged into main (or the Practicalli team pushes changes to the default branch).

Publish book workflow installs Material for MkDocs version 9


## Local development

[practicalli/software-engineering repository](https://github.com/practicalli/software-engineering){target=_blank} contains the content for this book

Install mkdocs version 9 using the Python pip package manager

```bash
pip install mkdocs-material=="9.*"
```

Install the plugins used by the Practicalli site using Pip (these are also installed in the GitHub Action workflow)

```bash
pip3 install mkdocs-material mkdocs-callouts mkdocs-glightbox mkdocs-git-revision-date-localized-plugin mkdocs-redirects pillow cairosvg
```

> pillow and cairosvg python packages are required for [Social Cards](https://squidfunk.github.io/mkdocs-material/setup/setting-up-social-cards/)

Fork the GitHub repository and clone that fork to your computer,

```bash
git clone https://github.com/<your-github-account>/<repository>.git
```

Run a local server from the root of the cloned project

```bash
make docs
```

The website will open at <http://localhost:8000>

If making smaller changes, then only rebuild the content that changes, speeding up the local development process
```bash
make docs-changed
```

