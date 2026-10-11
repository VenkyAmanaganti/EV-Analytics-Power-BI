# ⚡ Electric Vehicle (EV) Analytics Dashboard | Power BI

## 📌 Project Overview

The **Electric Vehicle (EV) Analytics Dashboard** is a Power BI data analytics project designed to explore the electric vehicle market, vehicle performance, pricing, and customer-related characteristics.

The project uses interactive dashboards and data visualizations to analyze EV manufacturers, vehicle types, driving range, battery capacity, charging time, safety ratings, and pricing.

The objective is to transform raw EV data into meaningful insights that support data-driven analysis and decision-making.

## 🎯 Project Objectives

- Analyze the EV market across manufacturers and countries.
- Compare electric vehicles by type, price, and driving range.
- Evaluate technical performance, including top speed, acceleration, and efficiency.
- Analyze battery capacity and charging time.
- Explore vehicle safety ratings, seating capacity, and cargo space.
- Build interactive dashboards using Power BI slicers and visualizations.
- Identify data-quality issues and opportunities for improving analysis.

## 🛠️ Tools and Technologies

- **Power BI Desktop** — Dashboard development and data visualization
- **Power Query** — Data cleaning and transformation
- **DAX** — Measures and KPI calculations
- **CSV / Excel** — Data storage and preparation
- **GitHub** — Project documentation and version control

## 📊 Dashboard Pages

### 1. EV Market Dashboard

Provides an overview of the electric vehicle market.

**Key visualizations:**
- Total EV records
- Average vehicle price
- Average driving range
- Average battery capacity
- Average safety rating
- EVs by manufacturer
- Average price by vehicle type
- Price versus driving range
- EV distribution by country
- Release-year trends
- Average battery charging time

### 2. EV Technical & Performance Analysis

Focuses on the technical specifications and performance of electric vehicles.

**Key metrics:**
- Average top speed
- Average acceleration
- Average efficiency
- Average safety rating
- Average driving range

**Key visualizations:**
- Average efficiency by manufacturer
- Safety rating distribution
- Price versus driving range
- Interactive filters for country, manufacturer, vehicle type, drive type, and release year

### 3. Market & Pricing Analysis

Explores vehicle pricing and its relationship with other characteristics.

**Key visualizations:**
- Average vehicle price
- Minimum and maximum price
- Average driving range
- Safety rating distribution
- Average price by vehicle type
- Price versus range by manufacturer
- EV models by release year

**Interactive filters:**
- Country
- Manufacturer
- Vehicle type
- Release year

### 4. EV Customer & Safety Analysis

Examines vehicle characteristics related to safety, passenger capacity, and cargo space.

**Key metrics:**
- Average safety rating
- Average seats
- Average cargo space
- Average driving range

**Key visualizations:**
- Safety rating distribution
- Safety rating by manufacturer
- Seating capacity by vehicle type
- Cargo space by vehicle type

**Interactive filters:**
- Country
- Manufacturer
- Vehicle type
- Drive type
- Release year

## 🗂️ Dataset Description

The project uses `EV_dataset.csv`, containing **250,000 rows and 22 columns**.

Important fields include:

| Column | Description |
|---|---|
| `manufacturer` | EV manufacturer |
| `model` | Vehicle model |
| `type` | Vehicle category |
| `price_usd` | Vehicle price in USD |
| `battery_kwh` | Battery capacity in kWh |
| `range_km` | Driving range in kilometers |
| `charging_time_hr` | Charging time in hours |
| `top_speed_kmph` | Maximum speed in km/h |
| `efficiency_score` | Vehicle efficiency score |
| `safety_rating` | Vehicle safety rating |
| `seats` | Passenger seating capacity |
| `cargo_space_liters` | Cargo capacity in liters |
| `release_year` | Vehicle release year |
| `country` | Country associated with the record |
| `city` | City associated with the record |
| `drive_type` | Vehicle drivetrain category |
| `fuel_type` | Fuel or powertrain category |
| `fast_charging` | Fast-charging availability |
| `warranty_years` | Warranty duration in years |
| `target_high_efficiency` | High-efficiency classification |

## 📈 Skills Demonstrated

- Data analysis and exploratory data analysis
- Power BI dashboard development
- Data visualization and chart selection
- Data cleaning and transformation using Power Query
- DAX measures and KPI development
- Interactive reporting with slicers
- Comparative and trend analysis
- Data-quality validation
- Dashboard design and storytelling

## 🔍 Data Quality Considerations

Before drawing conclusions from the dashboard, the following checks should be performed:

- Validate missing values, duplicates, and invalid records.
- Investigate negative vehicle prices.
- Confirm whether each row represents a vehicle model, trim, or another observation.
- Use suitable aggregations, such as averages or counts, instead of sums where appropriate.
- Verify the meaning and scale of efficiency and safety scores.
- Ensure that chart titles, units, and KPI labels are clear and consistent.

These checks help improve the accuracy and reliability of the analysis.

## 🚀 How to Use This Project

1. Clone or download this GitHub repository.
2. Install [Microsoft Power BI Desktop](https://powerbi.microsoft.com/desktop/).
3. Open the `.pbix` Power BI report file.
4. If required, update the dataset source path in Power Query.
5. Refresh the data.
6. Explore the four dashboard pages using the interactive filters.

**Note:** The Power BI `.pbix` file and the CSV dataset must be included in the repository or provided separately for users to reproduce the dashboard. Screenshots alone do not provide an interactive report.

## 💡 Future Improvements

- Add year-over-year market analysis.
- Create a manufacturer ranking based on clearly defined metrics.
- Add advanced DAX measures and comparative KPIs.
- Improve tooltip pages and drill-through navigation.
- Add a dedicated data-cleaning and validation report.
- Publish the dashboard to Power BI Service, subject to access and licensing requirements.

## 👨‍💻 Author

**EV Analytics Power BI Project**

This project demonstrates practical data analytics and business intelligence skills using Power BI, Power Query, DAX, and interactive visualizations.

## ⭐ Feedback

If you find this project useful, consider starring the repository. Suggestions and feedback for improving the dashboard are welcome.
