# Regression Analysis of Real-World CO₂ Emissions

**Author:** Shreya Mishra  
**Location:** Richmond, VA  
**Tools:** SAS Studio | Excel | Power BI | Python | Tableau  

---

## Overview
This project analyzes real-world vehicle CO₂ emissions using data from the **U.S. Environmental Protection Agency’s Automotive Trends Report (1975–2009)**.  
The objective was to identify key vehicle characteristics influencing CO₂ output and to build a predictive linear regression model capable of quantifying their environmental impact.

The final model achieved an **R² of 0.9872**, explaining **98.7% of the variation in emissions**, confirming exceptional predictive strength.

---

## Objectives
- Model the relationship between vehicle attributes and CO₂ emissions (g/mi).  
- Identify high-impact predictors such as fuel efficiency, engine displacement, and vehicle weight.  
- Evaluate model performance and diagnostic validity.  
- Provide actionable design recommendations for emission reduction.

---

## Dataset Details
| Attribute | Description |
|------------|-------------|
| **Source** | U.S. EPA Automotive Trends Report |
| **Years Covered** | 1975 – 2009 |
| **Observations** | 4,162 |
| **Key Variables** | Transmission Type, Vehicle Weight, Engine Displacement, Horsepower, Cylinders, MPG, CO₂ Emissions |

---

## Analytical Framework

### 1. Data Preparation
- Cleaned and standardized dataset using **SAS Studio (Linux)** and **Excel Power Query**.  
- Handled missing values and verified unit consistency.  
- Checked correlations and multicollinearity before regression.

### 2. Model Development
Applied **Multiple Linear Regression (PROC REG)** in SAS 9.04 to predict real-world CO₂ emissions:

\[
CO₂ = β₀ + β₁(\text{Transmission}) + β₂(\text{Weight}) + β₃(\text{Displacement}) + β₄(\text{Horsepower}) + β₅(\text{Cylinders}) + β₆(\text{MPG}) + ε
\]

**Diagnostics performed:**
- Residuals vs Fitted and Q-Q plots  
- Leverage and influence statistics  
- Observed vs Predicted CO₂ visualization  

---

## Key Predictors

| Predictor | Impact on CO₂ | p-Value |
|------------|---------------|---------|
| **Miles Per Gallon (MPG)** | ↓ Strong negative correlation | < 0.0001 |
| **Vehicle Weight (lbs)** | ↑ Increases emissions | < 0.0001 |
| **Engine Displacement (L)** | ↑ Direct positive effect | < 0.0001 |
| **Horsepower** | Slight negative (controlled for MPG) | < 0.0001 |
| **Transmission Type** | Automatic > Manual | < 0.0001 |

---

## Model Performance

| Metric | Value | Interpretation |
|---------|--------|----------------|
| **R²** | 0.9872 | 98.7% variance explained |
| **Adj R²** | 0.9872 | Minimal overfitting |
| **Root MSE** | 20.29 | Low residual error |
| **F-Value** | 45,816 (p < 0.0001) | Highly significant model |

**Diagnostics:**  
- Residuals approximately normal (Q-Q plot).  
- Minimal leverage and outliers.  
- Excellent alignment between observed and predicted CO₂.

---

## Environmental Insights
- **Fuel efficiency (MPG)** is the single most influential factor in emission reduction.  
- Lighter vehicle materials and smaller engine displacement substantially lower emissions.  
- Promotes sustainable automotive design and hybrid adoption.  

---

## Tools & Technologies
| Tool | Purpose |
|------|----------|
| **SAS Studio 3.8 (PROC REG)** | Regression modeling & diagnostics |
| **Excel / Power Query** | Data cleaning & transformation |
| **Python (pandas, matplotlib)** | Visualization & validation |
| **Power BI / Tableau** | Post-analysis dashboards |

---

## Key Results
- Model explained **98.7%** of CO₂ variability across 4,162 vehicles.  
- Identified **MPG, weight, and displacement** as primary emission drivers.  
- Recommended design improvements that can reduce emissions by 20–25%.  

---

## Recommendations
- Adopt lightweight materials and efficient transmission systems.  
- Enforce stricter emission and fuel-efficiency regulations.  
- Incentivize adoption of hybrid or low-emission vehicles.  
- Continuously recalibrate models with updated EPA data.

---

## Project Type
**Statistical Modeling · Regression Analysis · Environmental Analytics**
