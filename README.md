# ⚡ Electric Vehicle (EV) Analytics Dashboard

## EV Market, Technical Performance & Pricing Analysis

## 📌 Project Overview

This project analyzes Electric Vehicle (EV) data to understand market distribution, vehicle performance, pricing patterns, driving range, safety ratings, and customer-focused vehicle characteristics.

The goal is to explore differences between manufacturers and vehicle types, identify performance trends, compare pricing patterns, and transform raw EV data into actionable insights through an interactive Power BI dashboard.

The project contains four dashboard pages covering market analysis, technical performance, market pricing, and customer & safety analysis.

## 🎯 Business Task

Analyze electric vehicle data to answer key business questions:

- Which manufacturers and vehicle types are represented in the dataset?
- How do EV driving range, efficiency, speed, and acceleration compare?
- How does average vehicle price vary by vehicle type and manufacturer?
- What relationships exist between price, driving range, and performance?
- How do safety ratings, seating capacity, and cargo space vary across vehicle categories?
- How can interactive filters help users explore EV market segments?

## 🛠️ Tools Used

- **Microsoft Excel** — Data inspection and preparation
- **Microsoft Power BI** — Interactive dashboard development and visualization
- **DAX** — KPI calculations and analytical measures
- **Power Query** — Data transformation and cleaning
- **GitHub** — Project documentation and portfolio presentation

## 📂 Dataset

**Source:** EV Dataset (`EV_dataset.csv`)

The dataset contains information about electric vehicles, including manufacturer, model, pricing, performance, vehicle specifications, and geographical attributes.

### Dataset Information

| Metric | Details |
|---|---|
| Total Records | 250,000 |
| Total Columns | 22 |
| Manufacturer | Vehicle manufacturer |
| Model | Vehicle model name |
| Price | `price_usd` |
| Driving Range | `range_km` |
| Battery Capacity | `battery_kwh` |
| Charging Time | `charging_time_hr` |
| Efficiency Score | `efficiency_score` |
| Safety Rating | `safety_rating` |
| Cargo Space | `cargo_space_liters` |
| Seating Capacity | `seats` |
| Release Year | `release_year` |

*Note: Record counts and field names reflect the supplied dataset. Confirm the dataset's original source and licensing before redistribution.*

## 🧹 Data Preparation

The dataset was used to build a structured Power BI report with fields for vehicle characteristics, performance, pricing, and geographical analysis.

Key preparation and validation activities include:

- Reviewing column names and data types.
- Checking missing values and duplicate records.
- Validating numeric fields such as price, battery capacity, range, and safety rating.
- Checking for invalid values, including negative prices.
- Preparing categorical fields for manufacturer, country, vehicle type, and drive type analysis.
- Creating or configuring measures for dashboard KPI cards.
- Organizing fields for charts, slicers, and interactive filtering.

**Data quality note:** Validate the negative minimum price displayed on the Market & Pricing page before using it in business conclusions.

## 📊 Dashboard Overview

The Power BI report contains four interactive pages.

### 1. ⚡ Electrical Vehicle Market Dashboard

Provides a high-level overview of the EV dataset and its market characteristics.

**Visualizations:**
- EVs by Manufacturer
- Average Price by Vehicle Type
- Price vs. Range
- EVs by Release Year
- EV Distribution by Country
- Average Battery Charging Time

**Key KPIs:**
- Total EV Records
- Average Price
- Average Range
- Average Battery Capacity
- Average Safety Rating

**Purpose:** Understand the overall dataset, compare manufacturers, and explore geographical and vehicle-category patterns.

### 2. 🔋 EV Technical & Performance Analysis

Focuses on vehicle specifications and performance indicators.

**Visualizations:**
- Average Efficiency by Manufacturer
- Safety Rating Distribution
- Price vs. Driving Range

**Key KPIs:**
- Average Top Speed
- Average Acceleration
- Average Efficiency
- Average Safety Rating
- Average Range

**Interactive Filters:**
- Country
- Manufacturer
- Vehicle Type
- Drive Type
- Release Year

**Purpose:** Compare vehicle performance and examine differences between manufacturers and market segments.

### 3. 💰 Market & Pricing Analysis

Explores EV pricing patterns and their relationship with vehicle characteristics.

**Visualizations:**
- Safety Rating Distribution
- Average Price by Vehicle Type
- Price vs. Range by Manufacturer
- EV Models by Release Year

**Key KPIs:**
- Average Price
- Minimum Price
- Maximum Price
- Average Driving Range

**Interactive Filters:**
- Country
- Manufacturer
- Vehicle Type
- Release Year

**Purpose:** Compare pricing across vehicle categories and investigate potential relationships between price and driving range.

### 4. 🛡️ EV Customer & Safety Analysis

Examines vehicle characteristics relevant to passenger capacity, storage, and safety.

**Visualizations:**
- Safety Rating Distribution
- Safety Rating by Manufacturer
- Seating Capacity by Vehicle Type
- Cargo Space by Vehicle Type

