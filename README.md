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

## Writing Commits for Changelog

To ensure that commits are correctly categorized and displayed in the changelog, follow the **Conventional Commits** format:

### Commit Message Format

Commit messages should use the following structure:

```bash
<type>(<optional scope>): <subject>
<optional body>
<optional footer>
```


- **Type**: This is required and must be one of the following: `feat`, `fix`, `docs`, `style`, `refactor`, `perf`, `test`, or `chore`. The type defines the nature of the change.
- **Scope**: An optional part that indicates which module, feature, or component the change affects. This is written inside parentheses after the type.
- **Subject**: A short description of the change, using imperative mood (e.g., "add feature" instead of "added feature"). This should be concise (50 characters or less).
- **Body**: Optional, but useful for more detailed explanations or reasoning behind the change.
- **Footer**: Typically used to reference breaking changes or issues closed.

### Commit Types

- **`feat:`**: Introduces a new feature.
  - Example: `feat(auth): add user authentication`
- **`fix:`**: Fixes a bug.
  - Example: `fix(api): resolve CORS error`
- **`perf:`**: Improves performance.
  - Example: `perf(api): optimize database queries`
- **`refactor:`**: Refactors code without changing its functionality.
  - Example: `refactor(ui): simplify header component`
- **`style:`**: Changes that don’t affect functionality (e.g., formatting, whitespace).
  - Example: `style(css): fix button alignment`
- **`test:`**: Adds or modifies tests.
  - Example: `test(auth): add test for login flow`
- **`docs:`**: Adds or updates documentation.
  - Example: `docs(readme): update setup instructions`
- **`chore:`**: Maintenance tasks like dependency updates or renaming files.
  - Example: `chore(deps): update npm dependencies`

### Special Notes

- **Breaking Changes**: If your commit introduces a breaking change, include `Breaking:` or `Breaking changes:` in the commit message's footer, describing the change.
  - Example:
    ```
    feat(auth): add OAuth support
    
    Breaking changes: OAuth support replaces the old API key system.
    ```

- **Short Hash**: For readability, short hashes (like `[abc123]`) are appended to the end of each commit in the changelog, but these may be commented out if there are file size limitations. If you wish to display them, ensure they're enabled in the template.

### Example Commit Messages

- **Feature Commit**:
```bash
feat(events): add ability to create recurring events
```

- **Bug Fix Commit**:
```bash
fix(calendar): resolve date picker display issue on mobile
```

- **Documentation Commit**:
```bash
docs(api): update API endpoint documentation
```

- **Refactor Commit**:
```bash
refactor(profile): simplify user profile logic
```

- **Performance Improvement Commit**:
```bash
perf(database): optimize query for user search
```

### How This Works in the Changelog

Your `auto-changelog` tool will categorize commits based on the types defined in your commit messages, like this:

- **Features** (`feat`): Will be grouped under a "Features" heading in the changelog.
- **Fixes** (`fix`): Will be grouped under a "Bug Fixes" heading.
- **Other types** like `refactor`, `style`, and `perf` will also get their own respective headings.

Each commit message will be stripped of its type and scope in the subject line, as the headings will categorize them already, and the commit message itself will be displayed.

### Running the Changelog

Before updating the changelog, make sure you have the `auto-changelog` dependency installed. If you haven't done so, run:

```bash
npm install
```
To update the changelog for version 2.0, use the following command:

```bash
npm run changelog:v2
```

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
