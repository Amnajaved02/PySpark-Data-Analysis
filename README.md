# 🚕 NYC Yellow Taxi Trip Data Analysis with PySpark

A hands-on PySpark data engineering project analysing NYC TLC Yellow Taxi trip records for January and February 2026. Built as part of a portfolio to demonstrate practical big data pipeline skills.

> **Related certification:** [PySpark Essential Training: Introduction to Building Data Pipelines](https://www.linkedin.com/learning/) — LinkedIn Learning · Completed April 14, 2026 · Instructor: Shea Hanson

---

## 📌 Project Overview

This project applies core PySpark concepts to a real-world dataset — the NYC Taxi & Limousine Commission (TLC) trip records — covering the full journey from raw Parquet ingestion through to enriched, aggregated output.

The code is structured as a single, well-commented script suitable for running in Google Colab.

---

## 📂 Repository Structure

```
taxi_data_analysis_pyspark/
├── Dataset/
│   ├── taxi_zone_lookup.csv               # Borough and zone reference table
│   ├── yellow_tripdata_2026-01.parquet    # January 2026 trip records
│   └── yellow_tripdata_2026-02.parquet    # February 2026 trip records
├── EDA Notebook/
│   └── PySpark_EDA.ipynb                  # Main analysis notebook (13 sections)
└── README.md                              # This file
```

---

## 🗂️ Dataset

| File | Description |
|---|---|
| `yellow_tripdata_2026-01.parquet` | NYC TLC Yellow Taxi — January 2026 |
| `yellow_tripdata_2026-02.parquet` | NYC TLC Yellow Taxi — February 2026 |
| `taxi_zone_lookup.csv` | Borough and zone reference table |

**Source:** [NYC TLC Trip Record Data](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

All dataset files are included in the `Dataset/` folder of this repository.

---

## 🔧 Skills & Concepts Demonstrated

| # | Section | Concepts |
|---|---|---|
| 0 | Environment Setup | PySpark install, Google Drive mount |
| 1 | SparkSession | `SparkSession.builder.getOrCreate()` |
| 2 | Load Data | `spark.read.parquet()`, lazy evaluation |
| 3 | Schema Exploration | `printSchema()`, `describe()`, `count()` |
| 4 | Selection & Sorting | `select()`, `sort()` |
| 5 | Filtering | Single and compound filters, query chains |
| 6 | Null Handling | `isnull()`, `fillna()` |
| 7 | Feature Engineering | `withColumn()`, `unix_timestamp()`, trip duration |
| 8 | Column Renaming | `withColumnsRenamed()`, snake_case conventions |
| 9 | Union | Combining monthly DataFrames with `union()` |
| 10 | Joins | Left join with zone lookup table |
| 11 | Full Pipeline | End-to-end pipeline (2025 dataset challenge) |
| 12 | Aggregations | `groupBy()`, `agg()`, `avg()`, `count()`, `min()`, `max()` |

---

## ▶️ How to Run

1. Clone this repository
2. Install dependencies: `pip install pyspark`
3. Open `EDA Notebook/PySpark_EDA.ipynb` in Jupyter or VS Code
4. Run all cells — dataset files are already included in the `Dataset/` folder

```bash
git clone https://github.com/[YOUR_USERNAME]/taxi_data_analysis_pyspark.git
cd taxi_data_analysis_pyspark
pip install pyspark
jupyter notebook "EDA Notebook/PySpark_EDA.ipynb"
```

---

## 🛠️ Tech Stack

- **PySpark** — distributed data processing
- **Google Colab** — cloud execution environment
- **Google Drive** — dataset storage
- **Parquet** — columnar file format for efficient reads
- **Python 3.x**

---

## 🎓 Credits

This project was built alongside the LinkedIn Learning course:

**PySpark Essential Training: Introduction to Building Data Pipelines**
Instructor: Shea Hanson, Head of Learning Content Strategy — LinkedIn Learning
Completed: April 14, 2026

The course provided the foundational structure; all code in this repo has been extended, refactored, and commented independently.

---

## 👩‍💻 Author

**Amna Javed**
[LinkedIn](https://www.linkedin.com/in/) · [GitHub](https://github.com/)
