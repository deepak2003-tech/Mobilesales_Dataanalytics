# Mobile Sales Data Analytics with AI

**Student:** Deepak Phapale  
**Project Type:** Data Analytics with AI  
**Main File:** `DeepakPhapale_MobileSales_Data_Analytics.ipynb`

## Project Overview

This project analyzes mobile sales transaction data using Python. It performs data loading, dataset inspection, data-quality checks, date processing, monthly revenue aggregation, visualization, and a simple Linear Regression forecast for the next month's revenue.

## Dataset

The notebook expects a CSV file named:

`mobile_sales.csv`

The dataset used in the supplied project contains 1,000 transaction records and 11 original columns:

- TransactionID
- Date
- MobileModel
- Brand
- Price
- UnitsSold
- TotalRevenue
- CustomerAge
- CustomerGender
- Location
- PaymentMethod

The notebook also creates a derived `Month` feature from `Date`.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook / Google Colab

## Analysis Performed

1. Import Python libraries.
2. Upload and read `mobile_sales.csv`.
3. Inspect dataset shape, columns, and data types.
4. Check missing values and duplicate rows.
5. Convert the `Date` column to datetime.
6. Create a monthly time feature.
7. Calculate total revenue, total units sold, and transaction count.
8. Aggregate revenue by month.
9. Visualize the monthly revenue trend.
10. Train a Linear Regression model using sequential month numbers.
11. Predict the next month's revenue.
12. Plot actual revenue against the fitted/predicted trend.

## Reported Results From the Supplied Project

- Rows: **1,000**
- Original columns: **11**
- Missing values: **0 in every original column**
- Duplicate rows: **0**
- Total Revenue: **₹40,218,445.04**
- Total Units Sold: **50,074**
- Total Transactions: **1,000**
- Next-month predicted revenue: **₹5,199,874.31**
- Monthly aggregation covered **January 2024 to July 2024**

## Setup / Run Instructions

### Google Colab

1. Open the `.ipynb` file in Google Colab.
2. Run the library-import cell.
3. Run the upload cell.
4. Upload the file `mobile_sales.csv`.
5. Run the remaining cells from top to bottom.
6. Review the tables, charts, and forecast.

### Local Jupyter

Install dependencies:

```bash
pip install -r requirements.txt
```

Place `mobile_sales.csv` in the same working folder as the notebook and run the notebook cells in order. If running outside Google Colab, replace the Colab upload cell with a normal local CSV path, for example:

```python
df = pd.read_csv("mobile_sales.csv")
```

## Important Note About the Forecast

The Linear Regression model uses only sequential month numbers and monthly revenue. It is a simple trend model and does not include product, brand, price, customer, location, payment, seasonality, or other explanatory variables. Therefore, the forecast is an analytical estimate and should not be interpreted as a guaranteed business outcome.

## Files in This Submission

- `DeepakPhapale_MobileSales_Data_Analytics.ipynb` — complete project code
- `requirements.txt` — Python dependencies
- `DeepakPhapale_MobileSales_Project_Report.docx` — project report
- `README.md` — project overview and run instructions
