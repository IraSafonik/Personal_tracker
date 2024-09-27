# Personal Health and Phone Usage Data Analysis

## 💡 Project Overview
This project is a data analysis of personal health and phone usage metrics collected from various mobile apps. I have gathered data such as steps, sleep hours, active energy, and phone usage statistics (screen time, notifications, pickups) to explore potential relationships and trends. The project involves data collection, processing, visualization, and analysis using SQL, Python, and Tableau.

## ☝️ Project Goals
The primary goal of this project is to:
- Analyze personal health data and phone usage behavior.
- Visualize trends in daily health metrics (steps, sleep, active energy) and phone usage (screen time, notifications, pickups).
- Find correlations between my phone usage, health data, and self-assessed ratings of the day.
- Develop insights to improve daily habits and personal well-being.

## 💼 Tasks
1. Collect and structure data from health and phone usage apps.
2. Process and clean the data using Python.
3. Store and query the data using SQL for deeper analysis.
4. Visualize the data using Tableau for easy interpretation of trends and correlations.
5. Analyze the results and derive actionable insights to improve daily productivity and health.

## 🛠️ Tools and Technologies
- **CSV/Excel Files**: As data storage formats during data collection.
- **SQL**: For storing and querying the collected data.
- **DBeaver**: For managing the SQL database, running queries, and exploring the data.
- **Python**: For data processing and analysis.
  - Libraries: `pandas`, `numpy`, `matplotlib`
- **Jupyter Notebooks**: For data exploration and manipulation using Python.
- **Tableau**: For creating visualizations and dashboards to interpret trends.

## 🗂️ Data Sources
- **Health App**: Provides data on steps, sleep hours, and active energy.
- **Hapday App**: Provides a daily rating (rate of day) from 1 to 100.
- **Phone Usage Stats**: Provides data on screen time (hours), notifications (count), and pickups (count).

Example of a single day's data:
- Steps: 12,620
- Sleep: 8 hr 5 min
- Active Energy: 262 kcal
- Rate of Day: 83/100
- Screen Time: 8 hr 37 min
- Notifications: 116
- Pickups: 93

## 💻 Process and Steps

### 1️⃣ Step 1: Data Collection
I manually exported data from health and phone usage apps on a daily basis. This data was stored in CSV format to ensure consistency.

### 2️⃣ Step 2: Data Cleaning and Processing
Using Python and the `pandas` library, I cleaned the collected data:
- Converted sleep times to hours.
- Standardized formats for dates and numerical values.
- Removed any null or inconsistent entries.

### 3️⃣ Step 3: Storing Data in SQL
I used SQL to create a structured database for querying and deeper analysis. Example of creating the table:

```sql
CREATE TABLE health_data (
    date DATE,
    steps INT,
    sleep_hours FLOAT,
    active_energy INT,
    rate_of_day INT,
    screen_time_hours FLOAT,
    notifications INT,
    pickups INT
);
