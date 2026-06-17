# -Electric-Vehicle-Analysis-Dashboard-

PROBLEM STATEMENT 
KPI’S Requirement
Total Vehicles
Average Electric Range
Total BEV Vehicles and % of Total BEV Vehicles
Total PHEV Vehicles and % of Total PHEV Vehicles
Charts Requirement
Total Vehicles by Model Year 
Total Vehicles by State
Top 10 Total Vehicles by Make
Total Vehicles by CAFV Eligibility
Top 10 Total Vehicles by Model
 Filter Panel
     The report includes a filter panel that allows users to interactively filter the data by City           
      and Model Year.
 Background Color
By using the PPT, I have created this and saved the picture.

<img width="1748" height="989" alt="Image" src="https://github.com/user-attachments/assets/070ce725-d4c3-4e17-9ee0-1586742c14b6" />

Data Cleaning
1. Data Preparation
Data Cleaning: The raw dataset was processed using Power Query to remove unwanted rows, ensuring accuracy and consistency for analysis.1
2. KPI and Metric Definition


The report utilizes specific DAX measures to analyze the electric vehicle market, including:
Total Vehicles: A count of total records based on DOL Vehicle ID.
Vehicle Classification: Calculated fields for Battery Electric Vehicles (BEV) and Plug-in Hybrid Electric Vehicles (PHEV) using the CALCULATE function.
Market Share: Percentage metrics (% of BEV and % of PHEV) derived by dividing the specific vehicle type counts by the Total Vehicles count.1
3. Reporting Requirements & Analysis Strategy


The preparation followed a structured approach to address specific analytical goals:2
Landscape Analysis: Assessing total market size and growth trends.
Efficiency Metrics: Determining average electric range.
Categorization: Identifying the volume and percentage share of both BEVs and PHEVs.
4. Visualization Plan


The report is designed to include the following visualizations to provide deeper insights:2
Adoption Trends: A line/area chart showing vehicle counts by model year (from 2010 onwards).
Geographic Distribution: A map chart illustrating vehicle distribution by state.
Market Leaders: A bar chart highlighting the top 10 manufacturers (Make) and a treemap displaying the top 10 vehicle models.
Incentive Impact: A pie or donut chart showing eligibility for Clean Alternative Fuel Vehicle (CAFV) incentives.
5. Tools and Software
Data Processing: MS Excel (2021) with Power Query.
Visualization & Analytics: Power BI (Dec 2026 version).
Dax Functions used in BI Report

Total Vehicles = COUNT(Electric_Vehicle_Population_Data[DOL Vehicle ID])
BEV = CALCULATE([Total Vehicles],Electric_Vehicle_Population_Data[Electric Vehicle Type]="Battery Electric Vehicle (BEV)")
PHEV = CALCULATE([Total Vehicles],Electric_Vehicle_Population_Data[Electric Vehicle Type]="Plug-in Hybrid Electric Vehicle (PHEV)")
% of BEV = [BEV]/[Total Vehicles]
% of PHEV = [PHEV]/[Total Vehicles]



<img width="1920" height="1200" alt="Image" src="https://github.com/user-attachments/assets/a09f89d3-7ba8-40f7-828b-0045c2395702" />
<img width="4408" height="2523" alt="Image" src="https://github.com/user-attachments/assets/82671dd1-7bb7-44c8-ac10-fcfdb142b12c" />


