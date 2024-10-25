# Profile Event Tuner

## Overview
The Profile Event Tuner feature allows users to customize their profile by selecting their faculty, major, and student associations. This personalized information helps tailor event recommendations and provides a user-centric experience on the platform. Users must select at least one faculty, major, and a minimum number of associations to proceed.

## Key Functions
- Selection of faculty, major, and student associations.
- Dynamic display of majors based on the faculty selected.
- Option to select universal associations available to all students.
- Custom selection of associations based on the student’s major.
- Validation to ensure the user makes the required selections before proceeding.

## Usage
- **Faculty Selection**: Users can choose from four faculty buttons: Ingeniería, Administración de Empresas, Ciencias Agrícolas, and Artes y Ciencias. Once a faculty is selected, the major options will dynamically appear.
- **Major Selection**: After selecting a faculty, users can pick from a list of majors specific to that faculty.
- **Association Selection**: Users can choose from two types of associations:
  - **Universal Associations**: These are available to all students, regardless of faculty or major.
  - **Major-Specific Associations**: These are tailored to the user’s selected major.
- **Validations**: Users must select at least one faculty, one major, and a minimum number of associations before they can continue. This ensures that each profile is sufficiently personalized.

## Examples (Optional)
- A user studying in the Facultad de Ingeniería can select from majors such as Civil Engineering, Mechanical Engineering, etc., and then choose relevant associations based on their major.
- A user who selects Administración de Empresas can choose majors like Accounting, Marketing, and specific associations tied to those fields.

## Additional Notes (Optional)
The organization of associations is divided by faculty and major, ensuring users only see the relevant associations for their area of study. Universal associations are also presented for broader involvement across all faculties.

---

# Component Reference

## How to Add to This Reference
When a new component is created, add a new line at the end following this format. Include the component's name with a link to its documentation and a brief description.

### Existing Components:

#### <FacultySelectionComponent/>
Allows users to choose from four faculties, dynamically showing majors based on the selected faculty.

#### <MajorSelectionComponent/>
Displays a list of majors based on the chosen faculty and enables users to select their field of study.

#### <AssociationSelectionComponent/>
Allows users to choose from universal associations or associations specific to their major.

---

## Contributors
- **Edzel Ortiz**
- **Kiara Perez**
- **Kevin Lopez**
- **Gabriel Gonzales**
- **Angel Perez**
