# Director Actor Frontend Development

## **Overview**
This project is centered on creating a dynamic, responsive frontend tailored specifically for the Director actor role. It includes state management with Redux, a custom navigation experience for Directors, and integration with APIs to display relevant Director-specific data and insights.

---

## **Features**

1. **Redux for Director State Management:**
   - Handles Director-specific state, including access to analytics and team overviews.
   - Ensures smooth state updates and consistent data flow.

2. **Director-Specific Navigation:**
   - Custom navigation bar designed for the Director role.
   - Includes links to sections like Dashboard, Reports, and Settings.

3. **Analytics Dashboard:**
   - Displays data-driven insights such as performance metrics and team summaries.
   - Fetches data from an API for real-time updates.

---

## **Technologies Used**

- **React**: Framework for building the user interface.
- **Mantine**: UI component library for responsive design and accessibility.
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
   - Create a `db.json` file with sample Director data.
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
│   │   └── DirectorNavbar.jsx
│   └── pages/
│       └── DirectorDashboard.jsx
├── layouts/
│   └── DirectorLayout.jsx
├── store/
│   ├── index.js
│   ├── directorSlice.js
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
This project showcases the ability to:
- Build a role-specific frontend tailored for Directors.
- Leverage Redux for state management and seamless data flow.
- Design dynamic navigation and analytics dashboards using Mantine components.

The result is a feature-rich, responsive, and user-friendly interface specifically designed for the Director role.

