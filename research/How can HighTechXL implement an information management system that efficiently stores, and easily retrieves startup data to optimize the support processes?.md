
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

Given HighTechXL's current challenges in managing and retrieving data efficiently, integrating a structured storage system that works efficiently with PowerBI is essential. Choosing a storage solution that provides the necessary structural support while also integrating seamlessly with PowerBI is critical.

### PowerBI Data Sources
PowerBI supports a wide range of data sources, including cloud-based services, online services, and direct connections to databases. This versatility is crucial for HighTechXL, as it allows for flexibility in choosing a database solution that can provide the necessary structured storage while ensuring compatibility with PowerBI for advanced data analytics and visualization.
[PowerBI](https://learn.microsoft.com/en-us/power-bi/)

### Database
Considering HighTechXL's needs for an efficient, scalable, and integrated data management solution, a SQL database emerges as the most fitting choice.

#### What is SQL and How Does it Work?
SQL (Structured Query Language) is a standard programming language used for managing and manipulating relational databases. It functions through executing commands that perform tasks such as retrieving data, updating records, and defining permissions. SQL queries enable users to interact with the database, requesting specific information or making changes. Its widespread use across various database systems makes SQL a versatile and essential tool for database management.
[amazon](https://aws.amazon.com/what-is/sql/)

#### Structured Data Management
SQL databases excel in handling structured data, offering a systematic approach to storing, retrieving, and managing information. The relational model allows for the definition of tables and relationships among them, which is beneficial for managing the diverse data types associated with startups, investments, and performance metrics.
[amazon](https://aws.amazon.com/what-is/sql/)

#### Integration with PowerBI
SQL databases are well-supported by PowerBI, facilitating seamless data extraction and visualization. This compatibility enables HighTechXL to leverage advanced analytics and visualization tools, enhancing communication with stakeholders and investors.
[PowerBI](https://learn.microsoft.com/en-us/power-bi/)

#### Scalability
SQL databases address the growing data management needs of HighTechXL through scalability, which involves both upgrading the database server's hardware (vertical scaling) and adding more servers to distribute the load (horizontal scaling). This ensures that the database infrastructure can adapt to the organization's expansion.
[theKnowladgeacademy](https://www.theknowledgeacademy.com/blog/advantages-of-sql/)

#### Data Integrity and Reliability
SQL databases enforce data integrity through constraints and referential integrity checks, ensuring the data is accurate, consistent, and reliable.

#### Cost-Effectiveness
Open-source SQL databases like MySQL and PostgreSQL offer a cost-effective solution for data management, with no licensing fees and a wide range of free tools and extensions available.
[theKnowladgeacademy](https://www.theknowledgeacademy.com/blog/advantages-of-sql/)

#### Versioning Support
SQL databases support temporal tables, valuable for HighTechXL in maintaining a history of data modifications, enabling visibility into venture progress.
[Microsoft.com](https://learn.microsoft.com/en-us/sql/sql-server/?view=sql-server-ver16)

In summary, adopting a SQL database aligns well with HighTechXL's requirements for a robust, scalable, and efficient information management system.

[amazon](https://aws.amazon.com/what-is/sql/)
[theKnowladgeacademy](https://www.theknowledgeacademy.com/blog/advantages-of-sql/)
[PowerBI](https://learn.microsoft.com/en-us/power-bi/)
[Microsoft.com](https://learn.microsoft.com/en-us/sql/sql-server/?view=sql-server-ver16)

### how does the database look


## What is the best way to manage Venture information?

## What would be the best way to gather venture information?

winforms or google forms wont work (they are to strict and would take to long to fill in because they are not reactive)

### Automated collection

### Manual collection


## Conclusion


## References

- Amazon Web Services. What is SQL?: Retrieved from https://aws.amazon.com/what-is/sql/
- Microsoft. Power BI Documentation: Retrieved from https://learn.microsoft.com/en-us/power-bi/
- Microsoft. SQL Server Documentation: Retrieved from https://learn.microsoft.com/en-us/sql/sql-server/?view=sql-server-ver16
- The Knowledge Academy: What are the dvantages of SQL?. Retrieved from https://www.theknowledgeacademy.com/blog/advantages-of-sql/

