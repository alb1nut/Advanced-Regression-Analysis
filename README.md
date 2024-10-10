# Advanced Regression Analysis 

## Project Overview

This project focuses on conducting advanced regression analysis using the **Salaries** dataset from the `car` package in R. The aim is to explore relationships between different variables such as **salary**, **gender**, **academic rank**, **discipline**, and **years since PhD**. By fitting various linear models and analyzing the results, we gain insights into how these factors impact salaries in academia.

## Key Objectives

1. **Visualization**:
   - The project begins with visualizing the distribution of salaries after applying a logarithmic transformation. Both histogram and Q-Q plots are used to assess the normality of the data.

2. **Linear Regression Models**:
   - A linear regression model is fitted to predict the logarithm of salary using several predictors: **gender**, **rank**, **discipline**, and **years since PhD**.
   - A secondary linear model is constructed to examine whether the effect of years since PhD on salary differs by gender.

3. **Coefficient Visualization**:
   - The coefficients from the linear models are visualized to provide an intuitive understanding of the magnitude and direction of the effects of each predictor.

4. **Relative Importance Analysis**:
   - The relative importance of each predictor is computed using the `relimpo` package. Two different metrics, **LMG** and **CAR**, are used to determine the relative contributions of the predictors in explaining salary variation.

## Key Insights

- **Significant Predictors**: The analysis identifies statistically significant predictors, including **rank** and **discipline**, which have the greatest impact on salary.
- **Gender Differences**: The interaction between **gender** and **years since PhD** does not show a significant difference, indicating that the effect of experience on salary is similar across genders.
- **Relative Importance**: The **rank** of the individual, particularly being a **Professor**, has the highest relative importance in predicting salary, followed by **discipline** and **years since PhD**.

## Methodology

The analysis involves several key steps:
1. **Data Transformation**: Salaries are log-transformed to meet the assumptions of linear regression.
2. **Model Fitting**: Linear regression models are fitted to the log-transformed data.
3. **Visualization**: Coefficients of the predictors are visualized using the `coefplot` function to aid interpretation.
4. **Relative Importance**: Using `relimpo`, the relative importance of each predictor is computed, offering different perspectives on which factors most significantly influence salary.

## Conclusion

This project demonstrates the application of regression techniques to real-world data to uncover key drivers of salary disparities in academia. By utilizing both standard linear models and advanced metrics for relative importance, we provide a comprehensive analysis of the factors influencing academic salaries.

## Tools and Packages Used

- **R Programming Language**
- **car**: For the `Salaries` dataset and linear modeling.
- **coefplot**: To visualize model coefficients.
- **relaimpo**: For calculating the relative importance of predictors.

## Future Directions

- **Exploring Non-linear Models**: Future work could involve exploring non-linear relationships between predictors and salary to capture more complex patterns.
- **Additional Predictors**: Incorporating more features related to institutional characteristics or personal achievements could improve model accuracy.
- **Cross-validation**: Applying cross-validation techniques to evaluate model performance on unseen data.

## Author

Albert Nutifafa Dovlo
