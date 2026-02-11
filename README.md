# 🏥 US Healthcare Analysis: Cost Drivers & Demographic Trends

![Excel](https://img.shields.io/badge/Tools-Microsoft%20Excel-green) ![Status](https://img.shields.io/badge/Status-Completed-blue)

## 📌 Executive Summary
**The Myth:** High hospital bills are caused by expensive medication.
**The Reality:** The primary driver of cost is the **Medical Condition**, with Cancer treatments costing **300% more** than other conditions. Medication choice only accounts for a ~5% variance in total cost.

This project analyzed 10,000 patient records to identify the root causes of rising healthcare costs. By cleaning complex data anomalies and performing demographic segmentation, I developed a strategy shifting focus from "Cost Cutting" to **"Preventative Care"** for high-risk groups.

---

## 📂 Business Problem
The US Healthcare Department provided a dataset of 10,000 patients from 100 hospitals. The stakeholders required an analysis to answer two critical questions:
1.  **Who is getting sick?** (Demographic Analysis)
2.  **What is driving the cost?** (Price Optimization)

**Objective:** Derive actionable insights to improve hospital resource allocation and reduce patient costs.

---

## 🛠️ Data Cleaning & Preparation (The "Hidden" Work)
Before analysis, the dataset required a granular manual audit to correct human-entry errors that automation might have missed.

**Key Cleaning Steps:**
* **Typos in Numerical Data:** Identified and corrected entries where Age was written as `"8I"` instead of `"81"`. This prevented skewing of age-based averages.
* **Standardization:** Merged inconsistent categories:
    * Gender: `M` → `Male`
    * Blood Type: `A+ve` → `A+`
* **Sampling:** Performed random sampling to verify data distribution and ensure statistical significance before full-scale analysis.
* **Bucketing:** Created Age Groups (Young, Middle Age, Old, Very Old) to make the analysis readable for non-technical stakeholders.

---

## 📊 Key Insights

### 1. Demographic Analysis (Who is at risk?)
* **Young Adults (18-25):** The data shows a spike in **Asthma** cases.
* **Elderly Women:** **Arthritis** is the dominant condition.
* **Males (All Ages):** **Hypertension** shows a linear increase correlating with age.

![Insert Screenshot of Dashboard 1 - Demographics]

### 2. Price Optimization (The "Aha!" Moment)
My initial hypothesis was that expensive drugs (like Lipitor) were driving up bills. However, a deep-dive comparison revealed:

| Metric | Average Cost | Variance |
| :--- | :--- | :--- |
| **Drug: Lipitor** | $24,204 | -- |
| **Drug: Paracetamol** | $22,810 | **~5% Difference** |
| **Condition: Cancer** | **$39,677** | -- |
| **Condition: Obesity** | $12,544 | **~216% Difference** |

**Conclusion:** The medication prescribed has a negligible impact on the final bill compared to the Medical Condition itself.

![Insert Screenshot of Dashboard 2 - Price Analysis]

---

## 💡 Recommendations
Based on the data, cutting medication costs will not solve the financial issue. The strategy must change:

1.  **Invest in Preventative Care:** Launch targeted awareness programs for **Asthma (Young Adults)** and **Arthritis (Elderly Women)**.
2.  **Early Detection:** Implement screening programs for high-cost conditions like **Cancer** and **Diabetes**. Catching these early prevents the $39k+ treatments associated with late-stage care.
3.  **Resource Allocation:** Shift budget from "Medication Subsidies" to "Screening Infrastructure."

---

## 💻 Tools Used
* **Microsoft Excel:**
    * **Data Cleaning:** Logic formulas (`IF`, `TRIM`, `SUBSTITUTE`) to fix "8I" and blood type errors.
    * **Pivot Tables:** Used for multi-variable segmentation (Age vs. Condition).
    * **Statistical Sampling:** To validate data integrity.
    * **Dashboarding:** Created interactive views for stakeholder presentation.

---

