---
lang: en-US
title: Overview
description: Software Development Best Practices of the AI-READI Project
---

# Suggested automation tools/Developer experience

In this section, we provide suggestions of automated tools and approaches to fullfill some of the items from section 1-6. These are purely suggestions and developers are free to follow other approaches as long as they fullfill all the items from section 1-6.

1. Unless you have a preferred code editor, use [VS Code](https://code.visualstudio.com/) for developing your code and include the `.vscode` directory in your GitHub repository.
2. Use these VS Code extensions (or their equivalent in your preferred code editor) as applicable to your project to automatically implement some elements of the best practices: [Category: D] [Ref: 1]
   - [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments): Help you create more human-friendly comments and visualize them in your code.
   - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint): Integrates ESLint code formatting into VS Code for Javascript projects.
   - [Isort](https://marketplace.visualstudio.com/items?itemName=ms-python.isort): A Visual Studio Code extension that provides import sorting for Python using isort.
   - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - Code formatter: Prettier is an opinionated code formatter. It enforces a consistent style by parsing your code and re-printing it with its own rules that take the maximum line length into account, wrapping code when necessary.
   - [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin): A TypeScript server plugin to make the TypeScript server know `*.vue` files.
3. Use an appropriate linter for additional code quality checks before pushing a commit (eg: [Flake](https://pypi.org/project/flake8/)/[Black](https://pypi.org/project/black/) for Python, [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)/[Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) for Javascript, etc…)
4. When adding automated testing to your application try to use the following testing frameworks if possible:
   - Javascript:
     - Unit/Integration - [Vitest](https://vitest.dev/)/[Jest](https://jestjs.io/)
     - End-to-end - [Cypress](https://www.cypress.io/)
   - Python:
     - Unit/Integration - [pytest](https://docs.pytest.org/en/7.2.x/)
5. Use [GitHub actions](https://github.com/features/actions) to automate tasks such as fixing grammatical errors, formatting code, managing GitHub issue submission, stale issues and PRs, run unit/integration or end-to-end tests, build and release app/api/documentation versions on GitHub and Zenodo. Include GitHub action workflows in a `.github/workflows` folder in your repository. Standard workflow files are maintained for the AI-READI project in the `github-workflows` repository and can be copied into your software repository. [Category: D] [Ref: 1]
6. Use [TypeScript](https://www.typescriptlang.org/) for any web/Node.js applications instead of JavaScript where possible. TypeScript is a strongly typed programming language that extends JavaScript, for a better developer experience and more fault tolerant applications. [Category: D][ref: 1]
7. Use [Docusaurus](https://docusaurus.io/) for developing and maintaining simple hostable development and/or user documentation [Category: D] [Ref: 1]
8. Use [FAIRshare](https://docs.fairshareapp.io/docs/intro) to create metadata files easily, make GitHub releases, share software files on Zenodo, and register the software on bio.tools [Category: D] [Ref: 1-2]
9. Mirror repository on GitLab for backup. The AI-READI organization has GitLab sync automatically set up so no further actions are required [Category: D] [Ref: 1]
