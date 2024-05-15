# Portfolio Tool

***

## Table of Contents
- [Project Overview](#project-overview)  
- [Technical Details](#technical-details)
- [Project Management](#project-management)
- [Developement process](#development-process)
- [Key Features and Functionality](#key-features-and-functionality)
- [Challenges and Solutions](#challenges-and-solutions)
- [Project Outcomes and Impact](#project-outcomes-and-impact)
- [Lessons Learned](#lessons-learned)

<small><i><a href="https://github.com/BramVerkuijlen/Portfolio-S5-Internship"><- Back to the portfolio</a></i></small>

***
## Project Overview


### Introduction
The Portfolio Tool is designed to streamline the process of data collection from new and existing ventures. As a software engineering intern, my project aimed to automate and standardize the collection of quarterly updates from startups, which had traditionally been handled manually through emails and phone calls. This manual process often resulted in inconsistent and sometimes incomplete data, complicating the task of maintaining an up-to-date and clear view of each startup's progress within the HighTechXL ecosystem. 

By replacing these outdated manual methods with an automated, standardized system, the Portfolio Tool ensures data consistency and quality. Additionally, this initiative significantly enhances information storage capabilities, allowing for robust data management and easier access—key factors in providing better support and resource allocation within HighTechXL.

### Purpose
The primary purpose of this project was to develop the Portfolio Tool to replace inefficient and inconsistent data collection practices. This allows for a more streamlined, error-free process, facilitating the maintenance of a clear, comprehensive database of venture updates.

### Technical Implementation

Central to the Portfolio Tool is an online form designed specifically for ventures to easily provide HighTechXL with data about their businesses. Once this data is submitted, it is automatically stored in a well-structured database.

After the data is securely stored, the Portfolio team uses PowerBI to access and analyze the venture data. This helps them to create detailed, visually appealing portfolios that can be presented to potential investors.

### Role
As the main developer of the Portfolio Tool, I was responsible for all aspects of its development, from design and architecture to database creation and integration. My tasks included:

  Design and Architecture: I handled the comprehensive design and architectural setup, ensuring the tool was functional and efficient.
  Database Creation: I developed the database that supports the tool, focusing on scalability and ease of data management.
  Guidance and Collaboration: I worked closely with the current portfolio manager to understand the requirements and nuances of portfolio data collection. This collaboration was crucial in shaping the tool’s functionality.
  Software Development: Alongside the software team, which consisted of my supervisor, I integrated the new tool with the existing Venture Journey Tool to enhance its capabilities and ensure seamless operation.

This role provided me with significant hands-on experience in managing a full-cycle development project, honing my technical skills and understanding of effective team collaboration.

***
## Technical Details

### Architecture Diagrams
**NULL**

### Technology Stack
The development of the Portfolio Tool involved using a blend of technologies that were already familiar within HighTechXL, alongside some new adaptations to meet the specific needs of the project.

- **Frontend**: The frontend of the application was developed using AngularJS and TypeScript, a choice driven by its existing use within HighTechXL. This provided a consistent framework that aligns with other projects and applications within the organization. Material Components were integrated for styling, enhancing the user interface with a modern and responsive design. Additionally, TailwindCSS was incorporated early in the development to assist with the styling of the application.

- **Backend**: The backend functionality was built using a C# API with Entity Framework Core (EF Core) for managing the database interactions. This setup enabled a robust "code first" approach, allowing for an agile development process where changes in the database schema could be managed directly through the codebase.

- **Database**: A standard SQL database was chosen for its simplicity and ease of use, particularly given the requirements for compatibility with my personal development setup. SQL databases are well-known for their reliability and broad support, making them an ideal choice for the data management needs of this tool.

Further technical and strategic justifications for choosing this specific technology stack and the design of the web application over alternatives such as a form builder are detailed in my research document ["How can HighTechXL implement an information management system that efficiently stores, and easily retrieves startup data to optimize the support processes?"](https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/research/How%20can%20HighTechXL%20implement%20an%20information%20management%20system%20that%20efficiently%20stores%2C%20and%20easily%20retrieves%20startup%20data%20to%20optimize%20the%20support%20processes%3F.md). This research gives more insight on some of the technological decisions made.

***
## Project Management
### Methodology 
Initially, I used a Agile Scrum methodology for managing the portfolio project, suing a structures I had used in a previous project ([portfolio S3 agile method](https://github.com/BramVerkuijlen/Portfolio-S3/blob/main/ProofLearningOutcomes/Agile.md)).

However, as the project evolved, it became clear that the rapidly changing requirements and the fact that I was working solo made the structured Scrum approach less practical. The frequent changes and immediate decision-making did not align well with the structured sprint planning. Therefore, I decided to step away from using a strict Agile methodology.

Transitioning to a more fluid approach allowed for quicker responses to changing needs and more direct incorporation of new ideas and solutions as they arose. Despite moving away from formal Agile practices, I maintained a structured update and feedback rhythm by attending HighTechXL’s weekly scrum meetings, which kept everyone up-to-date. Additionally, I held weekly meetings with the portfolio manager to discuss specific project details and had frequent discussions with my company mentor.

### Version Control
In managing the version control for my project, I utilized Git with a straightforward branching strategy that was well-suited to solo development. The master branch functioned as the main build branch, reserved exclusively for stable versions of the software. This ensured that the master branch was always reliable and production-ready.

For development and testing of new features or updates, I utilized separate branches. This approach allowed me to freely experiment and refine functionalities without impacting the stability of the master branch. Each feature was developed in its own branch and only merged into master once it had been fully tested and confirmed stable. This branching strategy effectively maintained the integrity of the main project while allowing for continuous development and improvement.

***
## Developement process

**NULL**

## Key Features and Functionality

### Loading Previous Data

A critical feature of our application is its ability to load previous data for user convenience and efficiency. When users return to the application, they don't have to start from scratch; instead, the system automatically checks the database for existing data associated with the user's venture. If previous data is found, it pre-populates the forms with this information.

This functionality allows ventures to easily review and update their information as needed without re-entering all data, significantly reducing the time and effort involved in maintaining up-to-date records. Once the form is completed and submitted, the updated information is stored in the database, ensuring that the most recent data is always available.

### Tech1 and Tech2 Selection
In the application form, users encounter two fields labeled as Tech1 and Tech2. These labels, while perhaps initially unclear to some, are terms used within HighTechXL to denote 'Technology Tier 1' and 'Technology Tier 2,' respectively. Technology Tier 2 is essentially a subcategory of Tier 1.

The Tech2 field is initially disabled. It becomes active only after a selection is made in Tech1. Upon choosing a Tech1 category, the corresponding Tech2 options are dynamically loaded and enabled. This ensures that the choices in Tech2 are relevant to the broader category selected in Tech1, preventing mismatched or irrelevant data entries. This functionality helps the user through a logical sequence of choices, improving the overall ease and accuracy of data entry.

<div style="display: flex; justify-content: space-between; align-items: center;">
  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Tech1%2C%20Tech2%20disabled.png" alt="Tech1 Field Enabled, Tech2 Disabled">
    <p><em>Tech1 field enabled and Tech2 field disabled, indicating the initial state before any Tech1 selection.</em></p>
  </div>
  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Tech1%20Tech2%20active.png" alt="Tech1 and Tech2 Fields Active">
    <p><em>Tech1 and Tech2 fields active, showing selectable options in both fields after Tech1 is selected.</em></p>
  </div>
</div>


### Features Implemented
**NULL**

***
## Challenges and Solutions

### Component Library Limitations
Initially, my unfamiliarity with CSS, HTML, and TailwindCSS led me to adopt Preline's full system to make creating comoponents easier. Unfortionately, I encountered compatibility issues with Angular, some of the components that preline provided wouldnt work with angulars reactive forms. Because of this I switched to Flowbite, where I only used their styling without installing any plugins, allowing me to easilly style my components without the risk of the plugin not working with angular.


<div style="display: flex; justify-content: space-between; align-items: center;">
  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/WebApp%20I1.1.png" alt="First design using Preline" height="450">
    <p><em>First design iteration using <a href="https://preline.co/" target="_blank">Preline</a>.</em></p>
  </div>
  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/WebApp%20I2%20HTXL.png" alt="Second iteration using Flowbite" height="450">
    <p><em>Second iteration using <a href="https://flowbite.com/" target="_blank">Flowbite</a>.</em></p>
  </div>
</div>



As the project grew to include more sophisticated components like a stepper or multi selects, I needed a more robust solution that was guaranteed to work seamlessly with Angular. This led to my decision to adopt Angular Material. Angular Material not only offered a sleek and straightforward design but also provided the certainty of complete compatibility with Angular. This ensured that I could implement the more complex components needed for the project.

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/POC%20Company%20Details.png" alt="Third iteration using Material Angular">
  <p><em>Third iteration using <a href="https://material.angular.io/" target="_blank">Material Angular</a>.</em></p>
</div>

### Linking portfolios
After completing my initial proof of concept, I started to flesh out the functionality of what was initially called a "venture" but has since been renamed "portfolio." One of the earliest and most challenging issues I faced was linking these portfolios to specific start-ups.

In response, my supervisor, Jordy, and I initially considered integrating the portfolio tool with HighTechXL's existing "venture journey" system. This system already had a working login system created by Jordy, which seemed like a practical solution. However, integrating these systems felt problematic as we aimed to keep the two applications as separate as possible to avoid any operational conflicts.

This encouraged me to lokk for an alternative solution. I decided to rename the original venture table to "portfolio" and created a new venture table equipped with an ID. This new structure mirrored what HighTechXL employed in their venture journey, effectively resembling a user table found in standard applications. This change finally provided a coherent way to link a portfolio to specific venture, resolving the initial functional issues and enhancing the overall system architecture.

### Database Versioning
Because HightechXL was using a excel file as their main way to store data tehy lacked any kind of versioning. While versioning wasn't initially a requirement, I realized its potential benefits in tracking a venture's progress and aiding in securing investors. One of the solutions I considered was the use of temporal tables. This SQL Server feature seemed promising due to its seamless integration with my database structure and compatibility with PowerBI, which would facilitate historical data management and ensure data integrity.

<img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/DBO%20post%20POC1%20V2.png?raw=true" alt="Before Database Design">

However, during the development of my second proof of concept, I introduced an extra "venture" table to improve the system's architecture (as described in the previous alinea on "Linking Portfolios"). This modification complicated the use of temporal tables because they are most effective when updating existing data, not when linking new data entries.

To adapt, I revised the database structure to not use temporal tables. Instead, I linked multiple portfolios to a single venture and added a 'date submitted' column. This approach effectively allowed for tracking changes over time without the complexity of temporal tables, maintaining the ability to observe historical changes across different data submissions, thus mimicking the versioning effect I aimed to achieve. This change also came with the benifit that HightechXL could now also change certain portfolio information without it effecting the temporal history table.

<img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Screenshot%20Database%20after%20venture%20table%20split%202024-05-08%20144702.png?raw=true" alt="After Database Design">

### Login
Implementing the second proof of concept build, which was designed to collect and store data, presented several challenges. Initially, the application setup was too simplistic, using only an ID as an identifier. This method was inherently insecure as the ID could easily be guessed by potential attackers, potentially exposing sensitive data. Given the complexity and time requirements to develop a full-fledged login system, I initially opted not to host the application online. Instead, I chose to run it locally on my laptop via localhost, recognizing that this was not an ideal solution.

During discussions with my school mentor, Thijs, we looked at several potential solutions to enhance security without committing extensive resources to develop a complete login system. Among the options considered were implementing Google's OAuth for authentication, creating a simplified custom login system, or enhancing server security to protect the application.

After some consideration, I decided to develop a portion of the login system. I chose to manually create login credentials for each venture. By assigning secure usernames and passwords, I could ensure that only I had the authority to distribute access credentials directly to the ventures. Furthermore, I used JWT tokens to secure my API and altered my API calls to check if the user was allowed to interact with the venture.

### Updating to .NET 8

Initially, my API was built using .NET 6, which seemed to be version Visual Studio defaulted to when creating the project. However, while exploring authentication options, a suggestion from the C# Discord community led me to consider upgrading to .NET 8. This newer version had more features, including a new identity system. Although I ultimately decided against using this identity system, opting for a JWT solution, which ended up being compatible with .NET 6.

Transitioning to .NET 8, however, was not straightforward. After updating the API's version, I encountered several significant issues. The API functionality broke, and Rider, the IDE I had switched to, was behaving unusual.

To resolve these issues, I undertook the following steps:
1. **SDK Installation**: I installed the latest .NET 8 SDK, ensuring that the development environment was fully updated.
2. **Package Updates**: All dependent packages were updated to their latest versions compatible with .NET 8.

After this easy fix, the system stabilized, and the API worked again. Although the errors did scare me a bit and it took a few hours to resolve.

***
## Project Outcomes and Impact
### Results
**NULL**

### Impact
**NULL**

***
## Lessons Learned

### Technical Skills
**NULL**

<small><i><a href="https://github.com/BramVerkuijlen/Portfolio-S5-Internship"><- Back to the portfolio</a></i></small>
