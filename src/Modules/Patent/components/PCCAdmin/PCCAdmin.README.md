# PCC Admin Frontend Development

## **Overview**
This project involves building a dynamic, responsive frontend tailored specifically for the PCC Admin role. It integrates state management with Redux, provides custom navigation for PCC Admins, and incorporates APIs to manage and display administrative data effectively.

---

## **Features**

1. **Redux for PCC Admin State Management:**
   - Manages state related to administrative tasks, user management, and system configurations.
   - Ensures smooth and predictable state updates.

2. **PCC Admin-Specific Navigation:**
   - Custom navigation bar designed for PCC Admin roles.
   - Includes links to sections such as Dashboard, User Management, and Settings.

3. **Administrative Dashboard:**
   - Displays key data such as user statistics, system logs, and performance metrics.
   - Integrates with APIs for real-time administrative data.

---

## **Technologies Used**

- **React**: Framework for building user interfaces.
- **Mantine**: UI component library for responsive and accessible design.
- **Redux Toolkit**: Efficiently manages the application’s state.
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
   - Create a `db.json` file with sample administrative data.
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
│   │   └── PCCAdminNavbar.jsx
│   └── pages/
│       └── PCCAdminDashboard.jsx
├── layouts/
│   └── PCCAdminLayout.jsx
├── store/
│   ├── index.js
│   ├── adminSlice.js
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
- Build a role-specific frontend tailored for PCC Admins.
- Use Redux for efficient state management and data handling.
- Design user-friendly navigation and dashboards using Mantine components.

The result is a robust, scalable, and responsive interface designed for the PCC Admin role.

