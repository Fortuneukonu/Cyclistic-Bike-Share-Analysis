# Cyclistic Bike-Share: Marketing Strategy Report

**Date:** November 30, 2025
**Prepared By:** [Your Name]
**Role:** Junior Data Analyst
**Stakeholders:** Lily Moreno (Director of Marketing), Cyclistic Executive Team

---

## 1. Executive Summary
The goal of this analysis was to identify how annual members and casual riders use Cyclistic bikes differently to inform a new marketing strategy. Using historical trip data from December 2024 to November 2025, the analysis reveals distinct behavioral patterns: Annual Members use the service for daily commuting, while Casual Riders use it primarily for weekend leisure. The recommended strategy focuses on converting casual riders by targeting their weekend usage habits and seasonal riding patterns.

## 2. Business Task
Cyclistic has concluded that annual members are more profitable than casual riders. The Director of Marketing believes the company’s future growth depends on maximizing the number of annual memberships.

**Objective:** Analyze historical bike trip data to understand the differences between casual riders and annual members.
**Primary Business Question:** How do annual members and casual riders use Cyclistic bikes differently?

## 3. Data Sources and Integrity
**Data Source:** 12 months of historical trip data (December 2024 – November 2025) provided by Motivate International Inc. under the Divvy Data License Agreement.
**Data Integrity:** The dataset initially contained 5.5 million records. Data processing was conducted in Python to ensure accuracy.
**Cleaning Steps:**
* Removed trips with duration less than 60 seconds (potential false starts or docking errors).
* Removed trips with negative ride durations.
* Removed records with missing station names or timestamps.
* **Final Sample Size:** 4.8 million clean rows were used for the analysis.

## 4. Analysis and Key Findings

### Finding 1: Usage by Day of Week
There is a fundamental difference in when the two groups ride. Casual ridership peaks significantly on Saturdays and Sundays, often double their weekday volume. In contrast, Annual Members show consistent, high usage Monday through Friday.

**Conclusion:** Casual riders are "Weekend Warriors" using the service for leisure, whereas Members are utilizing the bikes for reliable weekday transportation.

![Weekly Usage](../03_Visualizations/weekly_usage.png)

### Finding 2: Usage by Hour of Day
Hourly data confirms the commuting hypothesis. Annual Members exhibit two distinct usage spikes at 8:00 AM and 5:00 PM (17:00), aligning with standard business hours. Casual riders show a gradual increase in activity throughout the day, peaking in the late afternoon (3:00 PM – 5:00 PM) without a morning spike.

**Conclusion:** Members are using bikes to commute to work or school. Casual riders are likely avoiding rush hour traffic and riding for recreation.

![Hourly Heartbeat](../03_Visualizations/hourly_heartbeat.png)

### Finding 3: Seasonal Trends
Both groups ride more frequently in the summer months. However, casual ridership is highly elastic based on season; it drops near zero in the winter months (December–February). Annual Members maintain a baseline level of activity throughout the winter.

**Conclusion:** Casual riders are weather-sensitive. Members rely on the service year-round, further supporting the evidence that it is their primary mode of transport.

![Seasonality](../03_Visualizations/seasonality_fixed.png)

## 5. Recommendations
Based on the data-driven insights above, the following three strategies are recommended to convert casual riders into annual members:

1.  **Launch a "Weekend Warrior" Membership Upgrade**
    Since casual riders are already heavy users on weekends, target them with a campaign specifically highlighting the cost savings of membership for weekend-only riding. Push notifications sent on Friday afternoons or Saturday mornings could be effective.

2.  **Introduce a Seasonal "Warm Weather" Pass**
    Data shows casual riders disappear in winter. A full annual membership is a hard sell for a user who only rides from May to September. Creating a 6-month seasonal pass (priced slightly higher per month than an annual plan) would capture this market segment.

3.  **Offer Leisure-Specific Member Benefits**
    Casual riders value leisure time over speed. The current membership model is designed for short commutes (often capped at 30 minutes). Offering members extended ride times (e.g., 45–60 minutes) on weekends would add specific value to the casual user's primary use case.
