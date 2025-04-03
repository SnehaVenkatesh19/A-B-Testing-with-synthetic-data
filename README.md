# 📊 A/B Testing: Web Page Design Impact on Conversion

## 📌 Objective
To evaluate the impact of a new webpage design (treatment) versus the original design (control) on user conversions using A/B testing. The project includes statistical testing, confidence intervals, regression analysis, and Tableau dashboarding.

---

## 📊 Dataset
- **Source**: Synthetic dataset (5,000 user sessions)
- **Fields**:
  - `group` — A/B group (control or treatment)
  - `converted` — Whether the user converted (0 or 1)
  - `revenue` — Revenue earned (if converted)
  - `trial_to_paid` — Whether the user upgraded from trial
  - `device`, `source` — User metadata for segmentation

---

## 🔬 Methodology

### 1. Exploratory Data Analysis
- Assessed conversion, revenue, trial upgrade rate
- Compared funnel metrics across A/B groups

### 2. Statistical Testing
- **Z-tests** for conversion rate differences
- **95% Confidence Intervals** for conversion and revenue
- Segmented analysis by device and user source

### 3. Regression Modeling
- **Logistic regression**:
  - Modeled `converted` ~ `group` + `device` + `source`
- **Linear regression**:
  - Modeled `revenue` (converted only) ~ predictors
- Included **interaction terms** to detect conditional effects

---

## 📈 Tableau Dashboard Highlights

-  Conversion Rate by Group  
-  Avg Revenue by Group (Converted Only)  
-  Trial-to-Paid Rate Comparison  
-  Revenue Distribution Histogram  

> Here's the Dashboard : https://public.tableau.com/app/profile/sneha.venkatesh3644/viz/AB_testing_synthetic_data/Dashboard1

---

## 📌 Key Insights

- Treatment group saw a **3% uplift** in conversion and **~10% revenue increase**
- Changes were **not statistically significant** (p > 0.05)  
- Strong **directional trends** suggest potential success with higher traffic
- Mobile users showed higher responsiveness to the new design

---


