# strava-weather-pipeline

David Wong's premiere personal project for Fall 2025 Co-op Job Search.

This project demonstrates modern data engineering and analytics practices by building a full-stack pipeline using **Strava running data** and **weather data**. The architecture follows the **medallion architecture (Bronze → Silver → Gold)** and includes API ingestion, data modeling, analytics, and machine learning components — all built using **free and open-source tools**.

---

## 🚀 Objectives

- Showcase skills relevant to **Data Engineering**, **Data Architecture**, **Data Analytics**, and **Consulting** roles.
- Build a fully automated data pipeline using **real-world APIs**.
- Apply the **medallion architecture** for data quality and modularity.
- Generate downstream use cases: analytics, dashboards, and predictive models.

---

## 🏗️ Project Phases

### 🔸 1. Data Pipeline Engineering

**BRONZE Layer** – _Raw Ingestion_

- Automate API calls to:
  - [Strava API](https://developers.strava.com/) for running activity data
  - [OpenWeatherMap API](https://openweathermap.org/api) for historical weather data
- Store responses in raw JSON/CSV format
- Schedule and log jobs for reproducibility

**SILVER Layer** – _Data Cleaning and Modeling_

- Normalize raw data into clean tables
- Design a relational schema (PostgreSQL or SQLite)
- Join activity and weather data by location and timestamp
- Perform feature engineering for analytics and ML

**GOLD Layer** – _Analytics and Insights_

- Denormalize key tables for fast access
- Build visual dashboards (e.g. Streamlit, Power BI)
- Create ML models to predict running pace or effort based on conditions

---

## 📊 Phase 2: Data Analytics

- 📈 **Dashboards**: Analyze run performance trends over time, by route, temperature, or pace
- 🧠 **Machine Learning**:
  - Predict pace from weather, distance, and terrain
  - Cluster runs by effort level or run type
  - Recommend optimal conditions or training patterns

---

## 🧰 Tech Stack

| Layer          | Tools & Technologies                                    |
| -------------- | ------------------------------------------------------- |
| Data Ingestion | Python, Requests, OAuth, Strava API, OpenWeatherMap API |
| Storage        | JSON, CSV, SQLite or PostgreSQL                         |
| Processing     | pandas, SQLAlchemy, dbt (optional), Jupyter             |
| Analytics      | Streamlit / Power BI / Plotly                           |
| ML (optional)  | scikit-learn, XGBoost, NumPy                            |
| Orchestration  | Python scripts, cron (optional), Prefect (optional)     |
| Deployment     | GitHub, GitHub Actions (optional for automation)        |

---

## 📁 Repository Structure

```
strava-weather-pipeline/
├── bronze/ # Raw ingested data (JSON/CSV from APIs)
├── silver/ # Cleaned, validated, and normalized data
├── gold/ # Denormalized tables ready for analysis and ML
├── notebooks/ # Jupyter notebooks for EDA, prototyping, ML
├── scripts/ # Python scripts for ingestion, transformation, and modeling
├── README.md # Project documentation
├── requirements.txt # Python dependencies
└── .gitignore # Exclude data, API keys, etc.
```

---

## 📅 Timeline (Target Completion: ~2 Months)

| Week  | Milestone                                              |
| ----- | ------------------------------------------------------ |
| 1–2   | ✅ API setup, data ingestion (Bronze)                  |
| 3–5   | 🔄 Cleaning, relational modeling (Silver)              |
| 6–8   | ⏳ Dashboards, ML, and insights (Gold)                 |
| Final | 🧹 Final polish, README, blog post, and portfolio prep |

---

## ✍️ Author

**David Wong**  
Aspiring Data Engineer / Analyst / Consultant  
📍 Waterloo, Canada  
📧 d78wong@uwaterloo.ca  
🌐 [David Wong's LinkedIn](https://www.linkedin.com/in/david-wong02)

---

## 📌 Status

**🚧 In Progress** – Currently building out the **Bronze layer**.

Follow progress in:

- GitHub Issues (task tracking)
- GitHub Projects (Kanban board)

---

## 🤝 Contributions

Thank you to running friends who have willingly provided their Strava running data, free of cost.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).  
You are free to fork and adapt for educational purposes.

---
