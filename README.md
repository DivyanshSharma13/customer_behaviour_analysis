# Data Analytics Project

## Overview

This project demonstrates an end-to-end **Data Analytics workflow**, starting from raw data loading and cleaning to SQL analysis and an interactive Power BI dashboard.

The project focuses on extracting meaningful business insights from the dataset using **Python, PostgreSQL, SQL, and Power BI**.

### Key Objectives

* Load and understand the dataset using Python
* Perform Exploratory Data Analysis (EDA)
* Clean and prepare the data
* Store and analyze data using PostgreSQL
* Write SQL queries to answer business questions
* Build an interactive Power BI dashboard
* Present key findings through a final analytical report

---

## Dataset

The dataset contains customer and purchase-related information such as:

* Customer ID
* Age and Gender
* Item Purchased
* Category
* Purchase Amount
* Location
* Season
* Review Rating
* Subscription Status
* Shipping Type
* Discount Applied
* Previous Purchases
* Payment Method
* Frequency of Purchases

The dataset was first analyzed and cleaned in Python before being used for SQL analysis and dashboard creation.

---

## Tools & Technologies

| Tool                     | Purpose                                 |
| ------------------------ | --------------------------------------- |
| **Python**               | Data loading, cleaning and EDA          |
| **Pandas**               | Data manipulation and preprocessing     |
| **Matplotlib / Seaborn** | Data visualization                      |
| **PostgreSQL**           | Database storage and SQL analysis       |
| **SQL**                  | Business analysis and data extraction   |
| **Power BI**             | Dashboard and interactive visualization |
| **Jupyter Notebook**     | Python analysis and documentation       |

---

## Project Workflow

### 1. Load Dataset

The dataset is loaded into Python using Pandas.

```python
import pandas as pd

df = pd.read_csv("dataset.csv")
```

Basic checks are performed to understand the data:

```python
df.head()
df.shape
df.info()
df.describe()
```

---

### 2. Exploratory Data Analysis

EDA was performed to understand the dataset and identify important patterns.

The analysis included:

* Checking dataset dimensions
* Understanding data types
* Identifying missing values
* Checking duplicate records
* Analyzing numerical columns
* Studying categorical variables
* Identifying important trends and patterns
* Creating visualizations

---

### 3. Data Cleaning

The dataset was cleaned before further analysis.

Major cleaning activities included:

* Handling missing values
* Removing duplicate records
* Correcting data types
* Standardizing categorical values
* Creating useful derived columns
* Checking inconsistent values
* Preparing the final dataset for PostgreSQL

The cleaned dataset was then exported for database analysis.

---

### 4. PostgreSQL & SQL Analysis

The cleaned data was imported into PostgreSQL.

SQL queries were written to answer different business questions, including:

* Total number of customers and orders
* Average purchase amount
* Sales by category
* Sales by location
* Most purchased products
* Customer segmentation
* Discount-related analysis
* Shipping type comparison
* Purchase frequency analysis
* Top products within each category

Example:

```sql
SELECT category,
       COUNT(*) AS total_orders,
       AVG(purchase_amount) AS avg_purchase
FROM customer
GROUP BY category
ORDER BY total_orders DESC;
```

SQL analysis helped convert raw data into meaningful business insights.

---

## Power BI Dashboard

The cleaned and analyzed data was used to create an interactive **Power BI dashboard**.

The dashboard includes important KPIs and visualizations such as:

* Total Customers
* Total Orders
* Total/Average Purchase Amount
* Category-wise Sales
* Product Performance
* Customer Segments
* Discount Analysis
* Shipping Analysis
* Purchase Frequency
* Location-wise Performance

Interactive filters/slicers allow users to explore the data based on different categories and customer attributes.

---

## Dashboard

The Power BI dashboard provides a visual summary of the project's key findings.

> Add your Power BI dashboard screenshot here.

Example:

```text
[ Power BI Dashboard Screenshot ]
```

---

## Key Results

The project helped identify important patterns in customer purchasing behavior and sales performance.

Key findings include:

* Identification of the highest-performing product categories
* Analysis of products with the highest number of purchases
* Understanding customer purchasing frequency
* Comparison of different shipping types
* Analysis of discount usage
* Identification of customer segments
* Understanding average purchase behavior
* Identification of trends across different locations and seasons

These insights can help businesses improve **sales strategy, customer targeting, promotions, and inventory planning**.

---

## How to Run

### Step 1: Clone the Repository

```bash
git clone <repository-url>
cd <project-folder>
```

### Step 2: Install Python Libraries

```bash
pip install pandas matplotlib seaborn jupyter
```

### Step 3: Run the Python Analysis

Open the Jupyter Notebook:

```bash
jupyter notebook
```

Run the notebook cells in order to perform:

**Data Loading → EDA → Data Cleaning → Export**

### Step 4: PostgreSQL

1. Install PostgreSQL.
2. Create a database.
3. Import the cleaned dataset.
4. Run the SQL queries provided in the `SQL` folder.

### Step 5: Power BI

1. Open the Power BI `.pbix` file.
2. Refresh the dataset if required.
3. Explore the dashboard and reports.

---

## Project Structure

```text
Data-Analytics-Project/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── notebooks/
│   └── data_analysis.ipynb
│
├── sql/
│   └── analysis_queries.sql
│
├── powerbi/
│   └── dashboard.pbix
│
├── reports/
│   └── project_report.pdf
│
└── README.md
```

---

## Skills Demonstrated

* Data Cleaning
* Exploratory Data Analysis
* Python & Pandas
* SQL
* PostgreSQL
* Data Visualization
* Power BI
* Business Analysis
* Data Interpretation
* Dashboard Development

---

## Conclusion

This project demonstrates a complete data analytics pipeline from **raw data to business insights**.

It combines Python for data preparation and EDA, PostgreSQL for structured SQL analysis, and Power BI for interactive visualization and reporting.

The project showcases practical skills required for **Data Analyst, Business Analyst, and entry-level Data Engineer roles**.
