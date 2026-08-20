# 🌍 World-Wide Energy Consumption & Emission Analysis

## 📌 Project Overview

**World-Wide Energy Consumption & Emission Analysis** is a SQL-based data analysis project focused on understanding the relationship between **energy consumption, energy production, emissions, population, and economic growth** across countries and over time.

The project uses multiple datasets and SQL queries to perform comparative, trend, ratio, per-capita, and global-level analysis.

The analysis was performed using **MySQL**.

---

## 🎯 Objectives

* Analyze energy consumption and production across countries.
* Identify countries with the highest emissions.
* Study global emission trends over time.
* Compare energy production with consumption.
* Analyze the relationship between GDP and energy-related metrics.
* Examine the effect of population growth on emissions.
* Calculate energy consumption and production on a per-capita basis.
* Measure emission-to-GDP ratios.
* Analyze relationships between economic growth and energy production.
* Compare countries based on population, emissions, GDP, and energy metrics.

---

## 🛠️ Technologies Used

* **MySQL**
* **SQL**
* **MySQL Workbench**
* **CSV datasets**

### SQL Concepts Used

* `SELECT`
* `WHERE`
* `GROUP BY`
* `ORDER BY`
* `HAVING`
* `JOIN`
* `SUBQUERY`
* `CASE`
* Aggregate Functions
* Common Table Expressions (`CTE`)
* Window Functions
* `LAG()`
* `SUM()`
* `AVG()`
* `MAX()`
* `MIN()`
* `COUNT()`
* Mathematical calculations
* Correlation analysis

---

## 📊 Datasets

The project uses multiple datasets stored inside the **`Data_Sets`** folder.

| Dataset            | Purpose                             |
| ------------------ | ----------------------------------- |
| `country_3.csv`    | Country reference data              |
| `consum_3.csv`     | Energy consumption data             |
| `emission_3.csv`   | Energy-related emission data        |
| `gdp_3.csv`        | GDP data by country and year        |
| `production_3.csv` | Energy production data              |
| `population_3.csv` | Population data by country and year |

These datasets are connected using country and year information to perform cross-dataset analysis.

---

## 🗄️ Database Design

The SQL script first prepares and models the datasets by:

* Modifying column data types
* Renaming columns for consistency
* Creating a primary key for the country table
* Creating foreign-key relationships between the datasets
* Connecting consumption, emission, GDP, population, and production data through the country table

The `country_3` table acts as the central reference table for the other datasets.

---

## 🔍 Analysis Performed

### 1. General & Comparative Analysis

The project analyzes:

* Total emissions by country for the most recent year.
* Top 5 countries by GDP.
* Energy production vs. energy consumption.
* Energy balance by country and year.
* Energy types contributing the most to total emissions.

These queries use aggregations, joins, subqueries, grouping, and sorting.

---

### 2. Trend Analysis

The project examines changes over time, including:

* Year-over-year global emission changes.
* GDP trends for individual countries.
* Population growth and its relationship with emissions.
* Energy consumption trends for major economies.
* Year-over-year changes in energy consumption.

Window functions such as `LAG()` are used to calculate year-over-year changes.

---

### 3. Ratio & Per-Capita Analysis

Several efficiency and per-capita metrics were calculated, including:

* **Emission-to-GDP ratio**
* **Energy consumption per capita**
* **Energy production per capita**
* Changes in consumption over time

These calculations help compare countries with different population sizes and economic scales.

---

### 4. GDP & Energy Production Relationship

The project also analyzes the relationship between **GDP growth and energy production growth**.

A CTE is used to calculate growth rates, followed by a correlation calculation for each country. This helps examine whether economic growth and energy production growth move together.

---

### 5. Global Comparisons

The project performs global comparisons such as:

* Top 10 countries by population and their emissions.
* Countries with the largest reduction in emissions over time.
* Global average GDP, emissions, and population by year.

These analyses provide a broader view of global energy and environmental patterns.

---

## 🧠 Key SQL Techniques Demonstrated

### Joins

Multiple datasets are combined using `JOIN` operations based on country and year.

### Window Functions

`LAG()` is used to calculate:

* Year-over-year emission changes
* GDP changes
* Population growth
* Consumption changes
* Production growth

### Common Table Expressions

A CTE is used to calculate GDP and production growth before performing correlation analysis.

### Subqueries

Subqueries are used to identify:

* Most recent available year
* Top countries
* Minimum and maximum years
* Historical comparisons

### Aggregation

Functions such as `SUM()`, `AVG()`, `MAX()`, `MIN()`, and `COUNT()` are used extensively for analysis.

---

## 📁 Repository Structure

```text
World-Wide-Energy-Consumption-Emission-Analysis/
│
├── Data_Sets/
│   ├── consum_3.csv
│   ├── country_3.csv
│   ├── emission_3.csv
│   ├── gdp_3.csv
│   ├── population_3.csv
│   └── production_3.csv
│
├── project_sql.sql
├── SqlProject_PPT.pptx
├── ~$SqlProject_PPT.pptx
└── README.md
```

### File Description

| File                  | Description                                               |
| --------------------- | --------------------------------------------------------- |
| `Data_Sets/`          | Contains the datasets used for the analysis               |
| `project_sql.sql`     | Contains database modeling and SQL analysis queries       |
| `SqlProject_PPT.pptx` | Project presentation containing the analysis and findings |
| `README.md`           | Project documentation                                     |

> **Note:** `~$SqlProject_PPT.pptx` is a temporary Microsoft Office file and can be removed from the repository.

---

## 🚀 How to Run the Project

### 1. Clone the Repository

```bash
git clone https://github.com/GuruPreeth9903/World-Wide-Energy-Consumption-Emission-Analysis.git
```

### 2. Open MySQL Workbench

Create or select a MySQL database.

### 3. Load the CSV datasets

Import the files from the `Data_Sets` folder into MySQL.

### 4. Run the SQL Script

Open:

```text
project_sql.sql
```

Execute the queries sequentially.

The script includes both **database preparation/modeling** and the analytical queries.

---

## 📈 Project Highlights

This project demonstrates practical SQL skills in:

* Relational database modeling
* Data integration
* Data analysis
* Complex SQL querying
* Multi-table joins
* Window functions
* CTEs
* Subqueries
* Aggregation
* Time-series analysis
* Per-capita analysis
* Ratio analysis
* Correlation analysis
* Business-oriented insight generation

---

## 💡 Business & Analytical Questions Answered

Some of the key questions addressed in the project include:

* Which countries have the highest emissions?
* Which countries have the highest GDP?
* How does energy production compare with consumption?
* Which energy types contribute most to emissions?
* How have global emissions changed over time?
* How does population growth relate to emissions?
* What is the emission-to-GDP ratio for each country?
* How much energy is consumed per person?
* How much energy is produced per person?
* Is GDP growth related to energy production growth?
* Which countries have reduced emissions the most?
* How do population, GDP, and emissions change globally over time?

---

## 🎓 Skills Demonstrated

**SQL | MySQL | Data Analysis | Data Modeling | Data Cleaning | Joins | CTEs | Window Functions | Subqueries | Aggregations | Time-Series Analysis | Correlation Analysis | Business Insights**

---

## 👨‍💻 Author

**GuruPreeth Reddy**

B.Tech – Computer Science & Engineering

GitHub: **GuruPreeth9903**
