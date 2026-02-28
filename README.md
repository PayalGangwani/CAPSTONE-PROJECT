📌 Project Overview
This is an end-to-end Weather Data Analysis Capstone Project that explores atmospheric patterns, seasonal trends, and regional climate variations across global cities using Power BI for interactive dashboards and Python for Exploratory Data Analysis (EDA).
The dataset covers multiple cities across USA, Canada, and the Middle East with weather records spanning from 2013 to 2017.

🎯 Objectives
Analyze key weather metrics — temperature, humidity, wind speed, and air pressure
Identify seasonal trends and regional climate variations
Visualize geographical distribution of cities and weather patterns
Discover correlations between different atmospheric conditions
Build interactive Power BI dashboards for data-driven insights

🗂️ Project Structure
📁 Weather-Analysis-Capstone/
│
├── 📊 weather_analysis_powerbi.pbix    # Power BI Dashboard file
├── 📓 weather_eda.ipynb                # Python EDA Notebook
├── 📂 dataset/
│   ├── city_attributes.csv            # City latitude & longitude
│   ├── city_lookup.csv                # City & country mapping
│   ├── final_fact.csv                 # Main weather fact table
│   ├── date_lookup.csv                # Date dimension
│   └── time_lookup.csv                # Time dimension
├── 📋 WEATHER_ANALYSIS_PPT.pptx       # Project presentation
└── 📖 README.md                       # Project documentation

📊 Dataset Description
Column
Description
City
Name of the city
Country
Country of the city
Latitude
Geographic latitude
Longitude
Geographic longitude
Temperature
Recorded temperature
Humidity
Humidity percentage
Wind Speed
Wind speed measurement
Air Pressure
Atmospheric pressure
Weather Condition
Clear / Cloudy / Rainy etc.
Date
Date of observation
Time
Time of observation
Time Period: 2013 – 2017
Cities: USA (27), Israel (6), Canada (3) + others
Total Pages in Dashboard: 21 pages 

🛠️ Tools & Technologies
Tool
Purpose
Power BI Desktop
Interactive dashboards & visualizations
DAX
Calculated measures & KPIs
Power Query
Data transformation & ETL
Python
Exploratory Data Analysis (EDA)
Pandas / NumPy
Data manipulation
Matplotlib / Seaborn
Python visualizations

📈 Power BI Dashboard Pages
Page
Analysis
Explanation
Project introduction & objectives
Geographical Analysis
City distribution by country & latitude
Temperature Analysis
Seasonal temperature trends over time
Humidity & Air Pressure
Regional humidity & pressure patterns
Wind Speed Analysis
Wind speed trends & seasonal patterns
Weather Conditions
Hourly & seasonal weather condition breakdown

📊 Visualizations Built
🗺️ Geographical Analysis
Bar Chart — Top 10 countries by number of cities
Scatter Plot — Latitude distribution of cities across continents
Map Visual — Geographical distribution by latitude & longitude
🌡️ Temperature Analysis
Line Chart — Temperature trends over time (2013–2017)
Area Chart — Max temperature comparison (Portland vs Vancouver)
Bar Chart — Cities with highest & lowest average temperatures
💧 Humidity & Air Pressure
Heatmap — Humidity variation across cities
Time-Series Chart — Wind speed vs air pressure relationship
💨 Wind Speed Analysis
Wind Rose Chart — Prevailing wind directions by city
Radial Chart — Wind speed across months
Scatter Plot — Wind speed vs air pressure correlation
Heatmap — Average wind speeds by city & month
☁️ Weather Conditions
Heatmap — Busiest hours by weather condition

💡 Key Insights
🇺🇸 USA dominates the dataset with 27 cities — influencing overall weather patterns
🌍 Most cities fall in 30°–45° latitude — temperate climate zone
☀️ Peak temperatures occur in July–August every year — consistent seasonal pattern
💨 Wind speed peaks in October–November — post-monsoon/early winter period
📉 Inverse relationship between wind speed and air pressure — higher wind = lower pressure
🌬️ Vancouver has higher wind speeds than Portland — due to coastal exposure
📅 Seasonal temperature cycles repeat consistently from 2013–2017

🧩 Data Model
The project follows a Star Schema design:
         city_attributes
               │
               ▼
city_lookup ──► final_fact ◄── date_lookup
                    │
                    ▼
              time_lookup
                    │
                    ▼
                country
Dimension Tables:
city_attributes — latitude & longitude
city_lookup — city & country mapping
date_lookup — date dimension
time_lookup — time dimension
country — country reference
Fact Table:
final_fact — all weather measurements
