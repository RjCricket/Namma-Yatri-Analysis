
# Namma Yatri Analysis

The objective of this project is to gain insights into the trip booking process and user interactions within the Namma Yatri mobile app.   

**tripid:** Unique identifier for each trip.  
**Searches:** User inputs current location and destination.  
**Searches_got_estimates:** User sees estimated fare price.  
**Searches_for_quotes:** User searches for available drivers.  
**Searches_got_quotes:** A driver is assigned to the customer.  
**customer_not_cancelled:** The customer didn't cancel the trip.     
**driver_not_cancelled:** The driver didn't cancel the trip.        
**otp_entered:** OTP (One-Time Password) is entered, likely for authentication purposes.              
**end_ride:** The driver ends the trip.

## Data Exploration using SQL

In this project, we connected an Excel file containing our dataset to SQL for analysis. This allowed us to leverage SQL's querying and analysis capabilities on the data stored in the Excel file. Below are the main steps involved in this process:

### Steps:
1. **Import Excel Data to SQL Database**: We imported the data from the Excel file into a SQL database table. This was done using a tool or method that allows for importing Excel data into a SQL database. Common methods include using MySQL Import Wizard or SQL statements such as `INSERT INTO`.

2. **Establish Connection to SQL Database**: After importing the data, we established a connection to the SQL database containing the imported Excel data. This connection was necessary for querying and analyzing the data using SQL.

3. **Perform Data Exploration and Analysis**: With the Excel data now available in the SQL database, we performed data exploration and analysis using SQL queries. This included tasks such as calculating basic statistics, analyzing data distributions, identifying patterns, and generating insights from the data.
### Example Queries:  
```sql
SELECT (COUNT(tripid) - SUM(driver_not_cancelled)) driver_cancelled_trips  
FROM trips_detail;
```

![Screenshot (1303)](https://github.com/RjCricket/Namma-Yatri-Analysis/assets/118374392/a295aafb-943c-455b-beaf-32fbf82e84b4)

### Some of the Queries of the Project are:
Q What is the total number of completed trips?  
Q What is the total driver’s earnings during a day?  
Q What is the average fare per trip?  
Q What is conversion rate?  
Q Who are the top 5 earning drivers?  
Q In which duration, there is the highest number of trips in each of the location present?  
Q Which area has highest number of cancellations by drivers?  
Q Which driver and customer pair had most trips together?  

## Dashboard Creation using PowerBi

[PowerBi Dashboard link](https://app.powerbi.com/view?r=eyJrIjoiNmJmOTRiZGUtNzU3YS00MTU4LWIyNGMtNzE3ZWY5MzBiMmU5IiwidCI6ImRmODY3OWNkLWE4MGUtNDVkOC05OWFjLWM4M2VkN2ZmOTVhMCJ9)

By visualizing key metrics and stages of the trip booking journey, the dashboard aims to help stakeholders understand user behavior, identify potential bottlenecks, and optimize the customer experience.  

Here is the screenshot of the namma yatri website showing all the parameters.


![Screenshot (1344)](https://github.com/RjCricket/Namma-Yatri-Analysis/assets/118374392/d9a5965c-e362-4311-932b-bb0d11dc0b25)


Screenshot of my powerbi dashboard:

![Screenshot (1334)](https://github.com/RjCricket/Namma-Yatri-Analysis/assets/118374392/fe8627ca-2caf-415d-b26d-c5a90201bf7e)

