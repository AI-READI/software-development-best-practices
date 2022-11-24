---
lang: en-US
title: Overview
description: Software Development Best Practices of the AI-READI Project
---

# Code development

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
