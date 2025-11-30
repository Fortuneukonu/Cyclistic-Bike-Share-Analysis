# Cyclistic Bike-Share Analysis Case Study

**Role:** Junior Data Analyst (Google Data Analytics Capstone)
**Tools:** Python (Pandas, Matplotlib, Seaborn)
**Data Source:** Divvy Trip Data (December 2024 - November 2025)

## Executive Summary
Cyclistic, a bike-share company in Chicago, aims to maximize the number of annual memberships. This analysis explores historical trip data from the last 12 months to identify behavioral differences between casual riders and annual members.

The findings indicate that Annual Members utilize the service primarily for commuting (peaking at 8 AM and 5 PM on weekdays), while Casual Riders utilize the service for leisure (peaking on weekends and afternoons). To drive conversion, marketing strategies should target weekend usage and seasonal riding habits.

## Business Task
**Goal:** Design marketing strategies to convert casual riders into annual members.
**Key Stakeholders:** Director of Marketing, Cyclistic Executive Team.
**Business Question:** How do annual members and casual riders use Cyclistic bikes differently?

## Data Source and Preparation
The analysis is based on 12 months of historical trip data (5.5 million rows). Due to GitHub file size limits, the raw data was processed locally, and the final cleaned dataset is hosted externally.

* **Cleaned Dataset:** [View on Google Drive](https://drive.google.com/file/d/1YhH8sqntLZ4nH_tjpKIIsXbHeyQOoL8W/view?usp=sharing)
* **Original Source:** Motivate International Inc. (Divvy Data License Agreement)

### Methodology (Python/Pandas)
1.  **Data Merging:** Combined 12 monthly CSV files into a single dataframe.
2.  **Feature Engineering:** Calculated ride duration and extracted day of week and month.
3.  **Data Cleaning:**
    * Removed rides with negative duration or duration less than 1 minute to eliminate technical errors.
    * Removed rides with missing timestamps or station identifiers.
    * **Outcome:** Removed approximately 13% of the raw data, resulting in a final sample size of 4.8 million rows.

## Key Insights and Visualizations

### 1. Weekly Usage Patterns
Casual ridership peaks significantly on Saturdays and Sundays, whereas Annual Members exhibit consistent usage throughout the work week. This suggests casual riders use the service primarily for leisure activities.

![Weekly Usage Chart](Visualizations/weekly_usage.png)

### 2. Hourly Usage Patterns
Hourly data reveals distinct usage spikes for Members at 8 AM and 5 PM, confirming a commuting use case. In contrast, Casual riders demonstrate a gradual increase in usage throughout the day, peaking in the late afternoon.

![Hourly Heartbeat](Visualizations/hourly_heartbeat.png)

### 3. Seasonality
Casual ridership declines significantly during winter months (December through February), while Members continue to use the service. This indicates that casual riders are more sensitive to weather conditions, whereas members rely on the service for essential transport.

![Seasonality Chart](Visualizations/seasonality_fixed.png)

## Strategic Recommendations
Based on the analysis, the following strategies are recommended to convert casual riders:

1.  **Target Weekend Riders:** Implement a marketing campaign focused on weekend users. Notifications sent on Friday afternoons comparing weekend pass costs to annual membership savings could drive conversion.
2.  **Seasonal Membership Tier:** Introduce a seasonal membership (May through September) to capture the segment of casual riders who are highly active in summer but inactive in winter.
3.  **Leisure Incentives:** Offer member-only benefits that appeal to leisure riders, such as extended ride time limits on weekends (e.g., 45 minutes instead of 30), to incentivize upgrades without impacting weekday commuter availability.

## Repository Structure
* **01_Data:** Documentation on data sources and access links.
* **02_Scripts:** Python code used for data processing and visualization.
* **03_Visualizations:** Output charts generated from the analysis.
* **04_Reports:** Final project documentation.
