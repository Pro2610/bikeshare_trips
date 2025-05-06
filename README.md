# 🚴 Ride the Data: Inside Austin’s Bikeshare Trends

## 🔍 Overview
This project analyzes bikeshare usage in Austin, Texas using real data from Google BigQuery.  
The goal was to uncover usage patterns, user behavior, and key operational metrics from 2013 to 2024.

## 🧰 Tools & Technologies
- 📌 BigQuery (SQL)
- 📊 Tableau (for dashboard visualization)
- 📁 Public dataset: `bigquery-public-data.austin_bikeshare.bikeshare_trips`

## 📈 Key Analyses
- **General Statistics**: total trips, average duration, number of stations
- **Monthly Dynamics**: how usage fluctuates by month
- **Top Starting Stations**: most frequently used starting points
- **Most Frequent Routes**: common station-to-station travel paths
- **User Behavior**: comparisons between Subscribers and Customers
- **Trip Duration Distribution**: time groups from short to long trips

## 🔎 Sample SQL Queries

```sql
-- Total trips and average duration
SELECT
  COUNT(*) AS total_trips,
  ROUND(AVG(duration_minutes), 2) AS avg_duration
FROM `bigquery-public-data.austin_bikeshare.bikeshare_trips`;


## 📄 Data Exports
Google Sheets with query results: https://docs.google.com/spreadsheets/d/1mtU-sdy5U5LOXHF7dPdBCL_Qs5H6OH4FXVghYn46rXA/edit?usp=sharing
