# 📊 Credit Card Payment Analysis — Exploratory Data Analysis (EDA)

## 🧭 Project Overview
This project performs **Exploratory Data Analysis (EDA)** on a credit card payment dataset (April–September 2005) to identify patterns and factors that distinguish **credible** from **non-credible** customers.  

The analysis focuses on understanding customers’ demographic and financial behavior by examining payment history, bill amounts, credit limits, and default tendencies.

---

## 🎯 Objective
To explore and analyze customer credit card payment data and extract insights that:
- Identify key factors influencing **credit default**.
- Highlight behavioral and financial trends of customers.
- Support risk assessment and data-driven credit decisions.

---

## 📁 Project Files
| File | Description |
|------|--------------|
| `EDA_CC.html` | The final rendered HTML version of the Jupyter Notebook containing all Python code, analysis, and visualizations. |
| `EDA Python Project Guidelines.pdf` | A structured guideline document outlining the step-by-step plan for performing the analysis, including data understanding, cleaning, EDA, and insight generation. |

---

## 🧩 Dataset Description
The dataset contains **customer demographic and credit card payment details** over six months.

| Feature | Description |
|----------|-------------|
| `LIMIT_BAL` | Amount of credit given (NT dollars) including personal and family credit. |
| `GENDER` | Gender of the cardholder (1 = Male, 2 = Female). |
| `EDUCATION` | Education level (1 = Graduate school, 2 = University, 3 = High school, 4 = Others). |
| `MARRIAGE` | Marital status (1 = Married, 2 = Single, 3 = Others). |
| `AGE` | Age of the customer. |
| `PAY_1`–`PAY_6` | Repayment status from April–September 2005 (−1 = Paid duly, 1 = Delay 1 month, etc.). |
| `BILL_AMT1`–`BILL_AMT6` | Bill statement amounts from April–September 2005. |
| `PAY_AMT1`–`PAY_AMT6` | Amounts paid from April–September 2005. |
| `DEFAULT` | Default payment next month (1 = Yes, 0 = No). |

---

## ⚙️ Tools and Libraries Used
- **Python 3**
- **Pandas**, **NumPy** – Data manipulation and preprocessing  
- **Matplotlib**, **Seaborn** – Visualization and exploration  
- **Scikit-learn** – Encoding and preprocessing (if applicable)
- **Jupyter Notebook / HTML Export**

---

## 🧠 Analysis Steps

### **1️⃣ Data Understanding**
- Loaded and inspected the dataset.
- Reviewed data types, missing values, and basic statistics.
- Identified target variable `DEFAULT`.

### **2️⃣ Data Cleaning & Feature Engineering**
- Handled missing values and outliers.
- Combined unknown education and marriage levels into “Unknown.”
- Engineered new features such as:
  - Average bill amount across six months  
  - Average payment amount across six months  

### **3️⃣ Exploratory Data Analysis**
#### *Univariate Analysis*
- Distribution plots for numerical features (e.g., `LIMIT_BAL`, `AGE`).
- Count plots for categorical variables (`GENDER`, `EDUCATION`, `MARRIAGE`).

#### *Bivariate Analysis*
- Relationship between `DEFAULT` and:
  - `LIMIT_BAL`, `AGE`, `GENDER`, `EDUCATION`, `MARRIAGE`.
- Box and violin plots to visualize differences between defaulters and non-defaulters.

#### *Multivariate Analysis*
- Pair plots for bill and payment amounts.
- Correlation heatmap to identify strong inter-feature relationships.

### **4️⃣ Insights and Conclusions**
- Customers with **lower credit limits** and **higher past due payments** showed a greater likelihood of default.
- Education and marital status exhibited weak relationships with default.
- Strong positive correlation between consecutive `BILL_AMT` and `PAY_AMT` columns.
- Outliers were observed in high credit limits and payment amounts.
- Repayment status (`PAY_1`–`PAY_6`) showed a strong predictive relationship with default behavior.

---

## 📈 Visual Highlights
Example plots and visuals from the notebook:
- Distribution of `LIMIT_BAL`
- Count plot of defaulted vs. non-defaulted customers
- Correlation heatmap of financial features
- Boxplot of `LIMIT_BAL` grouped by `DEFAULT`

> 🖼️ *For complete visualizations, refer to the HTML file: `EDA_CC.html`.*

---

## 📑 Project Deliverables
| Deliverable | Format | Description |
|--------------|---------|-------------|
| Jupyter Notebook / HTML | `.html` | Complete EDA with visualizations and commentary |
| Summary Report | `.pdf` | Guidelines and project steps for consistent reporting |

---

## 📅 Project Workflow
| Day | Task | Deliverable |
|-----|------|-------------|
| **Day 1** | Setup, data loading, basic understanding | Initial notebook |
| **Day 2** | Cleaning, feature engineering, and preprocessing | Clean dataset ready for analysis |
| **Day 3** | EDA and visualization | Visual reports and insights |
| **Day 4** | Summary and submission | Final HTML and report |

---

## 🚀 How to View the Project
To view the complete analysis:
1. Open the file **`EDA_CC.html`** in a browser.  
   *(Double-click or drag into any browser window.)*  
2. Review the structured code, visualizations, and insights section by section.

---

## 🏁 Final Takeaways
- Effective EDA enables data-driven insights for credit risk modeling.
- Payment history (`PAY_1`–`PAY_6`) is a strong early warning signal for defaults.
- Structured data cleaning and visualization provide clarity for downstream modeling.

---

## 👩‍💻 Author
**Nisha Rai**  
Data Analytics | EDA | Python | Visualization
