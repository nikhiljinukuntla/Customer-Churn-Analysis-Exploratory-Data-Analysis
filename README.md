# Customer Churn Analysis — Exploratory Data Analysis

An end-to-end EDA project exploring what drives customer churn, built as part of my data analyst portfolio. The notebook covers data cleaning, univariate and bivariate analysis, feature binning, correlation analysis, and a set of business-relevant insights and recommendations.

## 📌 Project Structure

This notebook is split into two parts:

1. **Part 1 — Warm-up EDA** on a bank customer dataset (`Churn_Modelling.csv`), used to practice univariate/bivariate analysis and correlation techniques.
2. **Part 2 — Case Study** on a telecom customer dataset (`CustomerChurn.csv`): full data cleaning, feature engineering, univariate/bivariate analysis, and a final set of insights.

## 📂 Datasets

The raw CSVs are not included in this repo. Download them and place them in a `data/` folder at the project root:

- **Churn_Modelling.csv** — the classic bank customer churn dataset (credit score, geography, age, balance, etc., with an `Exited` target column). Commonly shared via GitHub course repos (e.g. [sharmaroshan/Churn-Modelling-Dataset](https://github.com/sharmaroshan/Churn-Modelling-Dataset)); also mirrored on [Kaggle](https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling).
- **CustomerChurn.csv** — the well-known IBM Telco Customer Churn dataset (originally `WA_Fn-UseC_-Telco-Customer-Churn.csv`). Available on [Kaggle: Telco Customer Churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn).

Expected folder structure:
```
customer-churn-eda/
├── customer-churn-eda.ipynb
├── requirements.txt
├── README.md
└── data/
    ├── Churn_Modelling.csv
    └── CustomerChurn.csv
```

## 🛠️ Tools & Libraries

- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## 🚀 How to Run

1. Clone this repo:
   ```
   git clone https://github.com/nikhiljinukuntla/customer-churn-eda.git
   cd customer-churn-eda
   ```
2. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
3. Download the datasets from the Kaggle links above and place them in a `data/` folder as shown.
4. Open `customer-churn-eda.ipynb` in Jupyter or VS Code and run all cells.

## 🔍 Key Insights

- The dataset is highly imbalanced — roughly 73% of customers stay vs. 27% who churn.
- Customers on **month-to-month contracts** churn at a much higher rate than those on one- or two-year contracts.
- Customers paying via **electronic check** show notably higher churn than other payment methods.
- Customers **without Online Security or Tech Support add-ons** churn more frequently.
- Higher **Monthly Charges** correlate with a higher likelihood of churn.
- **Tenure** is negatively correlated with churn — newer customers are more likely to leave than long-tenured ones.

## 💡 Business Recommendations

- Target month-to-month, electronic-check customers with proactive retention offers or incentives to switch to longer contracts / other payment methods.
- Bundle Online Security and Tech Support into onboarding offers, since customers without these add-ons churn more.
- Focus retention efforts on the first few months of the customer lifecycle, where churn risk is highest.

## 📬 Connect

- GitHub: [nikhiljinukuntla](https://github.com/nikhiljinukuntla)
- LinkedIn: [jinukuntla-nikhil](https://linkedin.com/in/jinukuntla-nikhil/)
