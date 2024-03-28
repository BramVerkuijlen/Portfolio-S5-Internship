
# How can HighTechXL implement an information management system that efficiently stores, and easily retrieves startup data to optimize the support processes?

<p align="center">
  <img src="https://github.com/BramVerkuijlen/Portfolio-S5-Internship/blob/main/images/exploding%20database.png" alt="IMG Broke :(" width="50%" height="50%" />
</p>

*[Canva](https://www.canva.com) AI Picture Generation Tool*

***

## Introduction

HighTechXL is facing significant challenges in keeping pace with its data management demands during its rapid expansion. The organization's dependency on a large Excel file for storing crucial data about the startups it supports has become increasingly problematic. What once was an efficient system has now become unwieldy due to fast-paced growth, resulting in a file cluttered with outdated information and a slow, error-prone manual update process.

The manual updating of the master file, requiring data extraction and input from various sources like presentations and phone calls, is both time-consuming and susceptible to errors. This approach to data management is proving unsustainable for an organization experiencing rapid growth.

While the use of PowerBI for communicating with investors does offer structured and visually appealing data presentations, it also brings to light additional challenges. One major issue is finding the correct fields within the database, as some may be outdated, making it difficult to ensure the accuracy and relevance of the data presented. Another challenge is fitting all necessary information onto a page, given that the Excel file does not limit the size of a data field, which can complicate the presentation and interpretation of data in PowerBI.

These issues underscore the urgent need for HighTechXL to adopt a more advanced information management solution. The current system's limitations, including difficulties with using PowerBI effectively due to outdated fields and the unwieldy nature of the Excel database, highlight the necessity for a streamlined and efficient approach to data management to support the organization's continued growth.

## What storage solution would work best with PowerBI?
Given HighTechXL's current challenges with managing and retrieving data efficiently, integrating a structured storage system is hat works efficiently with PowerBI it is essential
to choose a storage solution that not only provides the necessary structural support but also integrates seamlessly with PowerBI. 

### PowerBI data sources
PowerBI supports a wide range of data sources, including cloud-based services, online services, and direct connections to databases. 
This versatility is crucial for HighTechXL, as it allows for flexibility in choosing a database solution that can provide the necessary structured storage while ensuring compatibility with PowerBI for advanced data analytics and visualization.

### Database

For HighTechXL, leveraging a database system is essential to overcome the limitations of the current Excel-based data management approach. 
A database will offer a more robust, scalable, and efficient method of storing, managing, and retrieving data.

A database, as opposed to simpler file or blob storage solutions, offers structured data management, enabling complex queries, relationship mapping between different data types, and transactional integrity. This structured approach is particularly beneficial for HighTechXL, given the varied and relational nature of the data involved—spanning startup details, investment information, and performance metrics. Databases support indexing, which dramatically improves the speed and efficiency of data retrieval operations, a critical factor for real-time analysis and decision-making.

### what type of database

htxl needs a good structured database that can handle all the information they would like to store. a database like mongo db can store files and is easyer in relations unfortionately powerbi doesnt fully support mongo db as of yet

SQL/MySQL

AzureSQL

PostgreSQL
https://learn.microsoft.com/en-us/power-bi/connect-data/desktop-data-sources

### how does the database look


## What is the best way to manage Venture information?

## What would be the best way to gather venture information?

winforms or google forms wont work (they are to strict and would take to long to fill in because they are not reactive)

### Automated collection

### Manual collection


## Conclusion


## sources

- [PowerBI](https://learn.microsoft.com/en-us/power-bi/)
