# 📈 Evaluating a Landing Page Redesign: A/B Testing Analysis for an E-Commerce Platform

**Project Category:** A/B Testing / Statistical Analysis  
**Tools & Technologies:**  
Python · Pandas · NumPy · SciPy · Matplotlib · Seaborn  
**Other Tools:** Jupyter Notebooks

---

## 🔍 Overview

In the fast-moving world of e-commerce, landing pages play a crucial role in converting visitors into customers. Even a small improvement in conversion rate can lead to significant revenue growth. This project explores whether a newly designed landing page improves conversion rates over the existing one, using a rigorous A/B testing framework.

By implementing a statistically sound A/B Test, the analysis investigates the effectiveness of the new design and its impact on user behavior across different countries. The final recommendation is backed by hypothesis testing using a two-proportion z-test.

---

## ❓ Problem Statement

A major e-commerce platform aims to optimize its conversion funnel by redesigning its landing page. The core question:  
**Does the new landing page lead to a statistically significant increase in user conversion rates compared to the current version?**

To answer this, users were randomly assigned to either the **control group** (old page) or the **treatment group** (new page). The conversion outcomes were then compared using robust statistical testing techniques.

---

## 📂 Dataset Description

**[Download Dataset](https://drive.google.com/file/d/1VM9JBEgFoWySWY4GBanb6BA1eFCIRcDd/view?usp=sharing)**

- **Rows:** ~295,000 user visits
- **Columns:** 5
  - `user_id`: Unique identifier for each user
  - `timestamp`: Time of visit
  - `group`: Control or Treatment group assignment
  - `landing_page`: Page version shown (old_page or new_page)
  - `converted`: Binary indicator (1 if user converted, 0 otherwise)

---

## 📊 Exploratory Data Analysis (EDA)

Key visualizations and breakdowns included:

- ✅ **Conversion Rate Comparison**
- 🌍 **User Distribution by Country and Group**

| Country | Control Users | Treatment Users |
|---------|----------------|------------------|
| CA      | 7,138          | 7,256            |
| UK      | 36,100         | 35,861           |
| US      | 100,988        | 101,197          |

**Conversion Rates**  
- Control Group: **12.02%**  
- Treatment Group: **11.87%**

Visualizations (bar charts) confirmed similar user distribution across groups and no visible conversion improvement for the new landing page.

---

## 📐 Hypothesis Testing

A **two-proportion z-test** was used to test the hypothesis:

- **Null Hypothesis (H₀):** Conversion rate of new page ≤ Conversion rate of old page
- **Alternative Hypothesis (H₁):** Conversion rate of new page > Conversion rate of old page

### 🧪 Test Results:

- **Z-Statistic:** -1.2942  
- **P-Value:** 0.1956

Since the p-value is greater than 0.05, we **fail to reject the null hypothesis**. There is **no statistically significant evidence** that the new landing page performs better than the existing one.

---

## 🧾 Code Documentation

- All analysis steps were executed in **Python** using a **Jupyter Notebook** environment.
- The notebook is well-documented with **Markdown explanations** for clarity.

### 💻 Setup Instructions

- **Python Version**: ≥3.7
- **Install Required Packages:**
```bash
pip install pandas numpy matplotlib seaborn scipy statsmodels
```

---

### 📌 Key Takeaways

* The new landing page did not significantly outperform the old one in terms of conversion rate.

* Statistically, the observed difference in conversion rates is not meaningful enough to justify a rollout.

* Recommendation: Stick with the current design or conduct additional testing with variations targeting specific user segments.

---

### 📅 Limitations & Future Scope

Limitations:

- The experiment assumes random assignment and no implementation bugs.

- No segmentation by user type, device, or visit behavior was included.

Future Improvements:

- Segmented A/B Testing by geography, traffic source, or device type.

- Time-Based Analysis to detect possible novelty effects or learning curves.

- Multivariate Testing to explore other page components (e.g., CTA buttons, layout changes).

---

### 👤 About the Author

Author: Rudrajit Bhattacharyya
Email: rudrajitb24@gmail.com
LinkedIn: LinkedIn Profile
GitHub: GitHub Profile

---
