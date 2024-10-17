# Eventero Documentation

**Eventero Documentation** is the comprehensive documentation repository for the Campus Resource and Event Management App. This documentation aims to enhance resource utilization and increase student event participation by providing detailed information about the application, its features, and how to use them effectively.

## Repository Structure

The repository is organized into the following folders and files:

- **README.md**: This file provides an overview of the project and its purpose.

- **guides/**: This folder is designated for future general guides and how-tos for using the application:
  - **setup.md**: Installation and setup instructions for the application.
  - **usage.md**: Detailed usage instructions for navigating and utilizing the app (to be added).
  - **best_practices.md**: Recommendations for best practices when using the application (to be added).
  - **documentation_guide.md**: A template for documenting features consistently, ensuring clarity and organization in feature documentation.

- **api/**: This folder is intended for documentation related to the application's API (to be added in the future):
  - **endpoints.md**: A list of available API endpoints along with their usage.
  - **authentication.md**: Information on authentication methods and token management.
  - **error_handling.md**: Common errors encountered while using the API and their solutions.

- **features/**: Documentation specific to individual features of the application (to be added in the future):
  - **login_signup.md**: Information about the login and signup process, including user flows and API endpoints.
  - **user_profile.md**: Instructions for managing user profiles, including editing and updating information.
  - **event_creation.md**: Guidelines for creating events, covering forms, validations, and workflows.

- **changelog/**: A history of changes made to the application, reflecting a new version for each milestone:
  - **v1.0.md**: Details for milestone 1 of the application. 
  - **v2.0.md**: Details for milestone 2 of the application (to be added).
  - **v3.0.md**: Details for milestone 3 of the application (to be added) (final version).

This structure is designed to facilitate easy navigation and updates to the documentation as the application evolves. Additional guides and API documentation will be added in the future. Contributions and feedback are welcome to help improve the quality and clarity of the documentation.

## Git Workflow for Eventero Documentation

### Branching Strategy

- **Main Branch**: The production branch, where only approved changes are merged.
- **Feature Branches**: New documentation updates should be developed in feature branches.
  - Branch naming convention: `feature/<feature-name>`.
  - Example: `feature/login-documentation`, `feature/add-changelog`.
- **Hotfix Branches**: Urgent fixes or corrections.
  - Branch naming convention: `hotfix/<fix-description>`.
  - Example: `hotfix/correct-typo`.

### Pull Request Guidelines

- Create a new pull request when your feature branch is ready.
  - Title: Provide a short description (e.g., "Add API documentation for Login/Signup").
  - Description: Detail the changes and issues resolved.
  - Link any relevant issues or milestones.
- Assign at least one reviewer.
- Changelog updates should be included if needed.

### Review Process

- Every pull request requires at least one reviewer approval before merging. Typically this would be @SaucyRexy as the documentation lead.
- Use inline comments to suggest changes or improvements.
- Ensure that the documentation adheres to the format specified in the Documentation Guide.
- Once approved, the PR can be merged into the main branch.

### Merging Changes

- Ensure all checks pass.
- Changelog is updated, reflecting the new version (if applicable).
- Use `git merge` to integrate changes into the main branch.

### Running the Changelog
Before updating the changelog, make sure you have the `auto-changelog` dependency installed. If you haven't done so, run:

```bash
npm install
```
To update the changelog for version 2.0, use the following command:

```bash
npm run changelog:v2
```