**Key KPIs:**
- Average Safety Rating
- Average Seats
- Average Cargo Space
- Average Range

**Interactive Filters:**
- Country
- Manufacturer
- Vehicle Type
- Drive Type
- Release Year

**Purpose:** Help users compare vehicle specifications and explore safety-related metrics across manufacturers and vehicle categories.

## 📈 Key Analytical Findings

The dashboard provides a foundation for investigating the following areas:

**Finding 1: Manufacturer and Market Coverage**

Manufacturer and country visuals help identify which brands and geographical markets are represented in the dataset.

**Finding 2: Performance Comparisons**

Range, efficiency, top speed, and acceleration measures can be compared across manufacturers to identify differences in vehicle specifications.

**Finding 3: Pricing Differences**

Comparing average prices by vehicle type helps explore potential price differences between sedans, SUVs, hatchbacks, coupes, trucks, and crossovers.

**Finding 4: Price and Driving Range**

Scatter plots allow users to investigate whether vehicles with higher prices also tend to have greater driving ranges.

**Finding 5: Practical Vehicle Characteristics**

Seating capacity and cargo space comparisons help users understand differences in vehicle utility across categories.

*These are analytical directions supported by the dashboard design, not independently verified conclusions. Validate the underlying measures and data before reporting specific rankings or relationships.*

## 💡 Recommendations

### 1. Improve KPI Accuracy

Use explicit DAX measures and confirm whether each KPI should use an average, sum, count, minimum, or maximum.

### 2. Investigate Price and Range Relationships

Compare price and driving range by manufacturer and vehicle type. Consider median values and outliers to avoid misleading comparisons.

### 3. Validate Data Quality

Investigate negative prices, missing values, duplicates, and unexpected numeric values before publishing the report.

### 4. Improve Dashboard Readability

Use consistent titles, units, colors, number formats, and axis labels across all four pages.

### 5. Use Interactive Filtering

Combine country, manufacturer, vehicle type, drive type, and release-year filters to make comparisons more meaningful.

## 🧮 Example DAX Measures

The following are example measures you can adapt to your Power BI table name and business requirements.

**Total EV Records**

```dax
Total EVs = COUNTROWS(EV_dataset)
```

**Average EV Price**

```dax
Average Price = AVERAGE(EV_dataset[price_usd])
```

**Average Driving Range**

```dax
Average Range = AVERAGE(EV_dataset[range_km])
```

**Average Battery Capacity**

```dax
Average Battery Capacity = AVERAGE(EV_dataset[battery_kwh])
```

**Average Safety Rating**

```dax
Average Safety Rating = AVERAGE(EV_dataset[safety_rating])
```

*Ensure `EV_dataset` matches the actual table name in your Power BI model.*

## 📁 Project Structure

A suggested GitHub repository structure is:

```text
EV-Analytics-PowerBI/
│
├── README.md
├── EV_dataset.csv
├── EV_Analytics_PowerBI_Project.pbix
│
├── screenshots/
│   ├── market-dashboard.png
│   ├── technical-performance.png
│   ├── market-pricing.png
│   └── customer-safety.png
│
└── dax-measures.md
```

*Add only files you have available. Avoid committing sensitive information or unnecessarily large datasets.*

## 🚀 How to Use the Project

1. Clone or download this repository.
2. Open `EV_Analytics_PowerBI_Project.pbix` in Microsoft Power BI Desktop.
3. If necessary, update the dataset path in Power Query.
4. Refresh the data model.
5. Review the DAX measures and verify their aggregations.
6. Explore the four dashboard pages.
7. Use the slicers to compare manufacturers, vehicle types, countries, drive types, and release years.

## 🎓 Skills Demonstrated

- Data analysis and exploratory analysis
- Data cleaning and validation
- Power Query transformations
- DAX measures and KPI development
- Data visualization and dashboard design
- Comparative and trend analysis
- Interactive reporting with slicers
- Data storytelling and business recommendations
- Project documentation using GitHub

## 🏁 Conclusion

The EV Analytics Dashboard brings together market, technical performance, pricing, and customer-focused vehicle characteristics in one interactive Power BI report.

By combining KPI cards, comparative charts, scatter plots, geographical visuals, and slicers, the project provides a practical way to explore EV data and investigate questions about vehicle performance, price, range, safety, and utility.

The next step is to validate the underlying measures and data quality, then document verified insights from each dashboard page.

## 👤 About Me

I'm an aspiring Data Analyst from India, building my portfolio through practical projects using Excel, SQL, Power BI, and data visualization.

This project demonstrates my ability to transform a dataset into an interactive dashboard and communicate analytical questions, findings, and recommendations.

🔗 **LinkedIn:** [https://www.linkedin.com/in/amanaganti-venkateswarlu-520404200]

🔗 **GitHub:** [https://github.com/VenkyAmanaganti]

---

*This project is intended for educational and portfolio purposes. Verify dataset provenance and licensing before sharing the source data publicly.*
