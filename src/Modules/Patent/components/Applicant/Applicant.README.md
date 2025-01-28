# Patent Application Management System

This repository contains the source code for the Patent Application Management System, developed using React, Mantine, and custom CSS. It manages patent application status, tracks progress, displays inventor details, and handles IP filing through a user-friendly interface.

## Project Overview

This project provides the following key features:

- **Patent Progress Tracking**: The system displays the progress of a patent application from submission to final approval.
- **Inventor Details**: It displays a table with inventor information, including names, email IDs, and phone numbers.
- **Application Status**: The system fetches and displays the current status of the patent application.
- **Patent Filing Form**: Users can input patent application details, inventor information, and commercialization details.
- **Attorney Details**: The application shows which attorney is assigned to a particular patent and their contact details.

### Code Structure Overview

The code is split into several components, which are responsible for different sections of the application. Here's a breakdown of the main components and how they work together:

---

## Components Description

### 1. **PatentProgressBar**

- **Purpose**: Displays the progress of a patent application.
- **Details**:
  - It uses a `progressMapping` object to map the current application status to a specific step in the progress bar.
  - The progress bar dynamically updates based on the current status, showing completed steps in green and upcoming steps in gray.
  - The `steps` array contains all possible statuses the application can go through, from "Patent Application Submission" to "Final Contract Completion."

- **Props**:
  - `currentStatus`: A string that indicates the current status of the patent application (e.g., "Attorney Assignment").

- **Usage**: This component is used inside the `PatentApplication` component to show a visual representation of the application's progress.

---

### 2. **InventorsTable**

- **Purpose**: Displays a list of inventors associated with the patent application.
- **Details**:
  - This component renders a table with columns for inventor's name, email, and phone number.
  - It loops over the `inventors` array and displays each inventor's information in a new row.
  
- **Props**:
  - `inventors`: An array of inventor objects, each containing `names`, `email`, and `phone`.

- **Usage**: This component is used inside the `PatentApplication` component to list the inventors' details.

---

### 3. **PatentApplication**

- **Purpose**: The main container component that displays detailed information about a patent application.
- **Details**:
  - It pulls the `currentStatus` of the application through a simulated API call (`fetchApplicationStatus`) and shows it to the user.
  - The component displays basic application details such as title, application number, token number, attorney name, and contact information.
  - The `InventorsTable` is embedded inside this component to show all inventors' details.
  - The `PatentProgressBar` is used to visually show the application's progress based on the current status.
  
- **Props**:
  - `title`: The title of the patent application.
  - `date`: The submission date of the application.
  - `applicationNumber`: The unique application number for the patent.
  - `tokenNumber`: A token identifier for the patent application.
  - `attorneyName`: Name of the attorney assigned to the patent application.
  - `phoneNumber`: The contact number of the attorney.
  - `email`: The email ID of the attorney.
  - `inventors`: An array of inventor details.

- **Usage**: This component is the core of the application and aggregates various pieces of information, including the patent status and inventor details.

---

### 4. **IPFilingForm** (Assumed)

- **Purpose**: Collects information from the user regarding their patent filing.
- **Details**: 
  - The form likely collects information such as patent title, inventor details, and commercialization details. 
  - (Note: Full implementation details for `IPFilingForm` were not included, but based on the context, this is the assumed purpose of the component.)
  
- **Usage**: The form is used to create new patent applications by capturing necessary data from users.

---

### 5. **SampleInventorsApp**

- **Purpose**: A sample implementation of the `PatentApplication` component with mock data for inventors.
- **Details**:
  - It provides sample inventor details and static data for patent applications.
  - This is typically used for testing or demonstration purposes.

- **Usage**: This is where sample data is passed to the `PatentApplication` component to display a mock-up of a real-world patent application. This helps visualize how the application would look with actual data.

---

## Supporting Libraries and Tools

### 1. **React**
- React is the main library used to build the user interface components.
- Components are structured using hooks like `useState` and `useEffect`.

### 2. **Mantine**
- Mantine is a UI component library used for building the interface. It provides components like `Loader`, `Table`, and `Text`, which are used for loading states, displaying tables, and showing text in various sections.

### 3. **Phosphor Icons**
- Phosphor icons are used in the UI, though they are not explicitly included in the code provided. This would likely be used for icons in buttons or other interactive elements.

### 4. **PropTypes**
- PropTypes are used to enforce type-checking on the props passed to each component, ensuring that the correct data type is provided.

### 5. **CSS Styling**
- Custom CSS files are used to style components like the `PatentProgressBar` and `IPFilingForm` to create a visually appealing layout.

---

## Code Flow

1. **Fetching Status**:
   - The `PatentApplication` component calls the `fetchApplicationStatus` function, which simulates fetching the status from a backend API.
   - Once the status is fetched, it updates the `currentStatus` state, triggering a re-render.

2. **Displaying Data**:
   - The `PatentApplication` component displays basic details of the patent, including the attorney's information and application status.
   - The `InventorsTable` and `PatentProgressBar` components are used to display additional details and a visual representation of the application's progress.

3. **Progress Bar**:
   - The `PatentProgressBar` component calculates the current step based on the fetched `currentStatus` and updates the progress bar to visually represent the progress.

4. **Sample Data**:
   - The `SampleInventorsApp` is used to simulate a working example of the `PatentApplication` component by passing mock data.

---

## Conclusion

This code is a part of a Patent Application Management System that allows users to track the status of their patent applications and view relevant information about the inventors and attorneys involved. The project demonstrates how to manage state, display dynamic content, and structure a React application using components that interact with each other.

## How to Run

To run this project locally, clone the repository, install the dependencies using `npm install`, and start the development server with `npm start`.

---

For any issues or questions, feel free to open an issue or submit a pull request!


 


