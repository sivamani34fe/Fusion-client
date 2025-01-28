# Applicant Actor Frontend Development

## **Overview**
This project focuses on creating a dynamic, responsive frontend tailored specifically for the Applicant actor role. It integrates state management using Redux, custom navigation for Applicants, and API integration for displaying relevant Applicant-specific data.

---

## **Features**

1. **Redux for Applicant State Management:**
   - Handles Applicant-related state, including profile details and application statuses.
   - Ensures seamless state updates and data flow.

2. **Applicant-Specific Navigation:**
   - Custom navigation bar designed for the Applicant role.
   - Includes links to sections such as Dashboard, Applications, and Profile.

3. **Dashboard with Real-Time Updates:**
   - Displays Applicant-specific data such as application status, deadlines, and updates.
   - Fetches data from an API for real-time information.

---

## **Technologies Used**

- **React**: Framework for building the user interface.
- **Mantine**: UI component library for creating a responsive design.
- **Redux Toolkit**: Manages the application's state effectively.
- **json-server** (optional): Used as a mock API for local testing.

---

## **Setup and Installation**

1. **Clone the Repository:**
   ```bash
   git clone <repository-url>
   cd <project-folder>
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

3. **Run the Development Server:**
   ```bash
   npm run dev
   ```

4. **Mock API Setup (Optional):**
   - Install `json-server` globally:
     ```bash
     npm install -g json-server
     ```
   - Create a `db.json` file with sample Applicant data.
   - Start the mock API server:
     ```bash
     json-server --watch db.json --port 3001
     ```

---

## **Folder Structure**

```
src/
├── components/
│   ├── common/
│   │   └── ApplicantNavbar.jsx
│   └── pages/
│       └── ApplicantDashboard.jsx
├── layouts/
│   └── ApplicantLayout.jsx
├── store/
│   ├── index.js
│   ├── applicantSlice.js
│   └── dataSlice.js
└── main.jsx
```

---

## **How to Run**

1. Clone the repository.
2. Install dependencies with `npm install`.
3. Start the development server with `npm run dev`.
4. (Optional) Start a mock API server with `json-server` for testing.

---

## **Conclusion**
This project highlights the ability to:
- Implement a role-specific frontend tailored for Applicants.
- Use Redux for efficient state management.
- Build dynamic navigation and dashboards using Mantine components.

The result is a robust, scalable, and user-friendly interface for the Applicant role.

