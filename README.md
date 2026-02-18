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

