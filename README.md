# MLIR WWW 🌐

Welcome to the source code repository for the MLIR website, which is hosted at [https://mlir.llvm.org/](https://mlir.llvm.org/). This website is automatically rendered from the `gh-pages` branch of this repository using GitHub Pages.

## How to Contribute 🚀

We encourage you to contribute to the development of the MLIR website. Feel free to fork this repository and submit a pull request. Your contributions help make the website better for the community.

## Automated Deployment 🤖

Our website is automatically deployed every time there's a push to this repository, thanks to a GitHub Action defined in `.github/workflows/main.yml`. Additionally, it runs every four hours to catch updates from the MLIR source repository (the LLVM monorepo), which is used for generating some of the documentation.

## Powered by Hugo 📝

We use the [Hugo](https://gohugo.io/) framework to generate our website. The source pages are written in Markdown format under the `website/content` folder.

## How to Preview Changes Locally 👨‍💻

Here's how you can preview your changes locally:

1. Download Hugo to your machine.
2. Run `hugo server` from the `website` directory.
3. Access a local version of the website at [http://localhost:1313/](http://localhost:1313/). Any changes you make to the source Markdown will be automatically refreshed by the local Hugo server.

## Auto-Generated Documentation 📚

A significant portion of our documentation is auto-generated from the MLIR source code. Check out the workflow defined in `.github/workflows/main.yml` for instructions on how to reproduce the entirety of [https://mlir.llvm.org/](https://mlir.llvm.org/) locally.

## Simplified Setup ⚙️

When making changes, you typically don't need to check out the doxygen branch. You can consider checking out only the main branch. If you're using [gh](https://cli.github.com/), you can clone the repository with the following command:

```sh
gh repo clone llvm/mlir-www -- --single-branch --branch main
