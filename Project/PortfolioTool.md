# Portfolio Tool

***
## Table of Contents
1. [Project Overview](#1-project-overview)
   - [Purpose](#purpose)
   - [Role](#role)
2. [Technical Details](#2-technical-details)
   - [Architecture Diagrams](#architecture-diagrams)
   - [Technology Stack](#technology-stack)
3. [Development Process](#3-development-process)
   - [Methodology](#methodology)
   - [Version Control](#version-control)
4. [Key Features and Functionality](#4-key-features-and-functionality)
   - [Features Implemented](#features-implemented)
   - [Screenshots](#screenshots)
5. [Challenges and Solutions](#5-challenges-and-solutions)
   - [Problems Encountered](#problems-encountered)
   - [Solutions Implemented](#solutions-implemented)
6. [Project Outcomes and Impact](#6-project-outcomes-and-impact)
   - [Results](#results)
   - [Impact](#impact)
7. [Lessons Learned](#7-lessons-learned)
   - [Technical Skills](#technical-skills)
   - [Project Management Insights](#project-management-insights)
   - [Future Improvements](#future-improvements)
8. [Additional Contributions](#8-additional-contributions)
   - [Beyond the Project](#beyond-the-project)
   - [Networking and Professional Growth](#networking-and-professional-growth)

***
## 1. Project Overview

### Purpose

The primary purpose of this project is to develop the "Portfolio Tool" during my internship at HighTechXL. As a software engineering student, my goal is to automate and standardize the collection of quarterly updates from startups, which has traditionally been handled manually through emails and phone calls. This manual process often resulted in inconsistent and sometimes incomplete data, complicating the task of maintaining an up-to-date and clear view of each startup's progress within the HighTechXL ecosystem. Such inconsistencies also hindered HighTechXL's ability to provide necessary data to potential investors.

The Portfolio Tool is designed to replace these outdated manual communications with an automated, standardized system that ensures data consistency and quality. Additionally, the tool addresses the crucial need for effective information storage, enabling HighTechXL to maintain a robust database of venture updates that can be easily accessed and managed. This enhancement will facilitate better support and resources allocation within the HighTechXL ecosystem.

### Role
As the main developer of the Portfolio Tool, I was responsible for all aspects of its development, from design and architecture to database creation and integration. My tasks included:

  Design and Architecture: I handled the comprehensive design and architectural setup, ensuring the tool was functional and efficient.
  Database Creation: I developed the database that supports the tool, focusing on scalability and ease of data management.
  Guidance and Collaboration: I worked closely with the current portfolio manager to understand the requirements and nuances of portfolio data collection. This collaboration was crucial in shaping the tool’s functionality.
  Software Development: Alongside the software team, which consisted of my supervisor, I integrated the new tool with the existing Venture Journey Tool to enhance its capabilities and ensure seamless operation.

This role provided me with significant hands-on experience in managing a full-cycle development project, honing my technical skills and understanding of effective team collaboration.

***
## 2. Technical Details
### Architecture Diagrams
![Architecture](/path/to/architecture.png)

### Technology Stack

The development of the Portfolio Tool involved using a blend of technologies that were already familiar within HighTechXL, alongside some new adaptations to meet the specific needs of the project.

- **Frontend**: The frontend of the application was developed using AngularJS and TypeScript, a choice driven by its existing use within HighTechXL. This provided a consistent framework that aligns with other projects and applications within the organization. Material Components were integrated for styling, enhancing the user interface with a modern and responsive design. Additionally, TailwindCSS was incorporated early in the development to assist with the styling of the application.

- **Backend**: The backend functionality was built using a C# API with Entity Framework Core (EF Core) for managing the database interactions. This setup enabled a robust "code first" approach, allowing for an agile development process where changes in the database schema could be managed directly through the codebase.

- **Database**: A standard SQL database was chosen for its simplicity and ease of use, particularly given the requirements for compatibility with my personal development setup. SQL databases are well-known for their reliability and broad support, making them an ideal choice for the data management needs of this tool.

Further technical and strategic justifications for choosing this specific technology stack and the design of the web application over alternatives such as a form builder are detailed in my research document ["How can HighTechXL implement an information management system that efficiently stores, and easily retrieves startup data to optimize the support processes?"](https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/research/How%20can%20HighTechXL%20implement%20an%20information%20management%20system%20that%20efficiently%20stores%2C%20and%20easily%20retrieves%20startup%20data%20to%20optimize%20the%20support%20processes%3F.md). This research gives more insight on some of the technological decisions made.



***
## 3. Development Process
### Methodology
We adopted an Agile Scrum methodology with...

### Version Control
We used Git for version control with the following branching strategy...

***
## 4. Key Features and Functionality
### Features Implemented

### Screenshots

***
## 5. Challenges and Solutions

### Problems Encountered

1. **Component Library Limitations**: My initial lack of experience with HTML, CSS, and TailwindCSS made it challenging to quickly develop effective UI components. Consequently, I first incorporated Preline to simplify UI development. As I gained more experience, I transitioned to using Flowbite's styling for better control over the appearance, though without adopting its full plugin system.

2. **Complex Component Requirements**: As the project's requirements evolved, especially the need to integrate complex components like steppers, the purely stylistic solutions offered by Flowbite proved insufficient. This necessitated a further switch to Material components, which offered comprehensive functionality and seamless integration with Angular and reactive forms.

3. **CORS Errors**: CORS errors initially complicated the connection between the frontend and the API, which hampered testing and integration.

4. **Database Migration Issues**: I faced difficulties with the database-first approach during updates, as models and context files did not align with evolving project requirements.

5. **Database Versioning**: Manual versioning of the database was complex and error-prone, especially for tracking changes over time in the venture data.

### Solutions Implemented

1. **Component Library Transitions**: To accommodate my initial inexperience with front-end styling and subsequent needs for more advanced functionality, we transitioned from Preline to Flowbite's styling, and ultimately to Material components. This progression not only enhanced the UI/UX but also supported the integration of more complex functional components required by the project.

2. **CORS Configuration**: To address the CORS issues, additional configurations were added to the API, setting up proper CORS policies to facilitate secure resource sharing between the frontend and backend.

3. **Shift to Code-First Approach**: The database-first approach was replaced by a code-first approach due to its flexibility in handling schema changes. This shift allowed for automatic migrations and easier management of the evolving database schema.

4. **Temporal Tables for Versioning**: We implemented temporal tables in SQL Server to automate database versioning. This feature automatically tracks changes, simplifying the management of historical data and ensuring data integrity without manual efforts.

These changes and improvements not only solved the initial problems but also enhanced the overall system's functionality, making the Portfolio Tool more robust and efficient.



***
## 6. Project Outcomes and Impact
### Results
The project successfully...

### Impact
This resulted in...

***
## 7. Lessons Learned
### Technical Skills
I enhanced my skills in...

### Project Management Insights
One key insight from managing this project was...

### Future Improvements
In future projects, we could...

***
## 8. Additional Contributions
### Beyond the Project
During the project, I also participated in...

### Networking and Professional Growth
This project allowed me to...
