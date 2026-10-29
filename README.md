# Task 2: Exploratory Data Analysis (EDA)

## Project overview
This project uses Python, Pandas, NumPy, Matplotlib, and SciPy to explore an e-commerce orders dataset, identify patterns, check data quality, visualize results, and test simple hypotheses.

## Dataset
- File: `Ecommerce_Dataset_3000.csv`
- Records: 3,000
- Columns: 24
- This is a 3,000-row sample created for easier sharing. Findings apply to this sample only, not necessarily the complete original dataset.

## Initial findings
- Most frequent category: **Set** (1,228 records; 40.9%).
- Most frequent order status: **Shipped** (2,002 records).
- Cancelled records: **438/3,000 (14.6%)**.
- Amount values available: **2,780**; missing Amount values: **220**.
- Mean amount among available values: **INR 624.41**; median: **INR 574.00**.
- Most frequent shipping state: **MAHARASHTRA** (517 records).
- Exact duplicate rows: **0**.
- Completely empty column(s): **Unnamed: 22**.

These are descriptive results, not causal conclusions. The notebook generates plots and runs a Welch two-sample t-test comparing amount by shipping service level.

## Repository files
- `CodeAlpha_Task2_EDA.ipynb` — notebook containing EDA code, visualizations, data-quality checks, and hypothesis tests.
- `Ecommerce_Dataset_3000.csv` — dataset sample.
- `README.md` — project summary and findings.
- `requirements.txt` — dependencies.

## How to run
1. Keep the notebook and CSV in the same folder.
2. Install dependencies: `pip install -r requirements.txt`
3. Open the notebook in Jupyter and select **Run → Run All Cells**.

## Data quality issues identified
- Missing values occur in `Courier Status`, `currency`, `Amount`, location fields, `promotion-ids`, and `fulfilled-by`.
- `Unnamed: 22` is entirely empty in this sample and is removed from the analysis copy.
- `Sales Channel ` has a trailing space; the analysis copy normalizes column names.
- Missing values are not replaced with invented values.

## Task 2 coverage
- Meaningful questions defined before analysis.
- Dataset structure and variable types explored.
- Patterns and potential anomalies investigated with statistics and visualizations.
- Hypothesis checked and statistical comparison performed.
- Data-quality issues documented.
