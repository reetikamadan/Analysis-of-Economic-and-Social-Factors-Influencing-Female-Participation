# Analysis of Economic and Social Factors Influencing Female Participation using Python

## Overview
This project explores the economic and social factors that influence female participation in education, the labor force, and leadership roles. Using statistical and machine learning techniques, I analyzed global datasets to uncover key drivers and relationships. The project is divided into three main analyses, followed by an exploration of feature importance.

## 1. Regression Analysis: Factors Influencing Female Tertiary Enrollment
This section examines the key factors driving female tertiary enrollment rates.

### Variables Analyzed:
- Female Literacy Rate  
- Government Expenditure Per Tertiary Student  
- GDP Per Capita  
- Female Population  
- Household Consumption Growth  

### Steps:
1. Ran a multiple linear regression model to examine the direct effects of these variables on tertiary enrollment.  
2. Introduced an interaction term between Female Literacy Rate and Female Population to capture joint effects.  
3. Evaluated model performance:  
   - **R-squared (with interaction term):** 0.746  
   - **Significant predictors:** GDP Per Capita, Female Literacy Rate, and the interaction term.  

### Key Insight:
Economic development (GDP per capita) and literacy initiatives are crucial for improving female tertiary enrollment, especially in countries with larger female populations.

---

## 2. Analyzing the Effect of Female Labor Force Participation on GDP
This section investigates how female labor force participation impacts economic growth using a **fixed effects panel regression** model.

### Steps:
1. Used a dataset with 25 time periods across 217 entities (countries/regions).  
2. Conducted a fixed effects regression to control for country-specific unobserved factors.  
3. Key variable analyzed: **Female Labor Force Participation Rate.**  

### Results:
- Each percentage point increase in female labor force participation is associated with an increase of approximately **$698 in GDP per capita.**  
- **Model R-squared (Within):** 0.1325  

### Key Insight:
Increasing female labor force participation has a significant positive impact on economic growth, highlighting the need for policies that promote workforce inclusion for women.

---

## 3. Analysis of Female Participation as Legislators, Senior Officials, and Managers
This section examines the factors influencing female representation in leadership roles using machine learning techniques.

### Steps:
1. Started with **30–40 variables** and used backward elimination to select the most relevant predictors.  
2. Applied machine learning models:  
   - **Decision Tree Regressor**  
   - **Bagging Regressor**  
   - **Boosting Regressor**  
   - **Random Forest Regressor**  
3. Evaluated model performance using RMSE (Root Mean Squared Error) and MAPE (Mean Absolute Percentage Error).  

### Results:
- **Best model:** Bagging Regressor (RMSE: 0.9046, MAPE: 1.43%).  
- **Key predictors identified through feature importance:**  
  - Female Population (% of total population)  
  - Gross National Expenditure  
  - Youth Unemployment Rate  

### Key Insight:
Demographic factors like population size and economic indicators such as national expenditure are critical for understanding women's representation in leadership roles.

---

## 4. Feature Importance Analysis
To further understand what drives female participation in leadership roles, I conducted a feature importance analysis using machine learning models.

### Steps:
1. Identified the most influential variables affecting female leadership representation.  
2. Generated **partial dependency plots** to visualize how key features impact predictions.  

### Key Findings:
- **Female Labor Force Participation:** Leadership representation increases significantly when women make up at least **50% of the labor force**.  
- **Gross Enrollment Ratio in Tertiary Education:** A sharp increase in leadership representation is observed when more than **50% of women enroll in higher education**.  
- **Employment-to-Population Ratio:** Stable relationship up to **45%**, with slight declines beyond this point.  

### Key Insight:
Access to **higher education** and **workforce inclusion** are critical for increasing women's representation in leadership roles.

---

## Project Highlights
### 📊 Comprehensive Analysis:
- Explored three interconnected areas—education, labor force participation, and leadership roles.  
- Used **advanced statistical techniques (regression)** and **machine learning models** to uncover insights.  

### 📈 Policy Implications:
- The findings emphasize the importance of investing in **women’s education, workforce inclusion, and leadership opportunities**.  
- These efforts can lead to **higher GDP growth** and **greater gender equality**.  

### 📌 Visualizations:
- Included **feature importance charts** and **partial dependency plots** to provide clear insights into how key variables influence outcomes.

---

