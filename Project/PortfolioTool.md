# The Portfolio Tool


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

- **Backend**: The backend functionality was built using a C# API with Entity Framework Core (EF Core) for managing the database interactions. EF Core with C# was chosen because it was already in use by HighTechXL and was the framework with which my internship mentor had the most experience.

- **Database**: Transitioning from the current Excel-based system to a SQL database is crucial for HighTechXL to manage startup data more efficiently. SQL databases provide the necessary infrastructure for scalability, data integrity, and reliability, essential as HighTechXL continues to grow, and they integrate seamlessly with PowerBI for robust data analysis and reporting. Additionally, a standard SQL database was chosen for its simplicity, ease of use, and compatibility with my personal development setup, making it an ideal solution for the data management needs of this tool.

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
## Development process

### Introduction to Angular and Project Setup
The first week, when I was supposed to start at the company, my supervisor was on vacation and unable to introduce me to the company and the project. Therefore, we decided that I would work from home during this week to get familiar with Angular and set up my Git and Jira board for the project. 

I used this first week to create a small CRUD application in Angular that used JSON server as a mock database. Additionally, I took the time to become familiar with Tailwind, as HighTechXL also used Tailwind. Having previously used .NET and Vue for front-end development, adapting to Angular was relatively simple due to its many similarities with Vue. However, I initially struggled with Angular's dependency injection and observables.

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Learning%20Angular%20using%20Json%20Server.png" alt="First week CRUD application using Angular and Tailwind" style="max-width: 60%;">
  <p><em>First week CRUD application using Angular and Tailwind</em></p>
</div>

### GitHub Organization Setup
I chose to set up a GitHub organization because it allows for easy management of repositories. In this organization I also set up my front-and back end repositories.

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/HTXL%20internship%20organization.png" alt="Screenshot of GitHub organization" style="max-width: 60%;">
  <p><em>Screenshot of GitHub organization</em></p>
</div>

