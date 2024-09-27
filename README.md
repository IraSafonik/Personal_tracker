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
```

### 4️⃣ Step 4: Data Analysis in Python
I used Python to analyze the data, calculate average daily steps, sleep hours, and identify any trends over time. I also explored correlations between metrics such as sleep and screen time, and the rate of day.

### 5️⃣ Step 5: Data Visualization with Tableau
I imported the cleaned and processed data into Tableau for visualization. This allowed me to create:

Time-series charts to observe trends over time.
Correlation heatmaps between different metrics (e.g., sleep and rate of day).
Comparative bar charts to see changes in behavior over weeks.

## 🌿 Results and Conclusion

Through this project, I identified several key insights:
- Sleep and Productivity: On days with more sleep, I tended to give higher daily ratings (rate of day).
- Screen Time Impact: Higher screen time correlated with more notifications, but not necessarily with lower active energy or step count.
- Consistency: I observed consistent patterns in steps taken per day, though variations occurred during weekends.

Overall, this analysis provided useful insights into how my daily habits impact my well-being. It also served as a foundation to optimize my daily routines and maintain a balanced lifestyle.

