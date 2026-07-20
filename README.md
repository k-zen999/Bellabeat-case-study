# BELLABEAT CASE STUDY

**Google Data Analytics Professional Certificate Capstone Project**

**Author: Zaina Khanum**



### Business Task Summary

**About the company**: Bellabeat is a high-tech manufacturer of beautifully designed smart health products targeted specifically at women.

**Business Objective**:  
Bellabeat aims to become a major player in the global smart device market. To achieve this, the marketing team wants to leverage consumer smart device usage data to uncover meaningful behavioral trends. These insights will help refine product features and shape more effective, data-driven marketing strategies.

**Key Guiding Questions**:
- What are the current trends in smart device usage?
- How can these trends be applied to Bellabeat’s existing and potential customers?
- What high-level recommendations can be made to influence Bellabeat’s marketing strategy?

**Role**: As a Junior Data Analyst on the Bellabeat marketing team, this analysis focuses on transforming raw Fitbit usage data into actionable marketing intelligence.

### Data Sources

The analysis was conducted using the **Fitbit Fitness Tracker Data** publicly available on [Kaggle](https://www.kaggle.com/datasets/arashnic/fitbit).

**Dataset Details:**
- **Time Period**: March 12 – May 12, 2016 (split into two export folders)
- **Sample Size**: 30 eligible Fitbit users who consented to share their data
- **Data Type**: Daily, hourly, and minute-level activity, sleep, and weight logs

**Main Files Used:**
- `dailyActivity_merged.csv` — Primary file (steps, distance, calories, active minutes)
- `hourlySteps_merged.csv` — For hourly activity patterns
- `hourlyCalories_merged.csv` — For Calorie tracking

**Note**: The dataset is from 2016 and represents a small sample of Fitbit users. Limitations include potential sampling bias and short observation period.

## Data Cleaning & Manipulation

**Tools Used**: Microsoft Excel, Tableau

**Cleaning Steps:**
- Checked and removed duplicate rows (none found)
- Formatted `ActivityDate` column as proper Date type
- Removed invalid records where `TotalSteps = 0` and `Calories = 0` (5 rows removed — days device was not worn)
- Created two new calculated columns:
  - `DayOfWeek` using formula: `=TEXT(ActivityDate, "dddd")`
  - `TotalActiveMinutes` using formula: `=SUM(VeryActiveMinutes, FairlyActiveMinutes, LightlyActiveMinutes)`

Cleaned data was then imported into **Tableau Public** for analysis and visualization.

