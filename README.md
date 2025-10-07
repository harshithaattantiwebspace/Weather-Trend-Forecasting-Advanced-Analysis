# Global Weather Forecasting & Climate Analysis

## 🎯 Project Overview  
This repository contains a comprehensive data science project that analyzes global weather data to uncover climate patterns, detect anomalies, and forecast future temperature trends.  
The analyses include:  
- Advanced EDA (distributions, correlations, anomaly detection)  
- Spatial and geographical pattern exploration  
- Forecasting via multiple models and an ensemble  
- Unique analyses including climate trends, environmental impact, and feature importance  

This project aligns with the **PM Accelerator mission** by demonstrating how data and AI tools can be universally accessible and used to generate impactful insights.  

---

## 🧭 PM Accelerator Mission  
> “By making industry-leading tools and education available to individuals from all backgrounds, we level the playing field for future PM leaders. This is the PM Accelerator motto, as we grant aspiring and experienced PMs what they need most – Access. We introduce you to industry leaders, surround you with the right PM ecosystem, and discover the new world of AI product management skills.”  
>  
> PM Accelerator is committed to empowering aspiring and experienced Product Managers through quality education, real-world opportunities, and a supportive community. In line with this mission, we also extend our support to disadvantaged youths through PMA Kids – fostering the next generation of leaders and innovators.

---


## 🧰 Methodology & Workflow

### 1. **Data Loading & Cleaning**  
- Loaded the *Global Weather Repository* dataset (≈ 98,000 rows, 41 features).  
- Parsed datetime, removed duplicates, filled missing numeric values via interpolation.  
- Applied IQR-based outlier clipping to reduce extreme noise.  

### 2. **Advanced EDA**  
- Explored distributions (temperature histogram), correlations (weather vs air quality),  
- Detected anomalies globally (IQR method), visualized on world maps,  
- Assessed environmental relationships (temperature ↔ PM2.5, humidity effects).  

### 3. **Forecasting Models**  
- Developed three forecasting approaches: ARIMA, Prophet, and XGBoost.  
- Generated predictions on a holdout test set.  
- Constructed an ensemble (average of model outputs) to improve robustness.  
- Evaluated using MAE and RMSE metrics.  

### 4. **Unique Analyses**  
- **Climate Trends**: Ranked hottest countries, visualized warming trends.  
- **Geographical Patterns**: Compared weather metrics across continents.  
- **Feature Importance**: Trained a Random Forest or XGBoost model to find key predictors of temperature.  
- **Spatial Analysis**: Mapped anomalies and weather extremes geographically.  

---

## 📊 Key Results & Insights

- **Top Hot Regions**: Saudi Arabia, Morocco, Turkmenistan, and parts of India rank highest in average temperature.  
- **Anomalies**: ≈12% of locations flagged as temperature or pollution outliers, mostly in arid and tropical zones.  
- **Environmental Coupling**: Positive linkage between temperature and PM2.5; humidity inversely correlated with pollutants.  
- **Feature Importance**: Pressure and humidity were strongest predictors of temperature; particulate measures played a secondary role.  
- **Forecasting**: ARIMA yielded a stable baseline; ensemble of ARIMA + Prophet + XGBoost provided most balanced accuracy and adaptability.

---



