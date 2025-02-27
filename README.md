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
      
<img width="1015" alt="image" src="https://github.com/user-attachments/assets/c9e0b771-6368-43ce-aa47-f0b04e90fea9" />

<img width="1012" alt="image 1" src="https://github.com/user-attachments/assets/b5703112-bd9a-4b0b-9b58-fdb3e6e02425" />

- Renaming Columns:
    - Renamed columns to ensure clarity and consistency in the dataset.

<img width="1012" alt="image 2" src="https://github.com/user-attachments/assets/cf400cf3-4b92-463a-aa5e-7c2df3c80a0f" />

- Converting Data Types and Mapping Values:
    - Converted columns to appropriate data types (e.g., encoded seasons to their actual full names, humidity values to percentage).
    - Mapped the season and weather dictionaries to their more meaningful labels for easier interpretation.

<img width="1007" alt="image 3" src="https://github.com/user-attachments/assets/6da5bbe1-6432-4237-b78e-11e312f9a909" />

- Final Check on Cleaned Data:
    - Conducted a final review to ensure no missing or inconsistent data remained.
    - 
<img width="1010" alt="image 4" src="https://github.com/user-attachments/assets/25755cd1-d04f-4c1f-9158-cfc888ea739b" />

You can find the detailed Python code and dataset in this Repository.

# **Crafting an Exploratory Dashboard with Tableau 📈**

With the cleaned dataset ready, I used **Tableau** to create interactive and insightful visualizations. The exploratory dashboard was designed to provide an overall view of bike ride patterns, weather impacts, and time-based trends.

1. **Moving Average (Line Chart)**: This visualization presented a timeline of bike rides over dates, serving as the master control for the entire dashboard, utilizing Tableau Actions.

<img width="1433" alt="image 5" src="https://github.com/user-attachments/assets/5ae9bd8b-5849-40a5-b283-a1751aa8b883" />

2. **Total Rides (Text KPI)**: Displayed the total count of bike rides KPI for the selected period, providing a quick overview of overall activity.

<img width="1424" alt="image 6" src="https://github.com/user-attachments/assets/5483638d-c356-465e-a748-c2f83a04854f" />

3. **Temperature vs Wind Speed (Heatmap)**: Explored the relationship between temperature and wind speed, revealing how weather conditions influence bike ride patterns.

<img width="1424" alt="image 7" src="https://github.com/user-attachments/assets/5224a6ef-64f3-47ec-8e3e-21c419abf67d" />

4. **Weather (Bar):** llustrated the distribution of weather conditions during the selected timeframe, highlighting trends in bike rides under different weather scenarios.

<img width="1424" alt="image 8" src="https://github.com/user-attachments/assets/c02555cb-d6f8-4a81-8493-0416ffe134e1" />

5. **Hour (Bar)**: Showed the distribution of bike rides throughout a 24-hour cycle, identifying peak ride times.

<img width="1388" alt="image 9" src="https://github.com/user-attachments/assets/ddb514ba-34b2-4319-b400-13b15c5f8f3c" />

6. **Full Exploratory Dashboard**

<img width="1297" alt="image 10" src="https://github.com/user-attachments/assets/ed61a5d3-476d-4d58-a8ad-f16b016176b0" />

- **Dynamic Filtering:** Visuals update based on the selected date range or hover interactions.
  
<img width="1220" alt="image 11" src="https://github.com/user-attachments/assets/2e8487ff-29a0-4369-9423-9722c5e96a9e" />

- **Tooltip Details:** Weather and hourly distributions are displayed in tooltips when hovering over the heatmap or timeline.

<img width="1211" alt="image 12" src="https://github.com/user-attachments/assets/db9fe445-87f9-4c5e-8124-f22e561db9fb" />

- **Customizable Moving Average:** Users can adjust the moving average period (day/week/month) and date range for deeper analysis.

<img width="1304" alt="image 13" src="https://github.com/user-attachments/assets/fab38062-127d-4ada-b0ec-a883adab84c2" />

Check out the interactive dashboard on my [Tableau Public Profile](https://public.tableau.com/views/LondonBikeRides_17406648274520/Dashboard1?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link) 

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
