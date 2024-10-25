# User Log-In/User Sign-Up

## Overview
The User Log-In/User Sign-Up feature allows both students and organizations to create accounts and log in to the system. The sign-up process includes validation for password strength, and users are authenticated using a JWT token-based system.

## Key Functions
- Two sign-up buttons: one for student accounts and another for organization accounts.
- Password validation that requires at least 8 characters with a mix of letters and symbols.
- A toggle to show/hide password during the sign-up process.
- JWT token-based authentication for logging in.

## Usage
- **Create Student Account**:
  - Users can sign up by providing their Student ID, email address, and password.
  - Password confirmation is required, and users can toggle the visibility of their password using a show password button.
  
- **Create Organization Account**:
  - Organizations can sign up by entering the organization’s name, email address, and password.
  - Similar to the student sign-up, password confirmation is required with a show password toggle button.
  
- **Login**:
  - Once a user has created an account, they can log in using their email and password.
  - JWT token is generated upon successful login, and authentication is currently handled through the Command Prompt (until full backend integration).

- **Navigation**:
  - A link is provided on the sign-up page to redirect users to the login page if they already have an account.

## Examples (Optional)
- A student can create an account using their student ID, validate their password, and toggle the visibility of their password during input.
- After successful sign-up, the user can log in via the login page and receive a JWT token for authentication.

## Additional Notes (Optional)
The **User** class has been created with functions, setters, and getters. The current implementation of the authentication system uses JWT tokens, and while full backend integration is still in progress, login can be performed via Command Prompt with predefined users in the code.

---

# Component Reference

## How to Add to This Reference
When a new component is created, add a new line at the end following this format. Include the component's name with a link to its documentation and a brief description.

### Existing Components:

#### <SignUpPage/>
Provides the initial sign-up interface where users can choose between creating a student or an organization account. It includes two main buttons: "Create student account" and "Create organization account." Additionally, there is a link to redirect users to the login page if they already have an account.

#### <SignUpOrganization/>
Provides the interface for organizations to create an account. Includes fields for organization name, email, and password, with validation for password strength and confirmation. A password visibility toggle and error handling for mismatched passwords are also provided.


#### <SignUpStudent/>
Provides the interface for students to create an account. It includes fields for the student ID, email, and password, with real-time validation for password strength and confirmation. A password visibility toggle and error handling for mismatched passwords are also available.
---

## Contributors
- **AlejandroClaudio**
- **estefania-2817**
- **WilsonMorales8**
- **vivianaramos6**
- **Ingrid1089**
- **MIguelGibo**
- **arianarodz21**
