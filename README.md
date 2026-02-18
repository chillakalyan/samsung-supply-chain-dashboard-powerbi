# 📊 Samsung Supply Chain & Logistics Dashboard (Power BI)

## 📌 Project Overview

This project presents an interactive **Supply Chain & Logistics Dashboard** built using **Power BI**.  

The dashboard provides end-to-end insights into:

- Supplier performance  
- Revenue distribution  
- Operational KPIs  
- Logistics efficiency  

The main objective of this project is to analyze supply chain performance and identify key operational improvements using data-driven insights.

---

## 🛠 Tools & Technologies Used

- **Power BI Desktop**
- **DAX (Data Analysis Expressions)**
- **Data Modeling**
- **KPI Visualization**
- **Business Intelligence Concepts**

---

## 📁 Project Structure

```
samsung-supply-chain-dashboard-powerbi/
│
├── dashboard/ # Power BI (.pbix) file
├── screenshots/ # Final dashboard previews
├── README.md                      # Project documentation
├── dashboard-design-process/ # Development & modeling screenshots
├── datasets/ # Raw dataset (if applicable)
├── ml experiments /* ml integrated
└── streamlit_app.py               # Main Streamlit application
```
---


---

## 📊 Key Performance Indicators (KPIs)

The dashboard includes the following KPIs:

- **Total Revenue**
- **Gross Revenue**
- **Profit**
- **Profit Margin %**
- **Perfect Order %**
- **Discount Analysis**
- **Supplier Average Lead Time**
- **Channel-wise Revenue & Profit Breakdown**

---
---

## 🤖 Machine Learning Experimentation (Lead Time Prediction)

To extend the dashboard with predictive capabilities, a Machine Learning experiment was conducted using Python.

### Objective
Predict supplier **lead time (in days)** using procurement data.

### ML Workflow

1. Exported engineered dataset from Power BI
2. Performed feature engineering by merging:
   - Date dimension
   - Supplier dimension
   - Product dimension
3. Trained a **Random Forest Regression model**
4. Evaluated model performance using:
   - Mean Absolute Error (MAE)
   - R² Score

### Dataset Features Used

- order_quantity  
- supplier_id  
- product_id  
- unit_cost  
- total_cost  
- quality_score  
- month, quarter, year  
- supplier tier & category features  

### Model Results

- MAE ≈ 2.87 days  
- R² ≈ 0.10  

### Key Finding

Model performance indicated limited predictive signal in the available features.  
This suggests that supplier lead time may depend on additional operational or external factors not captured in the dataset.

This experiment demonstrates an end-to-end BI + ML integration workflow.

---

## 📂 ML Files
```│
├── lead_time_model.ipynb
└── procurement_ml_engineered.csv
```
---
## 🔍 Dashboard Insights

- The **Online channel** contributes the highest share of total revenue.
- Certain suppliers demonstrate **lower average lead times**, improving operational efficiency.
- Profit margins fluctuate across months, indicating **seasonal performance trends**.
- Order quantity directly impacts **supplier performance and logistics timelines**.
- Channel-wise profit distribution highlights the contribution of **Retailer vs Direct sales**.

---

## 🚀 Project Outcome

This dashboard enables:

- Data-driven supply chain decision making  
- Supplier performance optimization  
- Revenue and profit trend analysis  
- Identification of logistics bottlenecks  
- Strategic channel performance comparison  


