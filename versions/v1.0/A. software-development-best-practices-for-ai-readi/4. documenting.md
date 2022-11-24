---
lang: en-US
title: Overview
description: Software Development Best Practices of the AI-READI Project
---

# Documenting

1. If more details are required to run the software from the source code in addition to what is included in the "README.md" (cf 1d.ii), include them in other markdown files and refer to them in the README. These other markdown files can be located in a "docs" folder at the root of the repository [Category: A, C] [Ref: 1]
2. If the software contains a user interface, maintain user documentation of the interface and identify in your README where the user documentation is located
   - Use the [wiki of your GitHub repository](https://docs.github.com/en/communities/documenting-your-project-with-wikis/about-wikis) for simple software [Category: A, C] [Ref: 1]
   - Build and maintain a dedicated webpage for the documentation for more complex software. Have a dedicated GitHub repository for your documentation code in this case and follow our best practices for that code as well. [Category: A, C] [Ref: 1]
3. If your software includes an application programming interface (API), it must be documented separately as per API best practices. In the AI-READI project, APIs will be documented using the [OpenAPI Specification](https://swagger.io/specification/) and [hoppscotch](https://hoppscotch.io/). Mention in your README where the API documentation is located. [Category: A, C] [Ref: 1, 6, 7]
4. Include instructions for contributing to your software in a "CONTRIBUTING.md" file located at the root of your GitHub repository [Category: C] [Ref: 4, 7]
5. Use [GitHub issues](https://docs.github.com/en/issues/tracking-your-work-with-issues/about-issues) to manage bugs/issues [Category: D] [Ref: 1]
