Electric Vehicles Sales Analysis
 1. DEFINITION

This practical is based on analyzing Electric Vehicle (EV) Sales Data using visualization and transformation tools. The 
dataset includes details such as vehicle category (2-Wheelers, 4-Wheelers), makers (BMW India, OLA Electric, BYD 
India, etc.), sales by states, penetration rates, CAGR, and monthly trends. The objective is to clean, transform, and 
visualize the dataset to understand the growth, sales performance, and market trends of electric vehicles in India.

 2. OUTCOMES / LEARNING
- Understood how to import and clean raw EV sales datasets into a BI tool.
- Learned how to transform columns (date, vehicle_category, maker, state, etc.) for analysis.
- Analyzed the CAGR (Compound Annual Growth Rate) of makers and states. - Compared the revenue growth rates of 2-Wheelers vs. 4-Wheelers.
- Created trend analysis visuals such as line charts for monthly sales.

3. REQUIRED TOOL

Microsoft Power BI Desktop, KAGGLE

5. WORKING

In this practical, the given datasets were imported into Power BI and transformed using Power Query. The raw files 
included sales data by makers (electric_vehicle_sales_by_makers.csv), by state 
(electric_vehicle_sales_by_state.csv), and monthly sales trends. After data cleaning, transformations were applied 
such as date formatting, aggregation of electric vehicles sold, and calculation of penetration rate. Finally, multiple 
visuals (line charts, bar charts, and tables) were created to present insights on sales trends, growth rate, and market 
penetration across states and vehicle categories.

5.  Dataset

Source: Kaggle (dim_data.csv, electric_vehicles_sales.csv)
Records: ~817 rows
Key Fields:
{(date, fiscal_year, quarter), (date, vehicle_category, maker, electric_vehicles_sold)}

6. STEPS


Step 1: Importing the Dataset 
Imported the raw dataset files: 
-electric_vehicle_sales_by_makers
-electric_vehicle_sales_by_state
-dim_data.csv (for monthly and category-wise data). 
Verified column names such as date, vehicle_category, maker, state, electric_vehicles_sold, and total_vehicles_sold. 
Ensured correct data types for date (Date format), electric_vehicles_sold (Integer), and total_vehicles_sold (Integer).

Step 2: Data Cleaning & Transformation in Power Query 
Removed null/blank rows and standardized column names. 
Checked for zero values in electric_vehicles_sold and confirmed data quality. 
Split and reformatted the date column to extract Month and Year.

Step 3: Creating Revenue Growth Calculations 
Calculated Revenue Growth Rate 2022 vs 2024 and 2023 vs 2024 for both categories: - 2-Wheelers = 269.28% (2022 vs 2024) - 4-Wheelers = 367.79% (2022 vs 2024) 
Summarized overall growth = 324.92% (2022 vs 2024).  

Step 4: CAGR Analysis by Makers and States 
Added measures to calculate CAGR for each maker and state. 
Results showed BMW India had the highest CAGR (1140.97%), followed by Volvo Auto India (971.21%). 
By states, Meghalaya had the highest CAGR (28.47%). 

Step 5: Sales Trend Analysis by Month 
Created a line chart using date (Month-Year) vs. Sum of electric_vehicles_sold. 
Observed peak sales around April, with fluctuations in mid-year and a rise towards November.

Step 6: State-Wise Penetration Rate & Projected Sales 
Used the state column along with electric_vehicles_sold and total_vehicles_sold to calculate penetration rate. 
Projected sales for 2030 were visualized in a table, highlighting Karnataka and Delhi as top contributors.

Step 7: Building the Dashboard 
Combined visuals into a dashboard:
- Line chart (Monthly Sales)
- Bar chart (Sales by State)
- Bar chart (Penetration Rate by State)
- Tables for CAGR by makers and states
