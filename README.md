# HOTEL-BOOKINGS-CANCELLATION-AND-REVENUE-ANALYSIS.
An Explanatory Dashboard Analysis on the revenue Impact of Bookings Cancellations and  Why Overbooking is Necessary. 

---
## Project Overview 
This project examines booking and cancellation trends at our resort between **2015 and 2017**, with a particular focus on the high-demand summer months of **July and August**. The analysis explores how cancellation rates, average daily rates (ADR), and booking timelines influence both **revenue generation** and **revenue loss**.  

---
## Project Objective

This project analyses the relationship between bookings cancelled with revenue generated and revenue loss. 

---
## Data Dictionary
- The analysis was performed using a comprehensive dataset featuring booking details, guest demographics, distribution channels, and financial metrics etc.
 
| **Column Name**       | **Description**                                                                 | **Data Type**     | **Example of Data Type**   | **Values / Examples**                                                                 |
|------------------------|---------------------------------------------------------------------------------|-------------------|-----------------------------|---------------------------------------------------------------------------------------|
| Booking ID            | Unique identifier for each booking.                                             | Integer / String  | `Integer`                   | `10001`, `BKG_2345`                                                                   |
| Hotel                 | Type or name of the hotel within the Splendor Hotel Group.                      | String            | `Text`                      | `Resort Hotel`, `City Hotel`                                                          |
| Booking Date          | Date when the booking was made.                                                  | Date              | `YYYY-MM-DD`                | `2016-05-14`                                                                          |
| Arrival Date          | Date when guests are scheduled to arrive.                                        | Date              | `YYYY-MM-DD`                | `2016-07-01`                                                                          |
| Lead Time             | Number of days between the booking date and arrival date.                        | Integer           | `Numeric`                   | `34`, `120`                                                                           |
| Nights                | Number of nights the guests are booked to stay.                                  | Integer           | `Numeric`                   | `2`, `7`                                                                              |
| Guests                | Number of guests included in the booking.                                        | Integer           | `Numeric`                   | `1`, `4`                                                                              |
| Distribution Channel  | The channel through which the booking was made.                                  | String / Category | `Text`                      | `Direct`, `Online TA`, `Offline TA`, `Corporate`                                      |
| Customer Type         | Type of customer making the booking.                                             | String / Category | `Text`                      | `Transient`, `Corporate`, `Group`, `Contract`                                         |
| Country               | Country of origin of the guests (ISO code or name).                              | String            | `Text` (ISO Alpha-3 code)   | `PRT`, `USA`, `NGA`                                                                   |
| Deposit Type          | Whether a deposit was made for the booking.                                      | String / Category | `Text`                      | `No Deposit`, `Non Refund`, `Refundable`                                              |
| Avg Daily Rate        | Average daily rate for the booking.                                              | Float (Decimal)   | `Numeric (2dp)`             | `120.50`, `199.99`                                                                    |
| Status                | Final status of the booking.                                                     | String / Category | `Text`                      | `Check-Out`, `Canceled`, `No-Show`                                                    |
| Status Update         | Date of the last status update for the booking.                                  | Date              | `YYYY-MM-DD`                | `2016-07-02`                                                                          |
| Canceled (0/1)        | Binary indicator of whether the booking was canceled.                            | Integer (0/1)     | `Numeric`                   | `0 = Not Canceled`, `1 = Canceled`                                                    |
| Revenue               | Revenue generated from the booking (if not canceled).                            | Float (Decimal)   | `Numeric (2dp)`             | `850.00`, `0.00`                                                                      |
| Revenue Loss          | Revenue lost if the booking was canceled (0 or negative value if not canceled).  | Float (Decimal)   | `Numeric (2dp)`             | `-500.00`, `0.00`                                                                     |

---
## Cleaned Dataset

![image](Data.JPG)

#### Before diving into the analysis, we cleaned the data by:

- Checking and handling missing values.
- Verifying data types for each column.
- Removing duplicate records.

---
## Analysis and Calculations 

![image](Analysis1.JPG)
- **Analysis using Pivot tables and Conditional formatting to identify patterns and trends** 
---
## Explanatory Dashboard 

![image](Hotel_Dashboard.png)

---
## Insights 
### - **Cancellation Trends and Revenue Impact Analysis**  

![image](Image1.jpg)
  
- **High Cancellation Rates in Summer:**  
  - Peaks of **39% (2017)** and **34% (2016)** cancellation rates were recorded during July and August.  
  - This coincides with periods of **increased ADR**, amplifying the revenue impact.
 ---
### - **Revenue vs. Revenue Loss:**  
![image](Image2.jpg)

  - In **July 2016**, revenue reached **$781K**, but cancellations caused a **$398K loss**.  
  - In **August 2016**, revenue hit **$1M**, but **$593K was lost** due to cancellations.  
  - Overall, cancellations wiped out nearly **50% of peak summer earnings** which was approximately **$1M between July - August 2016**  
---
### - **Booking Patterns and Reliability** 
![image](Image3.jpg)

- **Bookings made >30 days before arrival:**  
  - Represent **83% of total cancellations**.  
  - Have a **38% cancellation rate**.  
  - Lower ADR: **$169 average**.  
---
![image](Image4.jpg)

- **Bookings made within 0–30 days of arrival:**  
  - Represent only **17% of cancellations**.  
  - Have a much lower **20% cancellation rate**.  
  - Higher ADR: **$191 average**.  

### - **Insight:** Last-minute bookings are both **more reliable** and **more profitable**.  
---
## Summary   
- By **overbooking same-month reservations during peak summer**, we can:  
- Offset early booking cancellations by filling rooms with more reliable last-minute reservations.  
- Increase revenue with higher ADR from short-term bookings.  
- Reduce revenue loss from cancellations, transforming potential losses into gains.  
---
## Conclusion 
- Cancellations are not only a challenge but also an opportunity. By strategically overbooking summer reservations, the resort can **recover the $1 million lost annually** and potentially unlock **additional revenue growth**.
---
## Recommendation 
- **Implement controlled overbooking** for July and August, aligned with historical cancellation trends.  
- **Prioritize late-booking customers** (0–30 days before arrival) who offer higher ADR and lower cancellation risk.  
- **Continuously monitor cancellation rates** to adjust overbooking thresholds dynamically.  
---
## About me
- I transform complex data into clear, actionable insights.
Using analytics, machine learning, and visualization, I help you understand trends, improve efficiency, and plan for the future.

Connect with me @https://www.linkedin.com/in/adetokunbo-olasupo-70aa042a1
