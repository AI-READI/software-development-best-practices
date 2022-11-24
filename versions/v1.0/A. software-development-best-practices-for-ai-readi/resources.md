---
lang: en-US
title: Overview
description: Software Development Best Practices of the AI-READI Project
---

# Best practices

## Software development best practices for AI-READI

Our best practices are designed to A) Comply with the FAIR4RS principles, B) Promote open-source practices, C) Facilitate collaborations and inclusivity (aligning with inclusive development and innovation which are part of the CARE principles), and D) Provide convenience to developers. The rationale for such a design is provided in Section 4 of this document. For each element of the best practices, we indicate which of the categories A-D they fulfill. Moreover, our best practices are based on the resources listed below. These resources were selected based on the authors' knowledge of their relevance to the categories A-D. For each element of the best practices, we indicate which resources it is based on.

## Project setup

1. Work from GitHub with a GitHub repository dedicated to your software in the [AI-READI organization](https://github.com/AI-READI) [Category: A, B, C] [Ref: 1-7]
2. Follow GitHub best practices [Category: C] [Ref: 9]
3. Make the GitHub repository public from day 1 [Category: B] [1, 7]
4. Choose a license and include a `LICENSE` file containing standard license terms in the root of your GitHub repository [Category: A, C] [Ref: 2-4, 7]
   - All software in the AI-READI project will be developed under the [MIT license](https://opensource.org/licenses/MIT) (unless exceptions) [Category: B] [Ref: 1]
5. Add a `README.md` file in the root of your GitHub repository and include at least the following information as they become available [Category: A, C] [Ref: 2, 4, 6]:
   - Brief description of the software [Ref: 2, 4, 6, 7,10-12]
   - How to run the software (from the source code) [Ref: 2, 4, 6, 10-12]
   - Inputs and outputs of the software, if applicable [Ref: 2]
   - Parameters, data, and data formats required to run the software, if applicable [Ref: 2, 10-12]
   - The standards followed during development (c.f. 2a) [Ref: 2, 10-12]
   - How to report bugs/issues (c.f. 4e) [Ref: 2, 10-12]
   - Acknowledgment of NIH funding support [Category: C] [Ref: 5]
   - Other acknowledgments, if applicable [Ref: 6]
   - Clear attribution for authorship and software dependencies
   - Include [shields.io](https://shields.io/) badges at the top of your README to showcase the following: license, number of contributors, number of open issues, Zenodo DOI (c.f. 6e) [Ref: 1, 6]
   - Include the AI-READI logo available [here](https://github.com/AI-READI/AI-READI-logo) at the bottom of your README [Category C][ref: 1].

## Code development

1. Follow language-specific standards and conventions when writing your code [Category: A, C] [Ref: 1, 2, 10-12]
   - Python: [Python Developer's Guide](https://devguide.python.org/)
   - R: [Google's R Style Guide](https://google.github.io/styleguide/Rguide.html)
   - Java: [Google's Java Style Guide](https://google.github.io/styleguide/javaguide.html)
2. Use an appropriate linter for automated code quality improvements and formatting fixes (c.f. section 7)
3. Give functions and variables meaningful names [Category: C] [Ref: 3, 4]
4. Include comments within your code when deemed necessary for reuse. These comments need to be added using already accepted standards or conventions (e.g: [JSDoc](https://jsdoc.app/) for JavaScript, [Google style guide for docstrings](https://google.github.io/styleguide/pyguide.html#38-comments-and-docstrings) for Python code) [Category: A, C] [Ref: 1, 2, 3, 4, 6, 10-12]
5. If using external libraries, favor well-maintained software libraries and make sure their license is compatible with your software license [Category: C] [Ref: 4, 7, 21]
6. Record software dependencies in a requirements.txt or similar file [Category: A, C] [Ref: 2, 4]
7. Add appropriate tests (unit, integration and end-to-end) to all modules in your application. Try to achieve high coverage to ensure that future developments do not cause accidental regressions in your application. Continuous Integration can/should? be setup to handle automated testing between all developers in the team. Cross browser accessibility can be handled by the end-to-end test runner [Category: B, D] [Ref: 3, 4, 11]
8. Identify and utilize tools to benchmark for accessibility such as Accessibility Insights for Web development etc. [Category: C] [Ref: 18-19]
9. Web-based software should support Modern Browsers developed with the Webkit, Blink, or Gecko rendering engines (e.g. Chrome, Safari, Firefox, MS Edge). Uncertainties around specific support for recent HTML/CSS/JavaScript features may be resolved via the CanIUse database (https://caniuse.com/). Testing of front-end layout rendering and cross-browser consistency can be performed via browser-specific development tools (e.g. Firebug, Chromium developer tools) or virtualization (e.g. https://www.browserstack.com/) if available.

## Pushing changes to GitHub repository

1. Use two branches for your software: main and dev. The main branch will be the most stable. The dev branch contains new features, and more unstable branches may be pull requested to this branch. Only bug fix branches should be merged directly into the main branch and these merges should be initiated by a Pull Request (PR) from the bug fix branch. All additional features/bug fixes should always be developed and merged via feature branches. [Category: C] [Ref: 3]
2. When committing a change to the repository, make sure the change reflects a single purpose (e.g. fixing a bug or adding a new feature) [Category: C] [Ref: 3]
3. Use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/#specification) [Category: C] [ Ref: 1]
4. Make sure your git commit hooks are always run before committing to the public repository. Avoid skipping these hooks as they might run important actions on your system.
5. When merging changes to the dev branch, create a PR from the feature or bug fix branch and invite at least one other collaborator to review the changes. Leave comments in the PR to clarify intent, decision points or particular sections to review to ensure the reviewer can focus on the areas of importance. Reviewers should use the PR to respectfully ask clarifying questions or make suggestions of the approach when appropriate.

## Documenting

1. If more details are required to run the software from the source code in addition to what is included in the "README.md" (cf 1d.ii), include them in other markdown files and refer to them in the README. These other markdown files can be located in a "docs" folder at the root of the repository [Category: A, C] [Ref: 1]
2. If the software contains a user interface, maintain user documentation of the interface and identify in your README where the user documentation is located
   - Use the [wiki of your GitHub repository](https://docs.github.com/en/communities/documenting-your-project-with-wikis/about-wikis) for simple software [Category: A, C] [Ref: 1]
   - Build and maintain a dedicated webpage for the documentation for more complex software. Have a dedicated GitHub repository for your documentation code in this case and follow our best practices for that code as well. [Category: A, C] [Ref: 1]
3. If your software includes an application programming interface (API), it must be documented separately as per API best practices. In the AI-READI project, APIs will be documented using the [OpenAPI Specification](https://swagger.io/specification/) and [hoppscotch](https://hoppscotch.io/). Mention in your README where the API documentation is located. [Category: A, C] [Ref: 1, 6, 7]
4. Include instructions for contributing to your software in a "CONTRIBUTING.md" file located at the root of your GitHub repository [Category: C] [Ref: 4, 7]
5. Use [GitHub issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues) to manage bugs/issues [Category: D] [Ref: 1]

## Adding metadata

1. Include metadata files:
   - Include a [codemeta.json](https://codemeta.github.io/) file in the root of your GitHub repository [Category: A] [Ref: 2, 7].
     Provide at least the following information: Software name ("name"), Software description/abstract ("description"), Unique identifier ("identifier"), Authors ("givenName", "familyName") with their Organization name ("affiliation"), Keywords ("keywords"), Programming Language ("programmingLanguage"), First and current release date ("datePublished" and "dateModified"), License used ("license")
   - Include a [CITATION.cff](https://citation-file-format.github.io/) file in the root of your GitHub repository [Category: A] [Ref: 2, 4, 5, 6]
     Provide at least the following information: Authors ("given-names", "family-names") with their Organization name ("affiliation"), Software description/abstract ("abstract"), Unique identifier ("identifiers"), Keywords ("keywords"), License ("license"), Release date ("date-released")

## Version release

1. Document changes between versions of your software in a "CHANGELOG.md" file located at the root of your GitHub repository [Category: C] [Ref: 1]
   - Follow the Semantic Versioning 2.0 principles outlined [here](https://semver.org) for version numbering [Category: C] [Ref: 1]
   - Follow the "[keep a changelog](https://keepachangelog.com/en/1.0.0/)" guidelines for structuring your CHANGELOG file [Category: C] [Ref: 1]
2. Make a GitHub release for each version of your software [Category: A] [Ref: 1]
   - Use an automated git changelog builder based on conventional commits to document the changes for each release [Category: D] [Ref: 1]
3. Deposit in a language-specific repository if available: [Category: A] [Ref: 2]
   - Python packages: [PyPI](https://pypi.org/) [Category: A] [Ref: 2]
   - R packages: [CRAN](https://cran.r-project.org/) [Category: A] [Ref: 2]
   - Docker-based tools: [Dockstore](https://dockstore.org/) [Category: A] [Ref: 2, 5]
   - JavaScript packages: [npm](https://www.npmjs.com/) [Category: A] [Ref: 1]
4. Deposit in a domain-specific repository if available:
   - Computational neuroscience models: [ModelDB](https://senselab.med.yale.edu/ModelDB) [Category: A] [Ref: 2]
   - R-packages aimed at the analysis of genomics data: [Bioconductor](https://www.bioconductor.org/) [Category: A] [Ref: 2, 5]
5. Deposit software on [Zenodo](https://zenodo.org/): [Category: A] [Ref: 2, 4-7]
   - Include source code [Category: A] [Ref: 2, 5]
   - Include executable and other files necessary to run the software if applicable [Category: A] [Ref: 2, 5]
6. Share software on the [bio.tools](https://bio.tools/) registry if the software could be of interest to the larger biomedical community outside the AI-READI project [Category: A] [Ref: 2, 7]

## Suggested automation tools/Developer experience

In this section, we provide suggestions of automated tools and approaches to fullfill some of the items from section 1-6. These are purely suggestions and developers are free to follow other approaches as long as they fullfill all the items from section 1-6.

1. Unless you have a preferred code editor, use [VS Code](https://code.visualstudio.com/) for developing your code and include the `.vscode` directory in your GitHub repository.
2. Use these VS Code extensions (or their equivalent in your preferred code editor) as applicable to your project to automatically implement some elements of the best practices: [Category: D] [Ref: 1]
   - [Better Comments](https://marketplace.visualstudio.com/items?itemName=aaron-bond.better-comments): Help you create more human-friendly comments and visualize them in your code.
   - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint): Integrates ESLint code formatting into VS Code for Javascript projects.
   - [Isort](https://marketplace.visualstudio.com/items?itemName=ms-python.isort): A Visual Studio Code extension that provides import sorting for Python using isort.
   - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) - Code formatter: Prettier is an opinionated code formatter. It enforces a consistent style by parsing your code and re-printing it with its own rules that take the maximum line length into account, wrapping code when necessary.
   - [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin): A TypeScript server plugin to make the TypeScript server know \*.vue files.
3. Use an appropriate linter for additional code quality checks before pushing a commit (eg: [Flake](https://pypi.org/project/flake8/)/[Black](https://pypi.org/project/black/) for Python, [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)/[Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode) for Javascript, etc…)
4. When adding automated testing to your application try to use the following testing frameworks if possible:
   - Javascript:
     - Unit/Integration - [Vitest](https://vitest.dev/)/[Jest](https://jestjs.io/)
     - End-to-end - [Cypress](https://www.cypress.io/)
   - Python:
     - Unit/Integration - [pytest](https://docs.pytest.org/en/7.2.x/)
5. Use [GitHub actions](https://github.com/features/actions) to automate tasks such as fixing grammatical errors, formatting code, managing GitHub issue submission, stale issues and PRs, run unit/integration or end-to-end tests, build and release app/api/documentation versions on GitHub and Zenodo. Include GitHub action workflows in a ".github/workflows" folder in your repository. Standard workflow files are maintained for the AI-READI project in the "github-workflows" repository and can be copied into your software repository. [Category: D] [Ref: 1]
6. Use [TypeScript](https://www.typescriptlang.org/) for any web/Node.js applications instead of JavaScript where possible. TypeScript is a strongly typed programming language that extends JavaScript, for a better developer experience and more fault tolerant applications. [Category: D][ref: 1]
7. Use [Docusaurus](https://docusaurus.io/) for developing and maintaining simple hostable development and/or user documentation [Category: D] [Ref: 1]
8. Use [FAIRshare](https://docs.fairshareapp.io/docs/intro) to create metadata files easily, make GitHub releases, share software files on Zenodo, and register the software on bio.tools [Category: D] [Ref: 1-2]
9. Mirror repository on GitLab for backup. The AI-READI organization has GitLab sync automatically set up so no further actions are required [Category: D] [Ref: 1]
