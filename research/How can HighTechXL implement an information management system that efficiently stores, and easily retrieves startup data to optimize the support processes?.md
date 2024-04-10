
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

***

## What storage solution would work best with PowerBI?

Given HighTechXL's current challenges in managing and retrieving data efficiently, integrating a structured storage system that works efficiently with PowerBI is essential. Choosing a storage solution that provides the necessary structural support while also integrating seamlessly with PowerBI is critical.

### PowerBI Data Source Integration
PowerBI supports a wide range of data sources, including cloud-based services, online services, and direct connections to databases. This versatility is crucial for HighTechXL, as it allows for flexibility in choosing a database solution that can provide the necessary structured storage while ensuring compatibility with PowerBI for advanced data analytics and visualization.
<sub>[2]</sub>


### The Case for SQL Databases
Considering HighTechXL's needs for an efficient, scalable, and integrated data management solution, a SQL database emerges as the most fitting choice.

#### What is SQL and How Does it Work?
SQL (Structured Query Language) is a standard programming language used for managing and manipulating relational databases. It functions through executing commands that perform tasks such as retrieving data, updating records, and defining permissions. SQL queries enable users to interact with the database, requesting specific information or making changes. Its widespread use across various database systems makes SQL a versatile and essential tool for database management.
<sub>[1]</sub>


#### Structured Data Management
SQL databases excel in handling structured data, offering a systematic approach to storing, retrieving, and managing information. The relational model allows for the definition of tables and relationships among them, which is beneficial for managing the diverse data types associated with startups, investments, and performance metrics.
<sub>[1]</sub>


#### Integration with PowerBI
SQL databases are well-supported by PowerBI, facilitating seamless data extraction and visualization. This compatibility enables HighTechXL to leverage advanced analytics and visualization tools, enhancing communication with stakeholders and investors.
<sub>[2]</sub>


#### Scalability
SQL databases address the growing data management needs of HighTechXL through scalability, which involves both upgrading the database server's hardware (vertical scaling) and adding more servers to distribute the load (horizontal scaling). This ensures that the database infrastructure can adapt to the organization's expansion.
<sub>[4]</sub>


#### Data Integrity and Reliability
SQL databases enforce data integrity through constraints and referential integrity checks, ensuring the data is accurate, consistent, and reliable.

#### Cost-Effectiveness
Open-source SQL databases like MySQL and PostgreSQL offer a cost-effective solution for data management, with no licensing fees and a wide range of free tools and extensions available.
<sub>[4]</sub>

#### Versioning Support
SQL databases support temporal tables, valuable for HighTechXL in maintaining a history of data modifications, enabling visibility into venture progress.
<sub>[3]</sub>

In summary, adopting a SQL database aligns well with HighTechXL's requirements for a robust, scalable, and efficient information management system.

***
## Streamlining the Collection of Venture Information

For HighTechXL, effectively gathering venture information from startups, each with its own unique business operations and data management practices, presents distinct challenges. The key is to implement methods that are flexible, user-friendly, and efficient, encouraging cooperation from the startups without exerting control over their operations. This makes it verry hard to automaticly collect venture data.

### Adopting a Hybrid Approach for Data Collection

A hybrid model, blending automated requests for data at predetermined intervals or milestones with provisions for manual updates by startups, offers a balanced solution. This strategy involves automatically requesting data at scheduled intervals or specific milestones and then allowing the ventures themselves to input or update their information manually. Although not a prefect solution because of the need for manual interaction, a completely automated solution will unfortionately not work in HighTechXLs situation.

#### Form Building Tools

While Google Forms and Microsoft Forms are accessible and user-friendly, they may not meet the advanced data collection needs of HighTechXL.
These platforms offer basic customization and integration capabilities but lack the advanced features necessary for complex data gathering, analysis, and integration tasks. For example, they might not support intricate logic, branching, or dynamic content that adapts based on user input, which could be critical for HighTechXL's ventures.
<sub>[5][6][7][8]</sub>

For creating more sophisticated forms, other builders like Feathery.

Feathery is a no-code form builder that enables the creation of sophisticated forms with advanced logic, integrations, and workflows. It supports over 100 integrations, allowing data to be sent to various systems, and offers a developer SDK for embedding forms with custom logic. It's designed for building personalized customer onboarding flows, loan applications, and more, without requiring extensive backend development.
<sub>[9]</sub>

