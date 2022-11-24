# 6. Version release

* 6.1. Document changes between versions of your software in a "CHANGELOG.md" file located at the root of your GitHub repository [Category: C] [Ref: 1]
   * 6.1.1. Follow the Semantic Versioning 2.0 principles outlined [here](https://semver.org) for version numbering [Category: C] [Ref: 1]
   * 6.1.2. Follow the "[keep a changelog](https://keepachangelog.com/en/1.0.0/)" guidelines for structuring your CHANGELOG file [Category: C] [Ref: 1]
* 6.2. Make a GitHub release for each version of your software [Category: A] [Ref: 1]
   * 6.2.1. Use an automated git changelog builder based on conventional commits to document the changes for each release [Category: D] [Ref: 1]
* 6.3. Deposit in a language-specific repository if available: [Category: A] [Ref: 2]
   * 6.3.1. Python packages: [PyPI](https://pypi.org/) [Category: A] [Ref: 2]
   * 6.3.2. R packages: [CRAN](https://cran.r-project.org/) [Category: A] [Ref: 2]
   * 6.3.3. Docker-based tools: [Dockstore](https://dockstore.org/) [Category: A] [Ref: 2, 5]
   * 6.3.4. JavaScript packages: [npm](https://www.npmjs.com/) [Category: A] [Ref: 1]
* 6.4. Deposit in a domain-specific repository if available:
   * 6.4.1. Computational neuroscience models: [ModelDB](https://senselab.med.yale.edu/ModelDB) [Category: A] [Ref: 2]
   * 6.4.2. R-packages aimed at the analysis of genomics data: [Bioconductor](https://www.bioconductor.org/) [Category: A] [Ref: 2, 5]
* 6.5. Deposit software on [Zenodo](https://zenodo.org/): [Category: A] [Ref: 2, 4-7]
   * 6.5.1. Include source code [Category: A] [Ref: 2, 5]
   * 6.5.2. Include executable and other files necessary to run the software if applicable [Category: A] [Ref: 2, 5]
* 6.6. Share software on the [bio.tools](https://bio.tools/) registry if the software could be of interest to the larger biomedical community outside the AI-READI project [Category: A] [Ref: 2, 7]
