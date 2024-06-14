# Investigative Problem Solving
*You take a critical look at your project from different perspectives, identify problems, find an effective approach and arrive at appropriate solutions.*
***

I demonstrated my investigative problem-solving skills multiple times during my internship. Here are a few problems I tackled during my internship:

## Checking the Need for the Portfolio Tool
One of the first steps in my project was to determine if the portfolio tool was necessary. To do this, I conducted extensive research on various data-gathering tools such as Windows Forms and Flutter. I also evaluated solutions that would integrate well with Power BI and address HighTechXL's data storage challenges. This comprehensive analysis ensured that the solution I developed was both needed and effective.

## Login System
One of the problems I encountered during the development of the portfolio tool was the need for a secure login system. Initially, I considered allowing ventures to "log in" using only their ID. This approach seemed efficient as it avoided the need to create a full-fledged login system, which would be redundant given that HighTechXL already had a login system in place. Moreover, developing a new login system from scratch would have been time-consuming.

However, this approach had a significant flaw: the ID of a venture could potentially be guessed. This vulnerability would allow potential attackers to not only view sensitive data but also send unauthorized data to the database using the API. Recognizing this risk, I consulted with my school mentor to brainstorm potential solutions.

After looking at potential options with my school mentor, I decided that the best approach was to create only the essential part of the login system—specifically, only the login functionality using JWT (JSON Web Tokens). This solution made sure the venture data was secure while avoiding the unnecessary duplication of a full login system. Implementing the login in this way would also make me the only person who could create login credentials, allowing only me to create and distribute safe credentials.

## Pre-filled Data
Another significant challenge was how to handle data input efficiently for the ventures using the portfolio tool. Most of the venture information remains consistent over time, and re-entering this data each time a venture fills in the form be cumbersome, prone to errors and take more time overall. To address this, I implemented a feature that pre-fills the data from the previous entry.

## Investment Fund Autofill
While adding an investment in the form, a venture needs to specify which fund has invested. Ventures often receive investments from the same investors, and to ensure the investments are linked correctly to a fund rather than an error-prone string (which can be written in various ways), I needed a better, more robust solution.

Creating a separate CRUD application for adding funds was one option, but it would add unnecessary steps when adding an investment. That is why I looked at how other applications handle similar issues and discovered the autofill feature commonly used for filling in addresses.

Although not entirely the same as filling in funds, I altered this concept to fit my project. My fund autofill feature allows users to quickly autocomplete a fund while typing if the fund is already in the database. This reduces the likelihood of input errors and saves time, while still allowing new funds to be added by simply filling in the information as usual.

<small><i><a href="https://github.com/BramVerkuijlen/Portfolio-S5-Internship"><- Back to the portfolio</a></i></small>
