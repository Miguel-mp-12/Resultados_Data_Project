# 📊 Customer Insights ETL & Advanced Analytics Pipeline

Welcome to the **Customer Insights Project** – an end-to-end, enterprise-grade data pipeline designed to simulate, clean, transform, analyze, and model commercial sales data.  
This project reflects a real-world data stack you’d find in a modern data-driven company.

---

## 🚀 Project Overview

This pipeline was designed for advanced data analysis, supporting predictive and prescriptive modeling, as well as simulating realistic data flows from scratch. It mimics how large pharmaceutical or commercial teams manage customer and sales data.

---

## 📁 Project Structure

Project/

├── data/

│ ├── bronze/ # Raw simulated data (dirty)

│ ├── silver/ # Cleaned, validated datasets

│ ├── gold/ # Business-ready, renamed datasets

│ ├── platinum/ # Fully joined dataset ready for ML

├── outputs/

│ ├── plots/ # Visualizations

│ ├── logs/ # Logs from each stage

│ ├── predictive/ # PDF reports for predictive models

│ ├── prescriptive/ # Scenario-based simulations

│ └── data_catalog/ # Auto-generated metadata

├── pipelines/

│ ├── utils/ # Shared functions, simulation scripts

│ ├── bronze_to_silver/

│ ├── silver_to_gold/

│ ├── analytics/ # Modeling scripts

├── src/

│ └── main.py # Master pipeline controller



## 🔁 ETL Pipeline Flow


  A[Simulate Data (Bronze)] --> B[Clean & Validate (Silver)]
  
  B --> C[Dimension Mapping + Join (Platinum)]
  
  C --> D[Predictive Model]
  
  C --> E[Prescriptive Simulation]
  
  D --> F[PDF Report]
  
  E --> F
  
##⚙️ Main Features
✅ Full synthetic data generation with [Faker]

✅ Data quality logs, ingestion tracking, and versioning

✅ Key business metrics calculated and validated

✅ Predictive modeling (Random Forest Regressor)

✅ Prescriptive simulation (price change, rep assignment...)

✅ Dynamic PDF generation with summaries & charts

✅ Fully modular: run individual scripts or the whole pipeline via run_etl.py

## 📊 Predictive Model Highlights
Target: Total Value (USD)

Top Features: Discount %, Customer Type, Rep Tenure

Metrics:

R²: >85% → Excellent fit

MAE: Error in dollar terms

RMSE: Measures variability

Report: Generated PDF with:

Executive summary

Feature importance

Prediction scatter plot

Recommendations based on top features

### 🧠 Prescriptive Model Scenarios
We simulate 3 real-world what-if strategies:

Reduce Discounts by 10%

Only Assign Experienced Reps (>1y)

Increase Price 5% for Hospitals

For each:

Predicted revenue impact (total + per transaction)

Distribution of deltas

Scatter comparison and textual recommendation

## 📌 How to Run
Activate virtualenv:

bash
source venv/bin/activate
Run entire pipeline:

bash
python src/run_etl.py
Explore outputs:

PDF reports in outputs/predictive/ and prescriptive/

Clean data in /data/*

Logs in /outputs/logs

🔧 Requirements

    pandas
    numpy
    matplotlib
    seaborn
    scikit-learn
    faker

Install with:

bash
pip install -r requirements.txt
