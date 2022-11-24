# 6. Version release

* a. Document changes between versions of your software in a "CHANGELOG.md" file located at the root of your GitHub repository [Category: C] [Ref: 1]
   * i. Follow the Semantic Versioning 2.0 principles outlined [here](https://semver.org) for version numbering [Category: C] [Ref: 1]
   * ii. Follow the "[keep a changelog](https://keepachangelog.com/en/1.0.0/)" guidelines for structuring your CHANGELOG file [Category: C] [Ref: 1]
* b. Make a GitHub release for each version of your software [Category: A] [Ref: 1]
   * i. Use an automated git changelog builder based on conventional commits to document the changes for each release [Category: D] [Ref: 1]
* c. Deposit in a language-specific repository if available: [Category: A] [Ref: 2]
   * i. Python packages: [PyPI](https://pypi.org/) [Category: A] [Ref: 2]
   * ii. R packages: [CRAN](https://cran.r-project.org/) [Category: A] [Ref: 2]
   * iii. Docker-based tools: [Dockstore](https://dockstore.org/) [Category: A] [Ref: 2, 5]
   * iv. JavaScript packages: [npm](https://www.npmjs.com/) [Category: A] [Ref: 1]
* d. Deposit in a domain-specific repository if available:
   * i. Computational neuroscience models: [ModelDB](https://senselab.med.yale.edu/ModelDB) [Category: A] [Ref: 2]
   * ii. R-packages aimed at the analysis of genomics data: [Bioconductor](https://www.bioconductor.org/) [Category: A] [Ref: 2, 5]
* e. Deposit software on [Zenodo](https://zenodo.org/): [Category: A] [Ref: 2, 4-7]
   * i. Include source code [Category: A] [Ref: 2, 5]
   * ii. Include executable and other files necessary to run the software if applicable [Category: A] [Ref: 2, 5]
* f. Share software on the [bio.tools](https://bio.tools/) registry if the software could be of interest to the larger biomedical community outside the AI-READI project [Category: A] [Ref: 2, 7]