### Jira Task Board Establishment
Initially, I used an Agile Scrum methodology with user stories and sub-tasks, as I had done in a previous project [(Proof of Learning Outcomes)](https://github.com/BramVerkuijlen/Portfolio-S3/blob/main/ProofLearningOutcomes/Agile.md). HighTechXL had no specific working method requirements, allowing me flexibility.

To track progress, I established a Task Board in Jira, creating an initial set of tasks and example templates for consistency.

However, as the project evolved, rapidly changing requirements and solo work made structured Scrum impractical. I shifted to a more flexible approach, enabling swift responses to changes and quick decision-making, which was crucial for the project's success.

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Jira%20board.png" alt="Screenshot of Jira task board" style="max-width: 60%;">
  <p><em>Screenshot of Jira task board</em></p>
</div>


### Information gathering and wireframe

The first week at the company, I focused on gathering information on what needs to be included in the portfolio tool. I achieved this by talking with the portfolio manager, examining the existing XL file, and reviewing documents from previous attempts at a portfolio tool.

Using the information I gathered, I started creating wireframes for the front-end of my application.

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Wireframe1%20HTXL.png" alt="Wireframe 1: Initial design for the portfolio tool" style="max-width: 60%;">
  <p><em>Wireframe 1: Initial design for the portfolio tool</em></p>
</div>

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Wireframe2%20HTXL.png" alt="Wireframe 2: Detailed layout for user interface" style="max-width: 60%;">
  <p><em>Wireframe 2: Detailed layout for user interface</em></p>
</div>


### Initial Database Setup
While developing the front-end of my application, I also began working on the database, as it was a big part of the project. During my research, I discovered temporal tables, which allow for versioning within the database—a feature HighTechXL lacked due to their reliance on Excel. I believed that implementing versioning in the database would enable interesting visualizations in Power BI, for example visualizing the growth of a venture. Therefore, I decided to implement temporal tables early on to test their functionality with Power BI.

To test the database setup, I collaborated with another intern, Andrea, who was working on portfolio management and Power BI. I asked Andrea to create a simple report using my database and compare it with one generated from the Excel master file. The results showed that, for Andrea, the database was as easy to use as the Excel master file.

<img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/tables%20and%20relatuions%20in%20DB.png" >
*This is one of the first database diagrams I made.*

### Finding the Right Style

For my project, there weren't any strict styling requirements, but because I didn't have a lot of experience with CSS and HTML, I decided to use a component library to help with styling. Additionally, because HightechXL was already using Tailwind in other applications, I decided to look for a component library that would work well with Tailwind.

Preline was my first library choice because I liked how the components looked and because of the large number of custom components it offered. Preline worked well in the beginning of the project as it was easy to use and my application was still small and relatively simple. However, as I needed to implement more complicated components like a multi-select, I encountered difficulties with Preline. Specifically, some bugs made it impossible to use Preline's multi-select with Angular's reactive form system that I used to get data out of input components. Additionally, Preline used a LOT of Tailwind code, which was often hard to read.


  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/WebApp%20I1.1.png" alt="First iteration using Preline 1" style="max-width: 60%;">
    <p><em>First iteration using Preline - Screenshot 1</em></p>
  </div>
  
  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/StepperPrelineCode.png" alt="First iteration using Preline - Stepper Code" style="max-width: 60%;">
    <p><em>First iteration using Preline - Stepper Code</em></p>
  </div>

In the second iteration, I wanted to take a step back because I was getting a bit overwhelmed by all the Tailwind code. I decided to set up my form again using Preline, based on a recommendation I received in the Angular Discord community. However, I chose not to implement Preline completely. Instead, I only copied the Tailwind HTML from the Preline website and did not install Preline into my program. While taking this step back, I also decided to temporarily not use a stepper and to put all the fields underneath each other. Additionally, I organized my input fields by placing them in their own separate folder within the components folder

  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/WebApp%20I2%20HTXL.png" alt="Second iteration using Flowbite 1" style="max-width: 60%;">
    <p><em>Second iteration using Flowbite - Screenshot 1</em></p>
  </div>
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/FormPrelineCode.png" alt="Second iteration using Flowbite - Code" style="max-width: 60%;">
    <p><em>Second iteration using Flowbite - Code</em></p>
  </div>

After getting to a point where a stepper needed to be implemented again, the approach of only using the Tailwind and HTML from Preline wouldn't suffice. I needed to install Preline to ensure the stepper would be implemented correctly. This prompted me to explore other options, including Google's design document on Material Design, which led me to Angular Material. I found the implementation and style of Angular Material more appealing than Preline, prompting me to make my final style switch to Angular Material. It was advantageous that I had already separated my components and used variables to set certain things like the labels or placeholders, making it very easy to implement Material.

 <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/POC%20Company%20Details.png" alt="POC Company Details Page" style="max-width: 60%;"">
  </div>
  <div style="text-align: center;">
    <img src="" style="max-width: 60%;"">
  </div>

to make sure all the fields ended up in the right step, I took a couple of sticky notes and wrote all inputs/necessary fields onto them. This way, I could easily group them and move them around. After grouping all the sticky notes, some of the other interns helped me come up with a couple of names for each step. These steps became: company details, mission team, and performance. Later, the extra step investments was added to these.

  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/StickyDevideOverSteps.jpg" style="max-width: 60%;">
  </div>

### First proof of concept build
Around halfway through my internship, I finished the first proof of concept build for the portfolio tool. This build was meant to test the portfolio tool with Hightechxls Ventures and did not have database/API integration yet (the API also did not exist at this point). This build worked with pre-set lists and did not save any data to a database. To host the build, my supervisor and I set up a pipeline on a separate branch using Githubs Actions to automatically build and push the proof of concept to an Azure server. This setup allowed me to push changes to the build, automatically updating the web server version, without interfering with other features I was working on.

One of the major features that I also wanted to test with the build was that after the portfolio had been filled in once, the data would be remembered for all following times (again, it was not stored in a database or anything, I did this locally using variables).

For this build, I also added a welcome screen and an end screen. The welcome screen would welcome the user, and the end screen would prompt the user to go through the form again. The second time the user would end up on the end screen, they would be thanked for filling in the form marking the end of the user test.


  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/POC%20Welcome%20page.png" style="max-width: 30%;">
  </div>
  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Filled%20in%20I1.png" style="max-width: 30%;">
  </div>
  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Tahnk%20you%20end%20page%20I1.png" style="max-width: 30%;">
  </div>

Another one of the features was the investmentForm component, which essentially acted as its own CRUD (Create, Read, Update, Delete) application. This component was at that point integrated into the performance step of the portfolio tool. Here, ventures had the ability to manage their investments by adding, editing, or removing them.

When users clicked on the "Add Investment" button, a small form would appear, where the ventures were able to input their investment's information and submit it to a list.

Following submission, the newly added investment would instantly populate a dynamically updating list within the performance step. This list served as a convenient hub, providing ventures with immediate access to all their investments. Each investment in the list would display key information about the investment and could be pressed on to show more information.

The listed ventures would also display an edit and delete button, allowing ventures to make necessary updates to investment details or remove investments.


  <div style="text-align: center;">
    <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/POC%20Investments%20page.png" style="max-width: 30%;">
  </div>

After discussions with the portfolio manager, it became clear that gathering the data filled in by the ventures during the user test was really helpful to test the portfolio tool. This led me to implement and make the API and database to collect all the information entered by the ventures.

### Creating a Back-end and connecting the front-end

For the back end, I used EF Core due to it being already in use within HighTechXL. Initially, I wanted to use the database I had already created, going for a database-first approach. However, implementing this proved challenging with EF Core due to compatibility issues with its migration system. That is why I transitioned to a code-first approach. In a code-first approach, the database is generated from the code, allowing for more flexibility and making it easier to change the database with the use of migrations.

After remaking my database using the code-first approach, I used .NET to automatically generate my initial API calls using their scaffolding system. The first API routes I created were the ones used to gather the lists that would be used inside my select components, including series, tech1, tech2, and sdgs. Which I integrated with my frontend by fetching the lists from the backend (and consequently, the database) instead of having them pre-coded.

After connecting all lists, I encountered a problem with how my application was set up. Due to the structure of my venture table at the time, I couldn't differentiate between a venture that hadn't already filled in a portfolio previously and one that had. Because I did not want to make all fields nullable in the database to determine if a user had filled in the form previously, as my supervisor, Jordy,  proposed as a possible solution, I looked for a better solution.

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/DBO%20post%20POC1%20V2.png?raw=true" style="max-width: 30%;">
  <p><em>Database before the venture table split</em></p>
</div>

That is why I decided to split the venture table into two separate tables: a venture table and a portfolio table. This change meant that I could check if a venture already had a portfolio linked to it. If it did, it meant that they had already filled in the portfolio. If not, it meant that they didn't already have a portfolio. This new structure also aligned better with the venture journey within HighTechXL's application.

This change made it challenging to incorporate temporal tables because it was still hard to know when to update a portfolio or when to add a new portfolio. Therefore, instead of figuring out a way to implement this, I decided to remove the temporal table. Instead, I altered the structure so that each time a venture filled in the tool, a new portfolio entry would be created and linked to that venture. Additionally, I included a new field in the portfolio table to store the date the portfolio was submitted. By adding a new portfolio entry instead of updating an existing one and recording the submission date, I maintained a form of versioning, with the added benefit that it was now possible to edit a particular portfolio in the database if some of the data were incorrect.

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Screenshot%20Database%20after%20venture%20table%20split%202024-05-08%20144702.png?raw=true" style="max-width: 30%;">
  <p><em>Database after the venture table split</em></p>
</div>

The only thing left to figure out was how I would know which venture was filling in the portfolio tool. This would normally be done using a login system, but because HighTechXL already had a login system in place that could be implemented into my application, and because it would take a lot of time to implement the login system, I decided to request the venture's ID instead on the starting page of my application.

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/WelcomePageLoginID.png" style="max-width: 30%;">
  <p><em>New welcome page with ID input</em></p>
</div>

### Login Functionality

After getting the application working again, I noticed a potential security risk with how I was calling my API. Because I was using an ID that could potentially be guessed, it would be possible to send requests to the API and gain access to a venture's data. 

While discussing this with the portfolio manager, we figured out some quick solutions. One suggestion was to refrain from hosting the project and instead keep it solely on my laptop locally. Ventures could then use my laptop to try out the portfolio tool, and we could implement HighTechXL's existing login system afterwards.

Even though this was a potential solution it really wasnt a good solution.

During discussions with my school mentor, Thijs, we explored several potential solutions to increase security without having to develop a complete login system. Some of the options we considered were implementing Google's OAuth for authentication, creating a simplified custom login system, or securing the server to protect the application.

I decided to develop a portion of the login system myself, focusing solely on the login functionality. This approach ensured that the API would be protected, and it allowed me to manually create login credentials for each venture. With this setup, only I had the authority to distribute access credentials directly, determining who could fill in the form and ensuring data analysis integrity for the user test.

After successfully configuring the back-end, I updated the welcome page on the front-end to integrate the new login system. Additionally, I created an authentication service responsible for storing the JWT token in the local storage.

<div style="text-align: center;">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/WelcomePageWithActualLogin.png" style="max-width: 30%;">
  <p><em>New login screen</em></p>
</div>

To get the other API calls working in my front-end again, I implemented an interceptor that intercepts the calls and adds the token form the local storage as a header.

And finally I made an error service that would redirect any 401 (unauthorized) to the login page.

### Second proof of concept build

With the new login system and both the front-end and back-end fully functional, Jordy and I used the same pipeline we had used for the first proof of concept build to host the second proof of concept build. Additionally, we set up a similar pipeline and created a database on the Azure server with extra login credentials specifically for the portfolio team to test the portfolio tool with Power BI.

To ensure the correct database structure was in place, I used EF Core to generate an initial SQL query that I could run on the server. This allowed me to set up the correct database structure. Furthermore, I used queries that I had created while developing the back-end to quickly and easily populate the database with all the predefined lists.

And after creating some login credentials in the database the portfolio tool, with back-end and database, was up and running again.

### Advanced investments

The main feedback I received during my halfway meeting at school was that it would be beneficial to expand the portfolio form by adding more advanced functionality that wouldn't typically work in standard forms. For example, making the form reactive depending on the specific venture that needs to fill it in.

However, making the form reactive for each company wouldn't be beneficial for HighTechXL because the data they need from each venture doesn't change depending on the venture. Instead, I had another idea: to make the investment form reactive. The investment step includes a part where the type of investment needs to be selected, such as equity or a CLA (Convertible Loan Agreement). These investments require completely different information to be filled in. For example, equity investments need details about share percentages and valuations, while a CLA requires information about loan terms and conversion conditions. 

#### Type
After I started sketching out all the necessary information for each type of investment, John, the CEO of HighTechXL, explained to me that although I was free to implement the reactive investments, it was not beneficial for several reasons. 

- First, for HighTechXL, the main pieces of information from an investment that are interesting to see in the portfolio are the type of investment, the stake HighTechXL has, and the amount that has been invested. This information can then be used to calculate the worth of the company, while any additional details can be looked up if needed. 

- Second, all the information that needs to be filled in also needs to be maintained, meaning that the more information required, the more work it will be to update if changes occur. 

- Lastly, requiring more data for each investment would take up more time from the ventures.

Because of this, I decided not to proceed any further with expanding the reactive aspects of the investment form.

#### Fund
Another part of the investment form that could be expanded was the way an investor was added or selected. Initially, ventures would fill in the information of the fund and its investor (email, name, chamber of commerce number, etc.), which would then be added as an investor in a separate table in the database. The problem was that there was no way to select investors already in the database. Every time a new investment was added, a new investor entry would also be created, even if multiple ventures had investments from the same investor.

Normally, this wouldn't be a big problem because we could filter by the name of an investor to find all the ventures that have received investments from that investor. Unfortunately, this approach wouldn't work reliably because people often write names differently, using various capitalizations or spacing.

The first thing I did to try and solve the problem was to split the investor table into two separate tables: a fund table and an investment manager table. The fund table would store the name of the investment fund and the Chamber of Commerce number, while the investment manager table would store the name and email of the manager. This way, I could keep track of the fund and manager separately. The fund could be linked to multiple investments, and the manager could be separate for each investment, as the manager's information was only necessary for contacting purposes.

After splitting the table, I needed a way to not only select a fund but also create a new fund. Although I could have implemented this with another new form, I felt that it would be too much to have another form pop up just for adding a fund. That is why I decided to use a type of autocomplete feature commonly seen when entering an address.

The idea was that the user would be able to start typing a fund name, and all funds with similar names already in the database would pop up. The user could then choose to select a fund from the list, which would automatically fill in the Chamber of Commerce number for the selected fund. If the venture had an investment with a new investor, they could simply fill in the fund details without selecting one of the "autocomplete options," which would also add the fund to the database.

In the investment form, I utilized Angular's Material Autocomplete component. With a bit of alteration, it already had the functionality to filter the funds by name and display the options in a list above the input field. One of the modifications I made was adding a display function to determine what would be shown and searched for when filtering. This allowed me to use the same component for the Chamber of Commerce field.

After successfully implementing the autocomplete component, I synchronized the fund name and Chamber of Commerce fields using the ValueChange method. This way one field would automatically update the other, and vice versa. To prevent potential infinite loops, I incorporated a variable to track when the value is permitted to change.



**NULL**

### User test
<img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/Windows%20feedback%20form.png">
<img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/PortfolioUsertestMailTemplate.png">

**NULL**

***
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

### Investements
**NULL**

### Stepper?
**NULL**

***
## Challenges and Solutions

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

angular
tailwind
efcore
**NULL**

### Soft Skills
**NULL**

<small><i><a href="https://github.com/BramVerkuijlen/Portfolio-S5-Internship"><- Back to the portfolio</a></i></small>
