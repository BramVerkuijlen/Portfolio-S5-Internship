# Investigative Problem Solving
*You take a critical look at your project from different perspectives, identify problems, find an effective approach and arrive at appropriate solutions.*
***

## Login System
One of the problems I encountered during the development of the portfolio tool was the need for a secure login system. Initially, I considered allowing ventures to "log in" using only their ID. This approach seemed efficient as it avoided the need to create a full-fledged login system, which would be redundant given that HighTechXL already had a login system in place. Moreover, developing a new login system from scratch would have been time-consuming.

However, this approach had a significant flaw: the ID of a venture could potentially be guessed. This vulnerability would allow potential attackers to not only view sensitive data but also send unauthorized data to the database using the API. Recognizing this risk, I consulted with my school mentor to brainstorm potential solutions.

After looking at potential options with my school mentor, I decided that the best approach was to create only the essential part of the login system—specifically,only the login functionality using JWT (JSON Web Tokens). This solution made sure the venture data was secure while avoiding the unnecessary duplication of a full login system.Implementing the login in this way would also make me the only person who could create login credentials, allowing only me to create and distribute safe credentials.

## Pre-filled Data
Another significant challenge was how to handle data input efficiently for the ventures using the portfolio tool. Most of the venture information remains consistent over time, and re-entering this data each time a venture fills in the form be cumbersome, prone to errors and take more time overall. To address this, I implemented a feature that pre-fills the data from the previous entry.

## Investment Fund Autofill
While adding an investment in the form a venture needs to add what fund has invested. Ventures often get investments from the same investors and to make sure the investments get linked to a fund instead of a error prone string which can be written in many different ways.I implemented an autofill feature. This allows users to quickly autocomplete a fund while typing if a fund is already in the database, reducing the likelihood of input errors and saving time. While still being able to add new funds by just filling in the information normally.

## Versioning in the Database
Finally, I recognized the need for versioning in the database to track the progression of ventures over time. This capability is crucial for analyzing historical data and making informed decisions based on past performance. Implementing versioning required a deep dive into the capabilities of EF Core and the database structure. After thorough research and testing, I successfully integrated a versioning system that allows HighTechXL to maintain a detailed history of each venture’s progress. This feature not only enhances data integrity but also provides valuable insights for future analysis and decision-making.

## Conclusion

Throughout the project, I applied critical thinking and problem-solving skills to address various challenges. By taking a strategic and investigative approach, I was able to implement effective solutions that improved the functionality and user experience of the portfolio tool. These experiences have strengthened my ability to tackle complex problems and deliver robust, user-centric solutions.


<small><i><a href="https://github.com/BramVerkuijlen/Portfolio-S5-Internship"><- Back to the portfolio</a></i></small>
