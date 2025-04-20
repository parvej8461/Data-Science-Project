

# Automotive Repair Data Analysis & Tagging

This project involves exploratory data analysis, cleaning, visualization, and feature extraction from an automotive repair dataset. The goal is to uncover insights related to part failures, cost anomalies, and customer-reported issues, and provide actionable recommendations for stakeholders.

## Source Notebook  
**Colab Link**: [Parvej Akhter.ipynb](https://colab.research.google.com/drive/15zDwY0AdEoR1qCekwWFl1TwekL0Fsrod)

## Dataset
The dataset (`Data for Task 1.xlsx`) contains records of repair events, including parts replaced, repair dates, costs, and customer feedback.

---

## 🔧 Steps Performed

### 1. **Data Cleaning**
- Dropped unnecessary columns (`CAMPAIGN_NBR`)
- Handled missing values:
  - Numerical columns: filled with median
  - Categorical/text columns: filled with `"unknown"`
- Handled outliers using the Interquartile Range (IQR) method

### 2. **Feature Selection**
Selected 5 critical columns for stakeholder analysis:
- `VIN`
- `REPAIR_DATE`
- `TOTALCOST`
- `CAUSAL_PART_NM`
- `CUSTOMER_VERBATIM`

### 3. **Data Visualization**
- **Top 10 Replaced Parts** (bar plot)
- **Repair Transaction Categories** (count plot)
- **Repair Trends Over Time** (line plot)
- **Total Repair Cost Distribution** (histogram)

### 4. **Text Processing & Tagging**
- Tokenized customer feedback using NLTK
- Removed stopwords and extracted top 10 frequent keywords from `CUSTOMER_VERBATIM`
- Exported cleaned and tagged data as `cleaned_tagged_axionray_data.csv`

---

## Key Insights & Recommendations

- **Frequent Issues**: Common problems involve stitching, heating modules, and peeling components.
- **Cost Analysis**: Cost distribution shows potential outliers which may impact warranty budgets.
- **Temporal Trends**: Repair volumes fluctuate over time, suggesting seasonal or batch-specific defects.
- **Customer Feedback**: Extracted keywords support targeting specific components for quality improvements.

### Recommendations
- Investigate high-frequency part failures for design/supplier issues.
- Segment data by model/region for deeper insights.
- Utilize tagged feedback for developing predictive maintenance strategies.

---

## 💾 Output
- Cleaned dataset: `cleaned_tagged_axionray_data.csv`
- Visuals: 
  - `Transaction_Categories.png`
  - `Repair_Trends.png`
  - `TotalCost_Distribution.png`

---

##  Author
**Parvej Akhter**  
Email: parvejakhter2303@outlook.com  
GitHub: [@parvej8461](https://github.com/parvej8461)

---
