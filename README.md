# Uber-Data-Dashboard
# 🚕 Uber Ride Bookings Analysis — NCR Dashboard

An end-to-end data analytics project that cleans, analyzes, and visualizes ~150,000 Uber ride bookings from the National Capital Region (NCR). The pipeline goes from raw CSV → Python cleaning/EDA → MySQL database → Power BI dashboard.

## 📊 Dashboard Preview
![Dashboard](Dasboard.gif)

## 🔧 Tech Stack
- **Python** (Pandas, NumPy, Matplotlib, Seaborn) — data cleaning, feature engineering, EDA
- **MySQL** (SQLAlchemy) — structured storage for querying
- **Power BI** — interactive dashboard & visualization

## 📁 Project Workflow
1. **Data Cleaning** — removed formatting issues (quoted IDs), merged Date/Time into a single datetime column
2. **Feature Engineering** — derived Year, Month, Weekday, Hour, and time-slot features for trend analysis
3. **Missing Value Handling** — logical imputation for operational metrics (VTAT, CTAT, Ride Distance)
4. **Exploratory Data Analysis** — booking status distribution, cancellation rates by vehicle type, and more
5. **Database Load** — cleaned data pushed to MySQL via SQLAlchemy for SQL-based analysis
6. **Dashboard** — key business KPIs (bookings, cancellations, ratings, revenue) visualized in Power BI

## 📂 Files
| File | Description |
|---|---|
| `Uber_Project.ipynb` | Full Python notebook: cleaning, feature engineering, EDA, MySQL load |
| `ncr_ride_bookings.csv` | Raw dataset (NCR ride bookings) |
| `uber_bookings_cleaned.csv` | Cleaned dataset ready for SQL/Power BI |
| `Dasboard.gif` | Preview of the Power BI dashboard |

## 📈 Key Insights
- Analyzed booking status distribution (completed, cancelled, incomplete)
- Identified cancellation trends by vehicle type and time of day
- Tracked ride volume, average ratings, and revenue patterns across time

## 🚀 How to Run
1. Clone the repo
2. Install dependencies: `pip install pandas numpy matplotlib seaborn sqlalchemy mysql-connector-python`
3. Run `Uber_Project.ipynb` to reproduce cleaning/EDA
4. Open the Power BI file (if included) to explore the dashboard
