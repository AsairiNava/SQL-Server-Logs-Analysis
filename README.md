# Logs Analysis with DuckDB

## Overview
- This project performs exploratory analysis on system logs using DuckDB directly over JSON files  
- The goal is to extract insights about traffic patterns, performance, and system reliability  
- The analysis is focused on generating actionable recommendations for the development team  

## Problem Statement
- Modern systems generate large volumes of logs across multiple services  
- Analyzing these logs is critical to identify performance bottlenecks and errors  
- The objective is to transform raw logs into meaningful insights for decision-making  

## Tech Stack
- Python  
- DuckDB  
- Pandas  
- Google Colab / Jupyter Notebook  

## Dataset
- The dataset consists of multiple JSON files representing different system entities  
- access_logs: user requests  
- error_logs: system errors  
- alerts: triggered alerts  
- services: service metadata  
- servers: infrastructure data  
- incidents: incident tracking  
- performance_metrics: system performance data  

## Data Loading
- JSON files are loaded into DuckDB as separate tables  
- DuckDB reads JSON files directly without preprocessing  
- Each file is converted into a relational table for analysis  

## Exploratory Analysis
- Total number of requests analyzed  
- Time range of the dataset  
- Number of unique users  
- Number of unique endpoints  
- Distribution of requests across endpoints  
- Error frequency across services  
- General traffic and usage patterns  

## Key Insights
- A small number of endpoints concentrate a large portion of total traffic  
- Certain endpoints show signs of higher latency or potential bottlenecks  
- User activity is unevenly distributed across the system  
- Some services present recurring error patterns  

## Recommendations
- Optimize high-latency endpoints by implementing caching and improving database query performance  
- Improve scalability for high-traffic endpoints through load balancing and rate limiting  
- Enhance error monitoring by adding alert thresholds and improving logging and debugging processes  

## How to Run
- Clone the repository  
- Install dependencies:

- Open the notebook in Jupyter or Google Colab  
- Execute all cells to reproduce the analysis  

## Why DuckDB
- Enables SQL queries directly on JSON files  
- Provides fast analytical performance without requiring a server  
- Integrates seamlessly with Python workflows  

## Future Improvements
- Build dashboards using Power BI or Tableau  
- Implement anomaly detection on logs  
- Automate the data pipeline  
- Integrate real-time data sources  

## Author
- Asairi Nava  
- Data Analyst | BI | Analytics Engineering  
