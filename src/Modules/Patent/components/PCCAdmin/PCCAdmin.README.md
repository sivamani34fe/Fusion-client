1. StatusOfApplications.js
This component handles displaying a table of all patent applications and their current status. It allows the user to:

View a list of all submitted patent applications.
View details of an application by clicking on the "View" button.
Display each application with columns like Token Number, Patent Title, Submitted By, Designation, Department, Date-Time, and Status.
Features:

Displays a table with patent application details.
Allows navigation to a detailed view of a selected application.
The StatusOfApplicationData is used as mock data for patent applications.

2. PccaStatusView.js
This component displays detailed information about a selected patent application. It is displayed when a user clicks on the "View" button for an application.

Features:

Shows detailed information for a single patent application.
Includes fields like "Title of Application," "Inventor Name," "Contact Information," "Funding Source," etc.

3. ReviewAppComponent.js
This component allows users to review filled patent applications. The user can:

Review the intellectual property (IP) filing form.
The form contains several sections, such as Administrative Details, General Questions, IPR Ownership Questions, and Commercialization details.
It fetches filled data (mock data in this case) and displays it in input fields for review.
Features:

Displays pre-filled data using fetchFilledData.
Contains form sections such as the title of the application, inventor's details, and questions about the invention.
The user can interact with buttons like "Review," "Download Form," and "Forward To Director."

4. StatusOfApplicationData.js
This file contains mock data for the patent applications, which is used by the StatusOfApplications component. Each patent application contains:

Token Number: A unique identifier for the application.
Patent Title: The title of the patent.
Submitted By: The inventor who submitted the application.
Designation: The role of the inventor.
Department: The department under which the application is submitted.
Date-Time: The date and time of submission.
Status: The current status of the application (e.g., Under Review, Pending, Approved, etc.).
The data is displayed in the table format in StatusOfApplications.js.

5. CSS Styling
The project uses two CSS files to style the components:

StatusOfApplications.css: Styles the StatusOfApplications table, buttons, and layout.
ReviewComponent.css: Styles the patent review form, ensuring a clean and organized layout for each section.

Functional Flow
Viewing Patent Applications:

When the user visits the page, a table of applications is displayed.
Each application has a "View" button, which, when clicked, opens the detailed view of the selected application.
Reviewing an Application:

In the ReviewAppComponent, users can see all the details filled in for an application.
Users can review the data, and the form includes input fields for sections like the title, inventor name, and description.
Navigating Between Views:

From the list of applications, the user can navigate to the detailed view of a specific application by clicking "View."
In the detailed view, a back button allows the user to return to the applications list.

