![pic2_thumbnails](https://user-images.githubusercontent.com/81752452/177544105-858b035e-5f6a-4dec-9d82-742f22e66536.png)

*Summary*

This project analyses the factors related to life expectancy based on a public dataset from WHO. The data was collected between 2000 and 2015. Studied factors include development status of a country, GDP, population, schooling years, alcohol consumption, BMI, government expenditure on health, per-capital expenditure on health, various immunisation coverage, thinness disease, measles cases, HIV/AIDS deaths, and mortality rate of adult, children, and infants.

During data processing, data were thoroughly checked (horizontally and vertically), cleaned, and transformed. Missing values were imputed using Bagged-trees algorithm. During exploratory data analysis (EDA), box and whisker plot, histogram, and multiple factor analysis (MFA) were applied to explore and mine the overall trends within the data. MFA is an unsupervised machine learning technique. 8 questions were designed and answered statistically in this project. Depending on the nature of each question, multiple analysis techniques were applied such as multiple linear regression, correlation matrix, VIF, assumption diagnostic plots, Welch’s t-test, principal component analysis (PCA), Shapiro-wilk test, Wilcoxon signed-rank test, and longitudinal multilevel mixed-effect modelling.

Multiple linear regression model that passed the assumption tests shown that the positively correlated significant variables (p < 0.05) in relation to life expectancy are schooling (Coeff. Est: 1.15), total expenditure by government on health (Coeff. Est: 0.08), BMI (0.03), GDP (Coeff. Est: 0.00004), and the immunisation of Diphtheria (Coeff. Est: 0.03) and Polio (Coeff. Est: 0.02), whereas, the negatively correlated significant variables (p < 0.05) are developing country status (Coeff. Est: -1.12), HIV/AIDS Death rate (Coeff. Est: -0.51), Adult mortality rate (Coeff. Est: -0.02), and infant deaths (Coeff. Est: -0.002) (adjusted R-squared: 0.85, F(15, 2775) = 1087, p < 0.001). A partial analysis from the full model of longitudinal multilevel modeling supports similar outcomes and it detected that if a country has lower initial life expectancy in year-2000, it would have a higher rate in life expectancy improvement across the year between 2000 and 2015 (intercept-slope corr = -0.55). It implies improvement of life expectancy in developing countries that associated with lower life expectancy since 2000 to 2015. The full model also concludes that life expectancy of human increases each year by 0.25 year on average, with a confidence level between 0.16 year and 0.34 year (p < 0.001).


*Highlight*

![pic1_graphs](https://user-images.githubusercontent.com/81752452/177544076-757abeb7-5007-4e82-a5a4-fdea229077ca.png)

*Reference*

Anderson D.R., Sweeney D.J, Williams T.A., 2006, Essentials of Statistics for Business & Economics, South-Western, Division of Thomson Learning, United States of America

Bruce, Peter, and Andrew Bruce. 2017. Practical Statistics for Data Scientists. O’Reilly Media.

James, Gareth, Daniela Witten, Trevor Hastie, and Robert Tibshirani. 2014. An Introduction to Statistical Learning: With Applications in R . Springer Publishing Company, Incorporated.

Kassambara.A 2018, Machine Learning Essentials: Practical Guide in R, eBook.

Kassambara.A n.d., COMPARING MULTIPLE MEANS IN R, viewed 1 July 2022, https://www.datanovia.com/en/lessons/ancova-in-r/#two-way-ancova

Kumarrajarshi 2018, “Life Expectancy (WHO)”, viewed 23 June 2022, https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who
