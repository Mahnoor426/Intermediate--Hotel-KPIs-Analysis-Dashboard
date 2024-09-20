# Detailed Explanation 
## About Data 
### Data Source: 
Data was provided by stakeholders and includes files like dim_date.csv, dim_hotels.csv, dim_rooms.csv, fact_aggregated_bookings.csv, and fact_bookings.csv.
### Dimensions:
1) dim_date.csv: Contains date-related information like day, week, month, and year.
2) dim_hotels.csv: Details about different hotels, such as hotel ID, name, and location.
3) dim_rooms.csv: Information about different rooms available, including room types and availability.
### Fact Tables:
1) fact_bookings.csv: Contains data on individual bookings, including booking ID, hotel ID, room ID, customer ID, booking date, and revenue generated.
2) fact_aggregated_bookings.csv: Aggregated data, such as total bookings and revenue per hotel or date.

## Data Preprocessing:
### ETL Process: 
Extracted data from CSV files, cleaned and transformed it to ensure consistency.
### Handling Missing Values: 
Null or missing values were removed, and all monetary values were converted into USD to standardize revenue data.
Created new metrics mentioned below. 

## KPI 
KPI include DSRN, DBRN AND DURN to monitor room availability.
Total Capacity to understand hotels potential and metrics like Total Cancelled and Total Successful Booking to understand booking sucess rates. 
### DSRN 
This metric represents the total number of rooms that are available for sale on a particular day. It considers rooms that are not under maintenance or blocked for any reason.
### DURN
The number of room nights actually used on a given day.
### DBRN 
Represents the number of room nights booked for a given day.
### Realisation %
This is the ratio of rooms used (actual bookings) to the total available rooms for a specific period. It can indicate the occupancy rate or booking efficiency.
### Occupancy %
The ratio of occupied rooms to available rooms, expressed as a percentage.
### Cancellation % 
The percentage of bookings that were canceled out of the total bookings made. This metric helps identify trends in guest behavior or booking issues.
### Revenue
revenue from completed stays is considered, excluding any potential bookings that were canceled or resulted in no-shows. This gives a more accurate picture of the actual revenue generated.
### RevPar
A standard metric in the hotel industry that combines occupancy and average daily rate (ADR) to measure overall performance.

## Insights From The Dashboard
I leveraged tooltips extensively to display additional contextual information, such as revenue, DSRN, DBRN, DURN, Realization %, and Cancellation %, allowing users to gain a deeper understanding of the metrics at a glance. These tooltips enabled a more detailed breakdown of data without cluttering the main visuals. The dashboard enables stakeholders to track these metrics on a daily, weekly, and monthly basis, helping in better decision-making related to pricing strategies, occupancy management, and guest satisfaction. This helped in revealing key insights like the impact of flat pricing strategies on revenue and occupancy.
The dashboard analysis suggested that despite high occupancy rates during weekends, the revenue did not increase proportionally due to the hotel's flat pricing strategy. This indicated a missed opportunity for dynamic pricing, which could optimize revenue based on demand fluctuations. The visual representation of these KPIs provided clear insights into how adjustments in pricing strategy could improve overall performance.

## DASHBOARD
![image](https://github.com/user-attachments/assets/57d72221-60db-4aa1-a8ee-813165b22557)
![image](https://github.com/user-attachments/assets/144ed066-70a8-4c91-b74d-64daee43770e)
![image](https://github.com/user-attachments/assets/8bfdedce-2f1d-49c1-9a09-bdd0ab05ca17)
![image](https://github.com/user-attachments/assets/20880728-c188-47a3-9580-a7fd82d06085)
![image](https://github.com/user-attachments/assets/f24aa8dc-d9ce-4003-9fea-129b42c46bcb)
![image](https://github.com/user-attachments/assets/e37926e2-4acd-4bc4-93ac-04063cd43b5d)
![image](https://github.com/user-attachments/assets/969e12db-f3bd-45e2-9f6e-65df203a5f31)
