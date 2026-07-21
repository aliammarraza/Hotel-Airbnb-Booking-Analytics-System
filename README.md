# Hotel-Airbnb-Booking-Analytics-System
This Power BI portfolio project features a Hotel &amp; Airbnb Booking Analytics System. It transforms raw data into insights using ETL, star schema modeling, and DAX. The interactive dashboard tracks revenue, occupancy, and guest behaviour to optimize business decisions.

# 📌 Business Problem & Objective
A rapidly growing hospitality company managing hotels and Airbnb-style rentals across multiple cities faced challenges in tracking business performance. Relying on manual spreadsheet reports made it difficult to monitor revenue growth, occupancy fluctuations, and service quality.

This project delivers a centralized Business Intelligence solution using Microsoft Power BI to replace manual reporting. The system provides interactive, real-time insights into revenue, profitability, guest behavior, and operational efficiency.

# 📊 Dataset
Source Data: HotelAirbnb_PortfolioProject.csv

Volume: Approximately 150,000 hotel and Airbnb booking records.

Scope: Includes booking details, property info, revenue/pricing, guest demographics, and operational metrics like complaints and ratings.

# 🛠️ Data Sourcing & Transformation (ETL)
Data extraction, cleaning, and transformation were performed using Power Query to ensure high data quality and accuracy.

Standardization: Corrected data types and standardized date formats across the dataset.

Deduplication: Identified and removed duplicate Booking_ID records.

Handling Missing Values: Replaced null values in text fields (Meal Plan, Reviews, Complaints, Cancellations) with meaningful labels.

Feature Engineering: Created new categorical columns including Guest_Age_Group, Loyalty_Status, Booking_Lead_Category, Revenue_Category, Occupancy_Status, and Stay_Duration_Category.

Validation: Validated revenue calculations and strictly excluded cancelled bookings from occupancy rate calculations.

# 🗄️ Data Model
The data model was structured using a highly optimized Star Schema.
![Star Schema Data Model](Image-Sample/Executive_summary.png)

Fact Table: Fact_Bookings (Contains transaction details and measurable values).

Dimension Tables: Dim_Date, Dim_Guest, Dim_Property, Dim_Room, Dim_Payment, Dim_Location, Dim_Booking, Dim_Loyalty.

Measures: A dedicated _Measures table was created to house all DAX calculations cleanly.