However, it's important to note that most, if not all, form builders place the majority of their advanced features behind paywalls and subscriptions.

#### Integrating a Custom Web Application with HighTechXL's Venture Journey Tool

While form builders like Google Forms and Microsoft Forms provide simplicity and accessibility, a bespoke web application represents a significant leap forward in data collection and management for HighTechXL. This custom solution not only offers unparalleled flexibility and control but also integrates seamlessly with HighTechXL's pre-existing tools and systems. Crucially, it can be designed to enhance and work in harmony with the Venture Journey Tool that HighTechXL has already developed and is actively used by its ventures. Here's how this integration can elevate HighTechXL's support processes:

  - Dynamic Data Collection Enhanced by Venture Journey Insights: A custom web application can dynamically adjust its data collection focus based on insights gleaned from the Venture Journey Tool. By understanding the progress and current stage of each venture, the application can tailor the information it requests, ensuring relevance and minimizing redundancy.

   - Seamless Integration with Existing Ecosystem: By building upon the foundation of the Venture Journey Tool, the bespoke application ensures a seamless user experience for ventures. It becomes a natural extension of the tools they are already using, facilitating easier adoption and encouraging more consistent data submission.

   - Tailored User Experience: The custom web application can be designed with the specific needs and feedback of startups in mind, optimizing the interface and functionality for those who will use it the most. This tailored approach can lead to a more intuitive and engaging experience, increasing the likelihood of timely and accurate data submissions.

   - Enhanced Data Security within the Venture Ecosystem: Integrating the bespoke application with HighTechXL's existing platform allows for consolidated data security measures. It ensures that sensitive startup information is protected according to the highest standards of compliance and security, leveraging the protocols already in place within the Venture Journey Tool.

   - Unified Data Management and Analysis: The integration allows for a unified approach to data management, with the custom web application feeding directly into HighTechXL's databases and analytical tools, including the proposed SQL database and PowerBI. This unified data flow enhances the efficiency of data analysis, enabling more informed decision-making and personalized support for each venture.

Developing this bespoke web application and integrating it with the Venture Journey Tool requires a concerted effort in terms of development resources and time. However, the investment is justified by the significant benefits it brings in terms of data management efficiency, user experience, and the ability to provide targeted support to startups at every stage of their journey.
<sub>[10]</sub>
----------------


-------------
## What is the best way to manage Venture information?

What is the Best Way to Manage Venture Information?

Given that most people working at HighTechXL are not be familiar with SQL or a database, it's essential to provide a means for easy access and modification of database information beyond what's available in PowerBI, especially for things not implemented in the the Portfolio Tool. To address this a user-friendly database management tool or interface needs to be implemented. Such a tool should simplify the process of interacting with the database, allowing users to view, update, and manage venture data without needing to directly engage with SQL queries or understand the underlying database structure.

There are multiple options that would work for HighTechXL.

*I think the best would still be a web app (implemented in venture journey)*



-------------

## Conclusion


## References

## References

1. Amazon Web Services. "What is SQL?" (03-04-2024): https://aws.amazon.com/what-is/sql/
2. Microsoft. "Power BI Documentation" (03-04-2024): https://learn.microsoft.com/en-us/power-bi/
3. Microsoft. "SQL Server Documentation" (03-04-2024): https://learn.microsoft.com/en-us/sql/sql-server/?view=sql-server-ver16
4. The Knowledge Academy. "What are the advantages of SQL?" (03-04-2024): https://www.theknowledgeacademy.com/blog/advantages-of-sql/
5. Google Forms. (10-04-2024): https://www.google.com/forms/about/
6. Microsoft Forms. (10-04-2024): https://learn.microsoft.com/en-us/microsoft-365/online-surveys-polls-quizzes?view=o365-worldwide
7. Content Snare. "Google Forms vs Microsoft Forms." (10-04-2024): https://contentsnare.com/google-forms-vs-microsoft-forms/
8. Zapier. "Best Online Form Builder Software." (10-04-2024): https://zapier.com/blog/best-online-form-builder-software/
9. Feathery. (10-04-2024): https://www.feathery.io/
10. Kamee software (10-04-2024): https://kamee-software.com/blog/bespoke-web-applications


