India's Digital Payments Boom: A Data Analysis of RBI Transaction Trends (2020–2025)

A data analytics project on how India's digital payment ecosystem has grown, comparing UPI and other payment systems by transaction volume and value.

Problem Statement

How has India's digital payment ecosystem evolved between 2020 and 2025, and how do UPI and other payment modes compare in volume, value and growth?

Dataset
Source: Reserve Bank of India (RBI), Daily Digital Payments data
Size: 1,768 daily records, 50 columns (1 June 2020 to 31 January 2025)
Units: volumes in lakhs, values in INR crores
Tools

Python (pandas, matplotlib, seaborn), MySQL, Excel, Power BI

Status

In progress. This README will be updated as the project moves forward.

Data cleaning 

Found and removed 62 duplicate rows (identical except for id), leaving 1,706 daily records
Sorted records by date and converted date to datetime
Dropped 6 combined card columns that were reported only for Nov 2020–Sep 2021
Filled blanks with 0 where a payment system did not operate (weekends and holidays); left earlier blanks as missing where a series had not started
Added year, month, quarter, weekday, weekend flag and average UPI ticket size

Author

Sherin Kunjumon
