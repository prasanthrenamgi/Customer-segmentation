# 🛍️ Customer Segmentation in Retail

## 📌 Project Overview

This project focuses on analyzing retail customer purchasing behaviour and identifying meaningful customer segments using **Exploratory Data Analysis (EDA), Cohort Analysis, RFM Analysis, and K-Means Clustering**.

The objective is to understand customer purchasing patterns, measure customer retention, evaluate customer value, and group customers based on their purchasing behaviour. These insights can help businesses develop targeted marketing strategies and improve customer engagement and retention.

## 🎯 Project Objectives

- Analyze retail sales and customer purchasing behaviour.
- Identify missing values, duplicate records, and cancelled transactions.
- Understand sales distribution across countries and products.
- Perform Cohort Analysis to measure customer retention over time.
- Apply RFM Analysis to evaluate customer value.
- Use K-Means Clustering to identify distinct customer segments.
- Interpret customer segments to support business decision-making.

## 🛠️ Technology Stack

| Category | Tools |
|---|---|
| Programming Language | Python |
| Data Manipulation | Pandas, NumPy |
| Data Visualization | Matplotlib, Seaborn |
| Machine Learning | Scikit-learn |
| Development Environment | Jupyter Notebook |
| Dataset Format | Excel (.xlsx) |

## 📂 Dataset Information

The project uses the **Online Retail Dataset**, containing transactional records from a UK-based online retail business.

The dataset covers transactions from **December 1, 2010, to December 9, 2011**.

Important attributes include:

- `InvoiceNo` – Transaction invoice number.
- `StockCode` – Product identification code.
- `Description` – Product description.
- `Quantity` – Number of products purchased.
- `InvoiceDate` – Transaction date and time.
- `UnitPrice` – Price per unit.
- `CustomerID` – Customer identification number.
- `Country` – Customer's country.

The analysis identifies 4,372 customers, approximately 3,958 products, and around 22,000 transactions.

## 🔍 Project Workflow

### 1. Data Preparation and Cleaning

- Loaded the retail transaction dataset using Pandas.
- Examined data types, missing values, and statistical summaries.
- Removed records with missing CustomerID values.
- Identified and removed duplicate records.
- Calculated transaction amounts using Quantity × UnitPrice.

### 2. Exploratory Data Analysis (EDA)

Performed analysis to understand the underlying business data:

- Country-wise transaction distribution.
- Identification of the top 10 countries by order volume.
- Customer and product analysis.
- Order distribution across invoices.
- Identification of cancelled transactions.
- Analysis of transaction amounts and sales distribution.
- Country-wise sales comparison.

### 3. Cohort Analysis

Performed time-based cohort analysis to understand customer retention.

- Grouped customers based on their first purchase month.
- Created CohortMonth and CohortIndex variables.
- Calculated monthly active customer counts.
- Generated customer retention rates.
- Visualized retention patterns using a heatmap.

### 4. RFM Analysis

Applied RFM (Recency, Frequency, Monetary) analysis to evaluate customer purchasing behaviour.

| Metric | Description |
|---|---|
| Recency | How recently a customer made a purchase. |
| Frequency | Number of transactions made by a customer. |
| Monetary | Total monetary value of customer purchases. |

- Calculated RFM metrics for individual customers.
- Assigned quartile-based scores from 1 to 4.
- Generated RFM segments and combined RFM scores.
- Categorized customers into Low, Middle, and Top segments.

### 5. Data Preprocessing for Clustering

Prepared RFM variables for K-Means clustering.

- Examined the distributions of Recency, Frequency, and MonetaryValue.
- Applied logarithmic transformation to reduce skewness.
- Used StandardScaler for feature normalization.
- Examined the transformed feature distributions.

### 6. K-Means Clustering

Implemented K-Means clustering to identify groups of customers with similar purchasing behaviour.

- Applied the Elbow Method to determine potential cluster counts.
- Compared clustering solutions with K = 3, K = 4, and K = 5.
- Analyzed average Recency, Frequency, and MonetaryValue across clusters.
- Used snake plots to compare cluster characteristics.
- Examined relative feature importance using a heatmap.

### 7. Customer Segmentation and Interpretation

The final analysis identifies four customer segments:

- **New Customers** – Recently acquired customers.
- **Lost Customers** – Customers who have not purchased recently.
- **Best Customers** – Customers with strong purchasing activity and monetary contribution.
- **At-Risk Customers** – Customers showing signs of reduced engagement.

These segments can support targeted marketing, customer retention, and business growth strategies.

## 📊 Key Analysis and Visualizations

The notebook includes:

- Country-wise order distribution.
- Transaction and sales distribution charts.
- Customer Cohort Retention Heatmap.
- RFM Score Distribution.
- Customer RFM Summary Tables.
- Elbow Method Plot.
- K-Means Cluster Comparison.
- Customer Segment Snake Plots.
- Relative Importance Heatmap.

## ⚙️ Installation and Setup

**1. Clone the repository**

```bash
git clone https://github.com/your-username/customer-segmentation-retail.git
```

**2. Navigate to the project directory**

```bash
cd customer-segmentation-retail
```

**3. Install the required libraries**

```bash
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl jupyter
```

**4. Place the dataset in the expected directory**

```text
Customer-Segmentation-in-Retail/
│
├── Data/
│   └── Online Retail.xlsx
│
├── Customer Segmentation in Retail.ipynb
└── README.md
```

**5. Launch Jupyter Notebook**

```bash
jupyter notebook
```

Open `Customer Segmentation in Retail.ipynb` and execute the notebook cells.

## 💡 Business Applications

The analysis can help retail businesses:

- Identify high-value customers.
- Understand customer purchasing frequency.
- Monitor customer retention and engagement.
- Identify customers at risk of leaving.
- Develop personalized marketing campaigns.
- Improve customer relationship management.
- Make data-driven business decisions.

## 🚀 Future Improvements

- Develop an interactive Power BI dashboard.
- Explore additional customer segmentation techniques.
- Automate customer segmentation and reporting.
- Build predictive models for customer churn.
- Develop targeted marketing recommendations for each segment.

## 👨‍💻 Author

**Prasanth Renamgi**

Aspiring Data Analyst | SQL | Python | Excel | Power BI

GitHub: [https://github.com/prasanthrenamgi](https://github.com/prasanthrenamgi)

---

⭐ If you find this project useful, consider giving the repository a star!
