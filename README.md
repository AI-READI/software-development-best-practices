<div align="center">
<!-- HEADER -->
<br />

<p>

  <h1 align="center"> Software Development Best Practices of the AI-READI Project </h1>
  <h3 align="center"> View the latest version of the best practices: </h3>
  <p align="center">
    <a href="https://dev.aireadi.org"><strong> :globe_with_meridians: On our development website » </strong></a>
    <br />
    <a href="https://github.com/AI-READI/software-development-best-practices/tree/main/versions"><strong> :file_folder: In this repository »</strong></a>
    <br />
    <a href="https://doi.org/10.5281/zenodo.7363101"><strong> :cloud: On Zenodo » </strong></a>
    <br />
    <br />
    <a href="https://github.com/AI-READI/software-development-best-practices/issues/new">:warning: Report Issue or make suggestions</a>
  </p>
</p>

<br />

  <p>
    <a href="https://github.com/AI-READI/software-development-best-practices/stargazers">
      <img src="https://img.shields.io/github/stars/AI-READI/software-development-best-practices.svg?style=flat-square" alt="stars" />
    </a>
    <a href="https://github.com/AI-READI/software-development-best-practices/issues/">
      <img src="https://img.shields.io/github/issues/AI-READI/software-development-best-practices.svg?style=flat-square" alt="open issues" />
    </a>
    <a href="https://github.com/AI-READI/software-development-best-practices/blob/main/LICENSE">
      <img src="https://img.shields.io/github/license/AI-READI/software-development-best-practices.svg?style=flat-square" alt="license" />
    </a>
    <a href="https://doi.org/10.5281/zenodo.7363101">
      <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7363101.svg" alt="doi" />
    </a>
  </p>
</div>
<!-- TABLE OF CONTENTS -->

## Table of Contents

- [About](#about)
- [Repository structure](#repository-structure)
- [Feedback and suggestions](#feedback-and-suggestions)
- [New version release process](#new-version-release-process)
- [License](#license)
- [How to cite](#how-to-cite)
- [Acknowledgement](#acknowledgement)

## About
This repository is meant to share and maintain the software development best practices of the AI-READI project. The rationales for establishing these best practices are to:
- Help the standardization of the AI-READI software to facilitate future reuse, i.e. make the AI-READI software Findable, Accessible, Interoperable, and Reusable (FAIR)
- Ensure the efficient and effective development of software across the project, especially when contributions from several teams are required
- Facilitate on-boarding of new developers to the project

Our focus here is on establishing actionable best practices that can be directly implemented by the project's developers. These best practices are intended to remain general enough that they can apply to any software development project within AI-READI.

This repository is also meant to collect feedback/suggestions (through the [GitHub issues](https://github.com/AI-READI/software-dev-best-practices/issues/new)) such that we can improve our guidelines and/or align them with external teams (e.g., other teams from the Bridge2AI consortium).

## Repository structure
Each version of the best practices is stored in a dedicated folder under the `versions` folder. Each version includes:
1. The best practices, are provided in markdown format (one file per section of the best practices).
2. The rationale behind the different elements of the best practices, is provided in markdown format.
3. The approach for monitoring the implementation of the best practices in the project, provided in markdown format.
4. A pdf file combining all of the above.

Changes between the different versions are tracked in the [CHANGELOG](https://github.com/fairdataihub/FAIR-BioRS-guidelines/blob/main/CHANGELOG.md) file. A `main` folder contains the latest version of the best practices. Pull requests with suggestions should be made from that folder.

## Feedback and suggestions
Use the [GitHub issues](https://github.com/AI-READI/software-dev-best-practices/issues) for submitting feedback or making suggestions. You can also fork the repository and submit a pull request with suggestions by making changes to the files in the `main` folder. Only edit the markdown files (the pdf files will be created by the approvers of the suggested changes). Suggestions will be reviewed and, if deemed adequate, approved by the AI-READI Tools module PIs (with the inclusion of other team members as necessary). 

## New version release process
When changes are approved to the `main` folder, a copy with a new version number will be added to the `versions` folder.

A GitHub release is created for each new version of the best practices. The pdf version of the best practice document is archived on Zenodo with each release such that each version of the best practices can be referenced with a unique digital object identifier (DOI). Additionally, the latest version of best practices will be visible on [dev.aireadi.org](http://dev.aireadi.org), the developer documentation website for the AI-READI project. This documentation will display the best practices in a user-friendly manner and will contain additional elements (e.g., code snippets) such that the best practices can be easily implemented by developers.

## License
This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by]. See [LICENSE](https://github.com/AI-READI/software-development-best-practices/blob/main/LICENSE) for more information.

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png


## How to cite
If you are following these best practices or reusing them for any purpose, please cite:
```bash
Patel, Bhavesh, Soundarajan, Sanjay, McWeeney, Shannon, Cordier, Benjamin A., & Benton, Erik S. (2022). 
Software Development Best Practices of the AI-READI Project (v1.0.0). Zenodo. https://doi.org/10.5281/zenodo.7363102
```

## Acknowledgement
This project is funded by the NIH under award number 1OT2OD032644. The content is solely the responsibility of the authors and does not necessarily represent the official views of the NIH.

<br />

---

<br />

<div align="center">

<a href="https://aireadi.org">
  <img src="https://github.com/AI-READI/AI-READI-logo/raw/main/logo/png/option2.png" height="200" />
</a>

</div>
  
