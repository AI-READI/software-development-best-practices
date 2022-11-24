---
lang: en-US
title: Overview
description: Software Development Best Practices of the AI-READI Project
---

# Pushing changes to GitHub repository

1. Use two branches for your software: `main` and `dev`. The `main` branch will be the most stable. The `dev` branch contains new features, and more unstable branches may be pull requested to this branch. Only bug fix branches should be merged directly into the `main` branch and these merges should be initiated by a Pull Request (PR) from the bug fix branch. All additional features/bug fixes should always be developed and merged via feature branches. [Category: C] [Ref: 3]
2. When committing a change to the repository, make sure the change reflects a single purpose (e.g. fixing a bug or adding a new feature) [Category: C] [Ref: 3]
3. Use [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/#specification) [Category: C] [ Ref: 1]
4. Make sure your git commit hooks are always run before committing to the public repository. Avoid skipping these hooks as they might run important actions on your system.
5. When merging changes to the dev branch, create a PR from the feature or bug fix branch and invite at least one other collaborator to review the changes. Leave comments in the PR to clarify intent, decision points or particular sections to review to ensure the reviewer can focus on the areas of importance. Reviewers should use the PR to respectfully ask clarifying questions or make suggestions of the approach when appropriate.
