# London Bike Rides Data Analysis Project 🚴‍♂️📊

**Tableau Link:** https://public.tableau.com/views/LondonBikeRides_17406648274520/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link

## Introduction

This project explores patterns and trends in London’s bike ride data, leveraging a dataset sourced from **Kaggle**. The goal was to analyze bike ride activity, understand the impact of weather conditions, and identify time-based trends to derive actionable insights. The project demonstrates a comprehensive workflow, from **data cleaning** and **preprocessing** using Python to the creation of an **Exploratory Dashboard** in Tableau.

## Dataset Overview

The dataset used in this project is the **London Bike Sharing Dataset**, sourced from [Kaggle](https://www.kaggle.com/datasets/hmavrodiev/london-bike-sharing-dataset). It provides detailed information about bike-sharing activity in London, including ride counts, weather conditions, and timestamps. The dataset is publicly available and widely used for analyzing urban mobility patterns.

### Key Features of the Dataset:

- **Timestamp:** Date and time of each bike ride.
- **Ride Counts:** Number of bike rides per hour.
- **Weather Conditions:**
    - Temperature (in Celsius).
    - Relative humidity (in percentage).
    - Wind speed (in km/h).
    - Weather summary (e.g., clear, rain, snow).
- **Seasonal Information:** Categorical data indicating the season (e.g., spring, summer, autumn, winter).
- **Holiday and Weekend Indicators:** Binary flags to identify holidays and weekends.

### Dataset Structure:

- **Rows:** Approximately 17,000 records (hourly data over two years).
- **Columns:** 10 attributes, including ride counts, weather metrics, and time-based features.

### Relevance to the Project:

This dataset is ideal for analyzing trends in bike-sharing activity, understanding the impact of weather on rider behavior, and identifying peak usage times. Its comprehensive features enable a multi-dimensional analysis, making it a valuable resource for urban mobility studies.

## Data Cleaning and Preprocessing with Python

Before diving into analysis, I performed extensive data cleaning and preprocessing to ensure the dataset was ready for exploration. Using **Python** and the **Pandas** library, I transformed the raw data into a clean, analysis-ready format.

- Loading the Dataset:
    - Imported the dataset using Pandas and performed an initial inspection to understand its structure and identify missing or inconsistent data.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image.png)

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%201.png)

- Renaming Columns:
    - Renamed columns to ensure clarity and consistency in the dataset.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%202.png)

- Converting Data Types and Mapping Values:
    - Converted columns to appropriate data types (e.g., encoded seasons to their actual full names, humidity values to percentage).
    - Mapped the season and weather dictionaries to their more meaningful labels for easier interpretation.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%203.png)

- Final Check on Cleaned Data:
    - Conducted a final review to ensure no missing or inconsistent data remained.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%204.png)

You can find the detailed Python code and dataset in my [GitHub repository](https://github.com/aimanmaznan/LondonBikeRidesAnalysis).

# **Crafting an Exploratory Dashboard with Tableau 📈**

With the cleaned dataset ready, I used **Tableau** to create interactive and insightful visualizations. The exploratory dashboard was designed to provide an overall view of bike ride patterns, weather impacts, and time-based trends.

1. **Moving Average (Line Chart)**: This visualization presented a timeline of bike rides over dates, serving as the master control for the entire dashboard, utilizing Tableau Actions.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%205.png)

2. **Total Rides (Text KPI)**: Displayed the total count of bike rides KPI for the selected period, providing a quick overview of overall activity.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%206.png)

3. **Temperature vs Wind Speed (Heatmap)**: Explored the relationship between temperature and wind speed, revealing how weather conditions influence bike ride patterns.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%207.png)

4. **Weather (Bar):** llustrated the distribution of weather conditions during the selected timeframe, highlighting trends in bike rides under different weather scenarios.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%208.png)

5. **Hour (Bar)**: Showed the distribution of bike rides throughout a 24-hour cycle, identifying peak ride times.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%209.png)

6. **Full Exploratory Dashboard**

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%2010.png)

- **Dynamic Filtering:** Visuals update based on the selected date range or hover interactions.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%2011.png)

- **Tooltip Details:** Weather and hourly distributions are displayed in tooltips when hovering over the heatmap or timeline.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%2012.png)

- **Customizable Moving Average:** Users can adjust the moving average period (day/week/month) and date range for deeper analysis.

![image.png](London%20Bike%20Rides%20Data%20Analysis%20Project%20%F0%9F%9A%B4%E2%80%8D%E2%99%82%EF%B8%8F%F0%9F%93%8A%201a7b1a7e4bd880ae808cdb00f17fef92/image%2013.png)

Check out the interactive dashboard on my [Tableau](https://public.tableau.com/views/LondonBikeRides_17406648274520/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) Public profile.

## Insights and Takeaways 🚀

Through this analysis, I uncovered several key insights about London’s bike ride patterns:

1. **Seasonality Trends:**
    - The **Moving Average** visualization revealed clear seasonality, with higher ride counts during warmer months and lower counts during colder periods.
2. **Weather Impact:**
    - The **Temperature vs Wind Speed Heatmap** showed that bike rides are more frequent on days with moderate temperatures and low wind speeds, highlighting the influence of weather on rider behavior.
3. **Peak Ride Times:**
    - The **Hourly Distribution** chart identified peak ride times during morning and evening rush hours, providing valuable insights for resource allocation and infrastructure planning.
4. **Weather Preferences:**
    - The **Weather Distribution** bar chart indicated that most rides occur on clear or partly cloudy days, with fewer rides during rain or snow.

## Tools and Technologies Used

- **Python** (Pandas, NumPy) for data cleaning and preprocessing.
- **Tableau** for creating interactive and dynamic visualizations.
- **GitHub** for version control and sharing the project code.

## Conclusion

This project not only increased my technical skills in data cleaning and visualization but also deepened my understanding of how data can be used to uncover meaningful insights. 

By combining Python’s data manipulation capabilities with Tableau’s visualization power, I was able to transform raw data into actionable insights that could inform decision-making for urban planners, bike-sharing companies, and policymakers.

Explore the full project on GitHub and interact with the visualizations on Tableau Public.