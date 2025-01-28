Overview
The Patent Application Management System is a React-based web application designed to manage and review patent applications. It allows users to view and interact with applications at different stages: submitted, pending review, and reviewed. Additionally, it provides a detailed view of patent application statuses and inventor details. The system is designed for patent reviewers, administrators, and other relevant users in the patent management process.





Key Features:
Submitted Applications: Displays patent applications that have been forwarded by the PCC Admin.
Pending Reviews: Shows a list of applications awaiting review by the patent committee.
Reviewed Applications: Displays applications that have already been reviewed, with details such as attorney names and application numbers.
Patent Application Status: Allows for a deep dive into individual applications with detailed information on applicants, assigned attorneys, and inventors.
Responsive Design: Optimized for both desktop and mobile devices for seamless viewing across all screen sizes.
Interactive UI: Includes interactive cards and modals to view detailed application information with ease.
Technologies Used
React: JavaScript library used to build the user interface.
Mantine: A modern UI component library used for building elements such as cards, grids, and buttons.
Phosphor Icons: For icons like "View Details" and "Info" buttons.
PropTypes: Used for validating component props to ensure type safety and better development experience.
CSS: For custom styles and responsive design.



Components Overview
1. SubmittedApplications
Description: Displays applications forwarded by the PCC Admin. Each application card shows key details such as the title, date, application number, and assigned attorney.

Main Features:
View details for each application.
Responsive layout for both desktop and mobile views.


2. PendingReviews
Description: Displays patent applications that are waiting for review. This section lists the token number, title, date, application number, and assigned attorney for each application.
Main Features:
Displays applications in a responsive grid layout.
Interactive “View Details” button that opens a modal or navigates to a detailed view.



3. ReviewedApplications
Description: Shows patent applications that have already been reviewed. Each application card provides detailed information like the application’s title, assigned attorney, and a link to the submitted form.
Main Features:
Interactive buttons for viewing additional details.
Cards display detailed information regarding the reviewed application.


4. PatentApplication
Description: Displays detailed information about a selected patent application. This includes the title, application date, applicant details, assigned attorney, and the list of inventors with their contact information.
Main Features:
A table displaying inventor names, emails, and phone numbers.
Editable sections for different application details.

Data Structure
The application makes use of a mock data structure for each section. Here’s an overview of the data structure used in the components:

PendingReviewsData.js
Contains data for patent applications that are pending review, including:

tokenNumber: A unique identifier for the application.
title: The title of the patent application.
date: The date the application is due for review.
time: The time for the review.
applicationNumber: Unique identifier for the application.
attorney: Name of the attorney assigned to the application.
borderColor: Dynamic color for the left border of each card.
ReviewedApplicationsData.js
Contains data for applications that have been reviewed. Similar to the pending reviews data, it includes:

title: Title of the application.
applicant: Name of the applicant.
applicationNumber: Unique identifier for the application.
attorney: Name of the assigned attorney.
borderColor: Border color for styling the card.
SubmittedApplicationsData.js
Contains data for applications that have been forwarded by the PCC Admin. Similar to the other datasets, it includes:

tokenNumber: Unique identifier for the application.
title: The title of the application.
date: The submission date.
applicationNumber: The application number.
attorney: Name of the attorney handling the application.
Screenshots
Submitted Applications View

Pending Reviews View

Reviewed Applications View

Patent Application Status View

