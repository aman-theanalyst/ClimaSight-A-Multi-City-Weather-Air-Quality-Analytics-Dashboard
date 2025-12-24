# 🌦️ ClimaSight: Multi-City Weather & Air Quality Analytics Dashboard

![Dashboard Preview](Images/ClimaSight%20Dashboard.png)

## 📊 Project Overview

**ClimaSight** is an interactive **Power BI dashboard** designed to deliver comprehensive **weather and air quality analytics** across multiple cities. The project integrates real-time weather data with air quality indicators to provide actionable environmental insights through intuitive and visually rich dashboards.

This project showcases strong capabilities in **data integration, transformation, modeling, and visualization**, making it suitable for real-world environmental analytics and decision-support use cases.

🔗 **Live Dashboard**: [View Dashboard](your-dashboard-link-here)

---

## 🎯 Business Objective

To build a centralized analytics platform that enables users and stakeholders to:

- Monitor real-time weather conditions across multiple cities
- Track air quality indicators (AQI & pollutants) for health and environmental assessment
- Analyze 7-day weather forecast trends for planning and operations
- Support data-driven decisions using environmental data insights

---

## 🔑 Key Features

### 🌤️ Weather Analytics
- Real-time temperature with *feels-like* conditions
- 7-day weather forecast with trend visualization
- Multi-city comparison (Bangalore, Ajmer, Hyderabad)
- Key meteorological metrics:
  - Humidity (%)
  - Wind Speed (Kph)
  - Visibility (KM)
  - Atmospheric Pressure (mm)
  - UV Index
  - Precipitation (mm)

### 🌫️ Air Quality Monitoring
- Real-time **Air Quality Index (AQI)**
- Pollutant-level tracking:
  - PM10
  - PM2.5
  - O₃ (Ozone)
  - SO₂ (Sulfur Dioxide)
  - CO (Carbon Monoxide)
  - NO₂ (Nitrogen Dioxide)
- Color-coded health indicators (Good / Moderate / Unhealthy)

### ⏰ Additional Features
- Sunrise & sunset timings
- Rain probability (7-day)
- Last updated timestamp for data freshness

---

## 🛠️ Technical Stack

| Component | Technology |
|---------|------------|
| Data Source | WeatherAPI.com (REST API) |
| Data Integration | Power Query (M Language) |
| Visualization | Microsoft Power BI |
| Data Modeling | DAX |
| Deployment | Power BI Service |
| Refresh | Scheduled (Hourly) |

---

## 📈 Data Architecture

### Data Sources
- **Primary API**: WeatherAPI.com  
- **Endpoints Used**:
  - Current Weather API  
  - Forecast API  
  - Air Quality API  
  - Astronomy API  

### Data Flow
WeatherAPI → Power Query → Data Transformation → Data Model → Power BI Visuals


### Key Transformations
- API authentication & parameterization
- JSON parsing and flattening
- Data type normalization
- Derived metric calculations
- Time zone standardization

---

## 📊 Key Insights & Analysis (Data as per 24 dec,2025 at Kotdwara)

### Weather Insights
- Cool winter conditions at **12.2°C** with sunny skies
- Stable temperature pattern (14.3°C - 15.2°C range)
- Moderate humidity (**57%**) with sunny conditions
- Very low precipitation (**0.01 mm**)
- Low UV Index of **0.5** – safe for outdoor activities
- Visibility up to **10 KM**

### Air Quality Insights
- **Satisfactory** overall (**AQI 69**) but with concerns
- PM10 & PM2.5 both elevated (yellow zone) - winter dust/agricultural activity
- 🚨 Critical CO Alert: 813 (red zone) - serious concern requiring investigation
    - Likely sources: vehicular emissions, biomass burning, industrial activity
- Positive: O3, NO2, SO2 all in healthy green zone

### City Comparison
- **Kotdwara** (12.2°C) - Coolest, foothill climate
- **Kolkata** (17.1°C) - Coastal warming
- **Guwahati** (19.3°C) - Subtropical influence
---

## 🚀 Implementation Workflow

### Phase 1: Data Connection
- API key generation and Web connector setup
- Parameterized city selection

### Phase 2: Data Transformation
- JSON parsing using Power Query
- Separate queries for weather, forecast & AQI
- Table relationships creation

### Phase 3: Data Modeling
- Calendar table creation
- DAX measures for:
  - AQI status
  - Temperature trends
  - Aggregations

### Phase 4: Visualization
- Dark theme UI
- Custom visuals:
  - AQI Gauge
  - Forecast line charts
  - KPI cards
- Interactive slicers & filters

### Phase 5: Deployment
- Published to Power BI Service
- Hourly scheduled refresh

---

## 📁 Project Structure

ClimaSight/
│    
├── Dataset/    
│   ├── Current.xlsx    
│   ├── Forecast_by_Day.xlsx    
│   ├── Forecast_by_Hour.xlsx    
│   └── Master_Table.xlsx    
│    
├── Icons/     
│    
├── Images/    
│   └── dashboard-preview.png    
│    
├── Power BI/   
│   └── ClimaSight.pbix    
│     
└── README.md    
        

### 🔄 Data Refresh Schedule
- Refresh Frequency: Every 1 hour
- Data Retention: 30 days historical data
- API Call Limits: 1,000,000 calls/month (free tier)

---

## 🔮 Future Enhancements
- Historical weather analysis
- Predictive modeling (ML integration)
- Mobile-optimized dashboard
- Alert & notification system
- Expansion to 30+ cities

---

## 🙏 Acknowledgments
- WeatherAPI.com
- Microsoft Power BI Community
---

## 📞 Contact
    
Developer: Aman Singh Negi   
📧 Email: theanalyst.aman@gmail.com     
🔗 LinkedIn: https://linkedin.com/in/aman-singh-negi-482197310   
