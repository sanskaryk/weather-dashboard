# 🌦️ Weather Forecast Analytics Dashboard (Power BI)
Live Dashboard - https://bit.ly/4azENYj

## 📌 Project Overview

This project is a dynamic Weather Forecast Analytics Dashboard built using **Microsoft Power BI**.  
It fetches real-time weather and forecast data from a Weather API and visualizes:

- 🌡️ Current weather conditions
- 📅 Daily forecast
- ⏰ Hourly forecast
- 🌍 Multi-city comparison

The dataset is automatically refreshed in Power BI Service to always display the latest available weather data.

<img width="1006" height="581" alt="weather_dashboard" src="https://github.com/user-attachments/assets/2584e9fb-c908-403e-8f37-05dec9e32d49" />

---

## 🏗️ Project Architecture

The data model is structured into the following tables:

### 1️⃣ Weather Reports (Per City)
Raw API responses collected for multiple cities.

### 2️⃣ Current
Contains:
- Location details
- Current temperature
- Wind
- Humidity
- UV index
- Air pressure
- Other real-time metrics

### 3️⃣ Forecast_Day
Contains:
- Location details
- Forecast date
- Daily max/min/avg temperature
- Weather condition
- Chance of rain
- Astro information (sunrise, sunset, moon phase)

### 4️⃣ Forecast_Hour
Contains:
- Location details
- Forecast date
- Hourly time
- Hourly temperature
- Wind
- Humidity
- Precipitation probability

---

## 🔄 Data Source

Data is fetched using a Weather API:

- API Type: REST
- Format: JSON
- Refresh Mode: Scheduled Refresh in Power BI Service

---

## 🔁 Automatic Refresh

The dataset is published to **Power BI Service** and configured with:

- Scheduled Refresh enabled
- Proper API credentials
- Time zone set to local region
- Relative date filtering to always display latest data

This ensures the dashboard updates automatically without manual intervention.

---

## 📊 Dashboard Features

- 🌍 City selection slicer
- 📈 Temperature trends
- 🌧️ Rain probability visualization
- 🌡️ Current vs Forecast comparison
- ⏳ Hourly weather breakdown
- 📅 Dynamic latest-date filtering

---

## 🛠️ Tools & Technologies

- Microsoft Power BI Desktop
- Power BI Service
- Power Query (M Language)
- DAX
- REST API (Weather Data)
- JSON Parsing

---

## 🚀 How to Use

1. Clone this repository.
2. Open the `.pbix` file in Power BI Desktop.
3. Replace the API key (if required).
4. Publish to Power BI Service.
5. Configure scheduled refresh.

---

## ⚠️ Notes

- API key limits may affect refresh frequency.
- Some fields may return null depending on API response.
- Time-based fields are handled carefully to avoid schema inconsistencies.

---

## 📌 Future Enhancements

- Historical weather comparison
- KPI cards for alerts
- Extreme weather detection
- Map-based weather visualization
- Forecast accuracy tracking

---

## 👤 Author

Sanskar Gupta

---

## 📄 License

This project is for academic and learning purposes.
