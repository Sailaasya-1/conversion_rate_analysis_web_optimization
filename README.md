# 📊 Conversion Rate Analysis for Web Optimization (A/B Testing)

## Project Overview
This project analyzes a large-scale A/B experiment conducted on 290,000 users to evaluate whether a new webpage design improves user conversion rates.

Using statistical hypothesis testing and logistic regression, we determine whether the treatment page significantly increases conversions compared to the existing (control) page.

Dataset source: Udacity Data Analyst Nanodegree. (https://www.udacity.com/course/data-analyst-nanodegree--nd002)

---

## 🎯 Business Objective
To answer:

- Does the new webpage increase conversion rate?
- Is the observed lift statistically significant?
- Should the new design be rolled out?

---

## 📐 Hypothesis Testing

We formally tested:

H₀: p_new ≤ p_old  
H₁: p_new > p_old  

A one-tailed hypothesis test was conducted to evaluate whether the new page improves conversion.

Result:

- **p-value = 0.19**
- Failed to reject the null hypothesis
- No statistically significant improvement observed

---

## 📈 Logistic Regression Model

To validate results using a model-based approach:

log(p / (1 - p)) = β₀ + β₁ * ab_page

Where:
- β₀ → Baseline (control group) conversion log-odds
- β₁ → Treatment effect

The regression results aligned with the hypothesis test, confirming no significant treatment effect.

---

## 🌍 Country-Level Analysis

Additional analysis examined conversion differences across:

- US
- UK
- CA

Country effects were explored to assess potential confounding factors.

---

## 🛠 Tools & Technologies

- Python
- Pandas
- NumPy
- Statsmodels
- Matplotlib

---

## 📊 Key Insight

Despite the large sample size, the new webpage did not produce a statistically significant lift in conversions. 

📌 Recommendation: Retain the existing design and avoid premature rollout.

---

## 🚀 How to Run

1. Clone the repository
2. Install dependencies
3. Run the Jupyter notebook or Python script

---

