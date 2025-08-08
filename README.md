# The Effects on San Francisco Residents Choosing to Own a Home

**Author:** Kiara Dorion  
**Course:** ECON 611 – Computation for Economics  
**Institution:** University of San Francisco  
**Term:** Fall 2024  

---

## 📌 Project Overview
This project investigates the key factors influencing San Francisco residents’ decisions to own a home. Using survey data from the City and County of San Francisco, a **binary logistic regression model** was developed to quantify the impact of demographic, household, and perception-based variables on the probability of homeownership.

The analysis uses **Maximum Likelihood Estimation (MLE)** to fit the model and includes detailed goodness-of-fit diagnostics, predictive probability analysis, and policy-relevant insights.

---

## 📊 Dataset
**Source:** [San Francisco City Survey Data](https://data.sfgov.org/City-Management-and-Ethics/San-Francisco-City-Survey-Data/nufj-bfbw/about_data)  
**Description:** The dataset contains demographic and perception metrics collected from residents through city surveys.  

**Variables Used:**
1. **dem_homeown** – Dependent variable (binary: Own = 1, Not Own = 0 after dummy conversion)  
2. **dem_hhsize** – Number of household members  
3. **child_05** – Number of children aged 0–5 in the household  
4. **child_617** – Number of children aged 6–17 in the household  
5. **safe_day** – Perceived neighborhood safety during the day (1–5 scale)  
6. **safe_polqual** – Perceived quality of police services (1–5 scale)  
7. **dem_gender** – Gender of respondent (encoded as numeric after conversion)  

---

## 🛠 Methodology
1. **Data Preparation**
   - Selected relevant columns
   - Handled missing values with listwise deletion
   - Converted categorical variables to numeric dummy variables
2. **Model Specification**
   - Binary logistic regression estimated via MLE
   - Predictor variables included household demographics and perception indices
3. **Evaluation Metrics**
   - Log-Likelihood
   - Pseudo R²
   - Likelihood Ratio Tests
4. **Prediction**
   - Calculated predicted probabilities of homeownership
   - Visualized effects of significant predictors

---

## 📈 Key Findings
- **Household size** has a positive and statistically significant effect on homeownership likelihood.
- **Number of children (both 0–5 and 6–17)** in a household increases the probability of homeownership.
- **Perceived daytime safety** and **quality of police services** are positively correlated with ownership decisions.
- **Gender** effect was weaker but still noted, with male respondents slightly more likely to own homes in the sample.

---

## 📦 Technologies Used
- **Python** (pandas, numpy, statsmodels, matplotlib, scipy)
- **Jupyter Notebook**
- **San Francisco Open Data Portal**

---

## 📂 Repository Structure
