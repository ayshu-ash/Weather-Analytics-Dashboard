# Weather-Analytics-Dashboard

## Project Overview
This project is an End-to-End Power BI solution that transforms live data from WeatherAPI.com into an executive-level monitoring tool. It provides a real-time, consolidated view of global weather conditions, 72-hour forecasts, and critical air quality metrics for cities like Dubai, London, Mumbai, New York and Toronto.

## 📊 Dashboard Preview
![Weather Dashboard](Screenshots/Dashboard.png)

## Business Problem
Decision-makers often struggle with weather data because it is:

 * Scattered: Spread across multiple apps and websites.
   
 * Unstructured: Delivered in complex, "raw" formats (JSON).
   
 * Reactive: Focused on "what happened" rather than "what is coming."
   
**The Solution:** This dashboard acts as a Centralized Intelligence Hub, turning complex data into a simple, 3-day visual story for immediate risk assessment.

## Data Source
   ### Primary Source:  
   * WeatherAPI.com 
   ### Data Processing:
   * API connection in Power BI.
   * JSON expansion using Power Query.
   * Data cleaning and column formatting.
   * Structured relational modeling.

# Technical Architecture
I utilized a Multi-Fact Star Schema to ensure the dashboard remains fast and accurate across different levels of detail.

 * **Central Dimension:** Location (Master city list for dynamic filtering).

 * **Fact Tables:**
   
   * **Current:** Real-time atmospheric observations.

   * **Forecast_Day:** 3-day trend summaries.

   * **Forecast_Hour:** Granular 24-hour time-series data.

**Relationship Logic:** One-to-Many relationships ensure that city filters flow correctly across all visuals without data inflation.

# Key Features & KPIs
 **1. Real-Time Monitoring**
 
    * Core Metrics: Live Temperature (°C), Humidity, Wind Speed (Kph), and Pressure.

    * Visibility & UV Index: Safety indicators for transportation and outdoor planning.

2. 72-Hour Forecast Analytics
Temperature Trends: Visual line charts showing short-term fluctuations.

Chance of Rain: Probability-based bars (0–100%) for proactive scheduling.

3. Environmental Health (AQI)
Diagnostic Tracking: Real-time monitoring of PM2.5, PM10, CO, and NO₂.

Status Gauge: Instant color-coded categorization (Good / Moderate / Unhealthy).

# Key Insights
   The dashboard delivers multiple layers of insight:
   * Trend Analysis – Identifies short-term temperature movement patterns.
   * Comparative Analysis – Enables cross-city environmental evaluation.
   * Real-Time Monitoring – Tracks live weather and AQI conditions.
   * Predictive Insight – Highlights high-probability rainfall periods.
   * Diagnostic Insight – Identifies dominant pollutants impacting AQI levels.
This solution converts raw weather data into actionable environmental intelligence.

# Business Applications
   * Environmental monitoring and public health awareness.
   * Logistics and route planning based on weather conditions.
   * Outdoor event and travel planning using rainfall forecasts.
   * Risk assessment for extreme weather exposure.
   * Energy demand and infrastructure planning based on temperature patterns.
   * This dashboard demonstrates how environmental data can support operational and planning decisions.
The dashboard demonstrates how environmental data can support operational and strategic decision-making.

# Tools & Technologies Used
   * **Visualization:** Power BI Desktop
   * **Data Ingestion:** REST API (WeatherAPI)
   * **Transformation:** Power Query (M)
   * **Calculations:** DAX (Data Analysis Expressions)
   * **Modeling:** Dimensional Star Schema

# Technical Strengths Demonstrated
   * API-driven data ingestion.
   * JSON normalization and transformation.
   * Dimensional modeling design.
   * Multi-granularity reporting.
   * KPI development using DAX.
   * Insight-focused dashboard storytelling.
