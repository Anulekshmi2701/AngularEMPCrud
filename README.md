
Employee CRUD Application
This is a web-based CRUD (Create, Read, Update, Delete) application for managing employee data. It is built using Angular with Angular Material for the frontend and a JSON server for the backend.

Features
Add a new employee with details like name, email, date of birth, gender, education, company, experience, and salary package.
View a list of all employees in a dynamic table with sorting, filtering, and pagination.
Edit employee details.
Delete employees.
Responsive design with Angular Material components.
Snackbar notifications for user actions.
Tech Stack
Frontend: Angular, Angular Material
Backend: JSON Server
Styles: SCSS
Package Manager: npm
Getting Started
Prerequisites
Ensure you have the following installed on your system:

Node.js (v14 or above)
Angular CLI
npm (comes with Node.js)
Installation Steps
Clone the repository

bash
Copy code
git clone <repository-url>
cd employee-crud
Install dependencies

bash
Copy code
npm install
Set up JSON Server

Create a file named db.json in the root directory and add the following sample data:
json
Copy code
{
  "employees": [
    {
      "id": 1,
      "firstName": "John",
      "lastName": "Doe",
      "email": "john.doe@example.com",
      "dob": "1990-01-01",
      "gender": "Male",
      "education": "MBA",
      "company": "TechCorp",
      "experience": 5,
      "package": 8.5
    }
  ]
}
Start the JSON Server:
bash
Copy code
npx json-server --watch db.json
Run the application

Start the Angular development server:
bash
Copy code
ng serve
Open the application in your browser at http://localhost:4200.
Folder Structure
graphql
Copy code
src
├── app
│   ├── core           # Shared core services (e.g., snackbars)
│   ├── emp-add-edit   # Employee Add/Edit Dialog component
│   ├── services       # Service for API calls
│   ├── app.component  # Root component
│   └── app.module     # App-wide module configuration
├── assets             # Static assets
├── environments       # Environment configurations
├── styles.scss        # Global styles
└── index.html         # Main entry point
Usage
Add Employee
Click the "ADD EMPLOYEE" button on the top toolbar.
Fill in the form and click "Save".
Edit Employee
Click the pencil (edit) icon in the Action column for the employee you want to edit.
Update the details and click "Save".
Delete Employee
Click the trash (delete) icon in the Action column for the employee you want to remove.
Confirm the deletion.