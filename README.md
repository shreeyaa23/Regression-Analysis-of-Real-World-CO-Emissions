#  **Regression Analysis of Real-World CO₂ Emissions**

##  **Overview**
This project analyzes **real-world vehicle CO₂ emissions** using data from the **U.S. Environmental Protection Agency’s Automotive Trends Report (1975–2009)**.  
The goal was to identify **key vehicle characteristics** influencing CO₂ output and to build a **predictive linear regression model** capable of quantifying their environmental impact.

The analysis achieved an **R² of 0.9872**, explaining **98.7% of the variation** in emissions, confirming exceptional predictive strength.

---

##  **Objectives**
- Model the relationship between **vehicle attributes** and **CO₂ emissions (g/mi)**.  
- Identify **high-impact predictors** such as fuel efficiency, engine displacement, and weight.  
- Evaluate **model performance and diagnostic validity**.  
- Propose **sustainable design recommendations** for emission reduction.

---

##  **Dataset Details**
- **Source:** U.S. EPA Automotive Trends Report  
- **Years Covered:** 1975 – 2009  
- **Records Analyzed:** 4,162 observations  
- **Variables Used:**  
  - Transmission Type (Automatic / Manual)  
  - Vehicle Weight (lbs)  
  - Engine Displacement (L)  
  - Horsepower (HP)  
  - Cylinders  
  - Miles Per Gallon (Real-World MPG)  
  - CO₂ Emissions (Dependent Variable)

---

##  **Analytical Framework**

### **1️ Data Preparation**
- Cleaned and standardized dataset using **SAS Studio (Linux Environment)** and **Excel**.  
- Handled missing values and ensured consistent unit scaling.  
- Validated dataset integrity through **correlation matrices** and **multicollinearity checks**.

### **2️Model Development**
- Applied **multiple linear regression** in **SAS 9.04** to predict `RealWorld CO₂ (g/mi)`.  
- Model equation:
CO₂ = β₀ + β₁(Transmission) + β₂(Weight) + β₃(Engine Displacement)
+ β₄(Horsepower) + β₅(Cylinders) + β₆(MPG) + ε

- Diagnostic plots: Residuals, Q-Q, Leverage, and Observed vs Predicted.  

### **3️ Key Predictors Identified**
| Predictor | Impact on CO₂ | p-Value |
|------------|---------------|---------|
| **Miles Per Gallon (MPG)** | ↓ Strong negative correlation (most significant) | < 0.0001 |
| **Vehicle Weight (lbs)** | ↑ Increases emissions | < 0.0001 |
| **Engine Displacement (L)** | ↑ Higher displacement → higher emissions | < 0.0001 |
| **Horsepower** | Slight negative contribution when controlled for MPG | < 0.0001 |
| **Transmission Type** | Automatic > Manual in emissions | < 0.0001 |

---

##  **Model Performance**
| Metric | Value | Interpretation |
|---------|--------|----------------|
| **R-Square** | **0.9872** | 98.7% of emission variance explained |
| **Adj. R²** | **0.9872** | Minimal overfitting |
| **Root MSE** | **20.29** | Low residual error |
| **F-Value** | **45,816 (p < 0.0001)** | Highly significant model |

 **Diagnostics:**  
- Residuals normally distributed (validated via Q-Q plot).  
- Minimal leverage points and outliers.  
- Excellent fit between observed vs predicted CO₂ values.

---

##  **Environmental Insights**
- Improving **fuel efficiency (MPG)** is the single most impactful factor in reducing CO₂ emissions.  
- Reducing **vehicle weight** and **engine displacement** lowers emissions significantly.  
- Future vehicle designs should focus on **lightweight materials**, **efficient transmissions**, and **hybrid technologies**.

---

##  **Tools & Technologies**

| Tool | Purpose |
|------|----------|
| **SAS Studio 3.8 (PROC REG)** | Linear regression modeling & diagnostics |
| **Excel / Power Query** | Data cleaning & preparation |
| **Python (Matplotlib, Pandas)** *(optional)* | Visualization & validation |
| **Power BI / Tableau** | Post-analysis visualization of emission patterns |

---

##  **Key Results**
- Model explained **98.7%** of emission variability across 4,162 vehicles.  
- Identified **MPG** as the dominant predictor, followed by **weight** and **engine displacement**.  
- Recommended design and policy changes that can **reduce emissions by up to 20–25%** through efficiency improvements.  

---

##  **Recommendations**
1. **Adopt lightweight vehicle materials** to improve fuel efficiency.  
2. **Enforce stricter emission regulations** and periodic testing.  
3. **Incentivize low-emission / hybrid vehicle adoption.**  
4. **Enhance consumer transparency** via clear emissions labeling.  
5. **Continuously update datasets** for model recalibration and validation.

---

##  **Author**
**Shreya Mishra**  
*Business Intelligence & Data Analyst*  
Richmond, VA  
MBA (Business Analytics) | SAS | Excel | Power BI | Python | Tableau 

---

