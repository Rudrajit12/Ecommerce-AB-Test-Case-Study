# 📈 Evaluating a Landing Page Redesign: A/B Testing Analysis for an E-Commerce Platform

### **Project Category:** A/B Testing / Statistical Analysis  
### **Tools & Technologies:**  
![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54) ![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-3776AB?style=for-the-badge&logo=matplotlib&logoColor=white) ![Seaborn](https://img.shields.io/badge/Seaborn-43B02A?style=for-the-badge&logo=seaborn&logoColor=white) ![Statsmodels](https://img.shields.io/badge/statsmodels-0.14.0+-blue)

**Other Tools**: NumPy, Jupyter Notebooks

---

## 🔍 Overview

In the fast-moving world of e-commerce, landing pages play a crucial role in converting visitors into customers. Even a small improvement in conversion rate can lead to significant revenue growth. This project explores whether a newly designed landing page improves conversion rates over the existing one, using a rigorous A/B testing framework.

By implementing a statistically sound A/B Test, the analysis investigates the effectiveness of the new design and its impact on user behavior across different countries. The final recommendation is backed by hypothesis testing using a two-proportion z-test.

![A/B Testing Diagram](https://drive.google.com/uc?export=view&id=1C031Lqjv8PRpdAj48gPM9H8RXAMgXAq5)


---

## ❓ Problem Statement

A major e-commerce platform aims to optimize its conversion funnel by redesigning its landing page. The core question:  
**Does the new landing page lead to a statistically significant increase in user conversion rates compared to the current version?**

To answer this, users were randomly assigned to either the **control group** (old page) or the **treatment group** (new page). The conversion outcomes were then compared using robust statistical testing techniques.

---

## 📂 Dataset Description

**[Download Dataset](https://drive.google.com/uc?export=download&id=1NCHCTl-rmAK4NGLnUKvWoOQHDA2vbo0J)**

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

![User Distribution](https://drive.google.com/uc?export=view&id=122ac5ukO8U1cC7H-jgdmzGPRBWRgTfCS)

**Conversion Rates**  
- Control Group: **12.02%**  
- Treatment Group: **11.87%**

![Conversion Rates](https://drive.google.com/uc?export=view&id=16JBYkQpAQbbWYSGFu2_RCIUIL-dem_z7)

Visualizations (bar charts) confirmed similar user distribution across groups and no visible conversion improvement for the new landing page.

---

## 📐 Hypothesis Testing

A **two-proportion z-test** was used to test the hypothesis:

- **Null Hypothesis (H₀):** Conversion rate of new page = Conversion rate of old page
- **Alternative Hypothesis (H₁):** Conversion rate of new page ≠ Conversion rate of old page

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

## 📌 Key Takeaways

* The new landing page did not significantly outperform the old one in terms of conversion rate.

* Statistically, the observed difference in conversion rates is not meaningful enough to justify a rollout.

* Recommendation: Stick with the current design or conduct additional testing with variations targeting specific user segments.

---

## 📅 Limitations & Future Scope

### Limitations:

- The experiment assumes random assignment and no implementation bugs.

- No segmentation by user type, device, or visit behavior was included.

### Future Improvements:

- Segmented A/B Testing by geography, traffic source, or device type.

- Time-Based Analysis to detect possible novelty effects or learning curves.

- Multivariate Testing to explore other page components (e.g., CTA buttons, layout changes).

---

## References:

### 📊 Z-Test Methodology Reference
- [Two-Proportion Z-Test Explained – Towards Data Science](https://towardsdatascience.com/ab-testing-with-python-e5964dd66143/)
- [Hypothesis Testing – Khan Academy](https://www.khanacademy.org/math/statistics-probability/significance-tests-one-sample)

### 🧪 A/B Testing Concepts and Best Practices
- [Optimizely A/B Testing Guide](https://www.optimizely.com/optimization-glossary/ab-testing/)

---

## Resources

- **IPYNB Notebook**: [Colab Link](https://colab.research.google.com/drive/1_yLgcjAHwjWokom_zBbConsCq27GFX53?usp=sharing)  
- **GitHub Repository**: [GitHub Link](https://github.com/Rudrajit12/Ecommerce-AB-Test-Case-Study)

---

## About the Author

**Author**: Rudrajit Bhattacharyya  

- **Email**: [rudrajitb24@gmail.com](mailto:rudrajitb24@gmail.com)  
- **LinkedIn**: [LinkedIn Profile](https://www.linkedin.com/in/rudrajitb/)  
- **GitHub**: [GitHub Profile](https://github.com/Rudrajit12)

---
