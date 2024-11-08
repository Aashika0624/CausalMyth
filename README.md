# CausalMyth

## Overview

**CausalMyth** is a data science project developed for the Statistics for AI and Data Science coursework. The objective is to analyze the relationship between stork populations and human birth rates, testing the traditional folklore claim that storks deliver babies. By implementing regression models and employing bootstrap techniques, this project investigates whether there is a genuine causal relationship or if observed correlations are merely spurious.

## Objectives

- **Analyze Birth Rate Predictors:** Examine how different variables influence the number of births across various countries.
- **Compare Regression Models:** Implement and evaluate two regression models to determine the most effective predictors of birth rates.
- **Construct Confidence Intervals:** Use bootstrap techniques to estimate confidence intervals for model coefficients and performance metrics.
- **Debunk the Stork Myth:** Statistically assess the validity of the claim that stork populations affect human birth rates.

## Key Variables

- **Predictors:**
  - **Storks:** Number of breeding pairs of white storks in the country.
  - **Humans:** Human population of the country (millions).
  - **GDP per Capita:** Gross Domestic Product per capita (USD).
  - **Population Density:** Population density (millions per km²).

- **Target:**
  - **BirthRate:** Number of live births per year per 1,000 people.

## Key Findings

- **Regression Models:**
  - **Model 1 (Storks as Predictor):**
    - **R-squared:** 0.385
    - **Interpretation:** Storks explain 38.5% of the variance in birth rates. However, the high RMSE and moderate R-squared indicate a weak predictive relationship.
  
  - **Model 2 (Socioeconomic Predictors):**
    - **R-squared:** 0.774
    - **Interpretation:** Socioeconomic factors explain 77.4% of the variance in birth rates, significantly outperforming Model 1.
  
- **Bootstrap Confidence Intervals:**
  - **GDP per Capita:**
    - **95% CI:** [-0.0229, 0.0009]
    - **Interpretation:** The interval slightly overlaps zero, suggesting a marginally significant negative effect on birth rates.
  
  - **Population Density:**
    - **95% CI:** [-4,599,193.00, 567,075.51]
    - **Interpretation:** The wide interval includes zero, indicating high uncertainty and no consistent effect on birth rates.
  
- **Chi-Square Test:**
  - **Result:** Significant association between regions and the direction of flat price changes (p-value < 0.001).
  - **Interpretation:** Flat price changes vary significantly across different regions, rejecting the null hypothesis of uniform behavior.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib & Seaborn
- Scikit-learn
- SciPy

## Conclusion

The **CausalMyth** project effectively debunks the whimsical claim that storks deliver babies by demonstrating that socioeconomic factors, rather than stork populations, significantly influence birth rates. Regression analysis revealed that while storks show a moderate correlation with birth rates, they do not provide a meaningful predictive relationship. In contrast, factors such as population size and GDP per capita offer robust explanations for variations in birth rates. Bootstrap confidence intervals further reinforced the limited significance of stork populations, highlighting the importance of selecting relevant and theoretically grounded predictors in statistical modeling. This analysis underscores the critical distinction between correlation and causation, emphasizing the need for rigorous data analysis to uncover true underlying relationships.

