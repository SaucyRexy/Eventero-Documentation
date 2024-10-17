# Git Workflow for Eventero Documentation

## Branching Strategy

- **Main Branch**: The production branch, where only approved changes are merged.
- **Feature Branches**: New documentation updates should be developed in feature branches.
  - Branch naming convention: `feature/<feature-name>`.
  - Example: `feature/login-documentation`, `feature/add-changelog`.
- **Hotfix Branches**: Urgent fixes or corrections.
  - Branch naming convention: `hotfix/<fix-description>`.
  - Example: `hotfix/correct-typo`.

## Pull Request Guidelines

- Create a new pull request when your feature branch is ready.
  - Title: Provide a short description (e.g., "Add API documentation for Login/Signup").
  - Description: Detail the changes and issues resolved.
  - Link any relevant issues or milestones.
- Assign at least one reviewer.
- Changelog updates should be included if needed.

## Review Process

- Every pull request requires at least one reviewer approval before merging. Typically this would be @SaucyRexy as the documentation lead.
- Use inline comments to suggest changes or improvements.
- Ensure that the documentation adheres to the format specified in the Documentation Guide.
- Once approved, the PR can be merged into the main branch.

## Merging Changes

- Ensure all checks pass.
- Changelog is updated, reflecting the new version (if applicable).
- Use `git merge` to integrate changes into the main branch.
