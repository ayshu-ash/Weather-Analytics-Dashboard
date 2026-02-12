## Weather-Analytics-Dashboard

### Project Overview
The Weather Analytics Dashboard is an interactive Power BI solution that integrates real-time and forecast weather data from WeatherAPI.com to deliver structured environmental insights across multiple global cities.
The dashboard consolidates fragmented weather and air quality data into a unified analytical interface, enabling real-time monitoring, trend analysis, and cross-city comparison for informed decision-making.
This project demonstrates API integration, dimensional data modeling, DAX-based KPI development, and analytical storytelling.

### Business Problem
Urban planners, logistics teams, event organizers, and public health stakeholders require consolidated environmental intelligence to make weather-informed decisions.
However, weather data is often:
    * Scattered across multiple platform.
    * Presented in raw, unstructured formats.
    * Lacking comparative and trend-based analysis.
This dashboard transforms API-driven environmental data into a structured, decision-support reporting solution.

### Data Source
   # Primary Source:  
        WeatherAPI.com 
   # Data Processing:
     * API connection in Power BI.
     * JSON expansion using Power Query.
     * Data cleaning and column formatting.
     * Structured relational modeling.

### Data Modeling Approach
The model follows a dimensional structure to support analytical reporting.
   # Tables
   
   # Dimension Table:
      * Location

   # Fact Tables
      * Current (1:1 relationship with Location)
      * Forecast_Day (Many-to-One relationship with Location)
      * Forecast_Hour (Many-to-One relationship with Location)

  # Design Rationale
     * Location acts as a central dimension enabling dynamic filtering.
     * Separation of Current and Forecast tables prevents grain conflicts between real-time and aggregated data.
     * Forecast_Day supports trend-level reporting.
     * Forecast_Hour enables granular drill-down analysis.
This structure supports:
     * Multi-granularity reporting.
     * Clean aggregation logic.
     * Scalable future enhancements (e.g., Date dimension)
     * Efficient KPI computation
The model aligns with star-schema best practices for BI reporting.

### KPIs & Metrics
# Weather Metrics
   * Current Temperature (°C)
   * Minimum & Maximum Temperature
   * Humidity (%)
   * Wind Speed (km/h)
   * Visibility (km)
   * Atmospheric Pressure (hPa)
   * UV Index
   * Total Precipitation (mm)

# Forecast Metrics
   * 7-Day Temperature Trend
   * Daily Chance of Rain (%)
   * Rain Probability Patterns

# Air Quality Metrics
   * Air Quality Index (AQI)
   * AQI Category (Good / Moderate / Unhealthy)
   * Pollutant Levels:
       PM2.5
       PM10
       CO
       NO₂
       SO₂
       O₃
All KPIs dynamically respond to selected city filters using relational modeling and DAX measures.

### Key Insights
   The dashboard delivers multiple layers of insight:
   * Trend Analysis – Identifies short-term temperature movement patterns.
   * Comparative Analysis – Enables cross-city environmental evaluation.
   * Real-Time Monitoring – Tracks live weather and AQI conditions.
   * Predictive Insight – Highlights high-probability rainfall periods.
   * Diagnostic Insight – Identifies dominant pollutants impacting AQI levels.
This solution converts raw weather data into actionable environmental intelligence.

### Business Applications
   * Environmental monitoring and public health awareness.
   * Logistics and route planning based on weather conditions.
   * Outdoor event and travel planning using rainfall forecasts.
   * Risk assessment for extreme weather exposure.
   * Energy demand and infrastructure planning based on temperature patterns.
   * This dashboard demonstrates how environmental data can support operational and planning decisions.
The dashboard demonstrates how environmental data can support operational and strategic decision-making.

### Tools & Technologies Used
   * Power BI Desktop
   * Power BI Service
   * WeatherAPI
   * Power Query (M)
   * DAX
   * Dimensional Data Modeling

### Technical Strengths Demonstrated
   * API-driven data ingestion.
   * JSON normalization and transformation.
   * Dimensional modeling design.
   * Multi-granularity reporting.
   * KPI development using DAX.
   * Insight-focused dashboard storytelling.
