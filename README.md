# BoomBikes Bike Sharing Assignment

## **Problem Statement**

A bike-sharing system allows individuals to rent bikes for short periods, either for a fee or for free. Typically, users can borrow a bike from a computer-controlled dock by entering payment information, which unlocks the bike. They can then return the bike to another dock within the same system.

BoomBikes, a US bike-sharing provider, has experienced significant revenue declines due to the ongoing COVID-19 pandemic. Struggling to maintain its position in the market, the company is developing a strategic plan to boost its revenue once the lockdown ends and the economy recovers.

To prepare for a post-pandemic market, BoomBikes aims to understand the factors influencing bike demand across the nation. The goal is to tailor their services to meet customer needs, differentiate themselves from competitors, and maximize profits.

To achieve this, BoomBikes has hired a consulting firm to analyze the key variables affecting bike demand in the American market. Specifically, the firm seeks to identify:

The significant variables that predict bike demand.
How effectively these variables explain variations in bike demand.
The consulting firm has collected a comprehensive dataset detailing daily bike demand across the US, incorporating various meteorological and user-related factors.

**Business Goal**:

You are tasked with developing a model to predict the demand for shared bikes using the provided independent variables. This model will help management grasp how demand fluctuates with different factors, enabling them to adjust their business strategy to align with demand levels and customer expectations. Additionally, the model will offer valuable insights into the demand dynamics of new markets, aiding in strategic planning and decision-making.

## Table of Contents

- [General Info](#general-information)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Recommendations](#recommendations)
- [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

**Issues to Address:**

1. **Revenue Decline:** BoomBikes is experiencing significant drops in revenue because of the ongoing pandemic, prompting the need for a strategic response.
2. **Market Sustainability:** The company is finding it challenging to remain viable in the current market conditions, necessitating a well-considered business plan.
3. **Post-Lockdown Strategy:** BoomBikes seeks to boost revenue after the lockdown by gaining insights into bike demand in the post-quarantine period.

**Objectives:**
The objectives are to identify key variables affecting bike demand in the American market, determine the most important predictors, and develop a model to analyze demand fluctuations. This will aid in crafting adaptable business strategies and understanding demand dynamics for informed decision-making. To achieve these goals, the case study will construct a multivariate linear regression model using the provided [dataset](./day.csv).

The main objective is to pinpoint the key variables that substantially impact the prediction of shared bike demand and evaluate how well these variables capture the patterns in bike demand.

## Conclusions

- The equation of the best fit line is given by:
  - **_cnt_** = 4491.30 + 998.75 x **_yr_** + 178.28 x **_workingday_** + 1174.49 x **_temp_** - 429.07 x **_hum_** - 349.15 x **_windspeed_** + 344.84 x **_Summer_** + 526.80 x **_Winter_** + 234.70 x **_September_** + 159.98 x **_Sunday_**
- The close alignment of R2 and adjusted R2 values between the training and test sets (R2: 0.810 vs. 0.800 and Adjusted R2: 0.810 vs. 0.800) in a linear regression model indicates effective generalization. This similarity suggests the model avoids overfitting to the training data and is likely to perform consistently on new, unseen data.
- Bike demand is influenced by features such as **yr**, **workingday**, **temp**, **hum**, **windspeed**, **Summer**, **Winter**, **September**, and **Sunday**.
- Three key feature variables, **temp**, **yr**, and **Winter**, exhibit the highest coefficient values, indicating their significant impact.
- The RMSE values of **844** in the training set and **839** in the test set for a linear regression model indicate that the model is fitting well to the training data and generalizing reasonably to new, unseen data with a small difference between training and test set performance.

## Recommendations

- **Leverage High-Impact Features:** Focus on features such as **temp**, **yr**, and **Winter** as they exhibit the highest coefficient values, indicating significant impact on bike demand.

- **Seasonal Strategies:** Develop targeted marketing and pricing strategies for different seasons, particularly emphasizing promotions during **Summer** and **Winter**.

- **Optimize Operational Planning:** Adjust bike availability and distribution based on the significant features identified, optimizing resources for peak demand periods.

- **User Engagement on Weekends:** Capitalize on increased demand on **Sunday** by introducing special promotions or events to encourage bike usage during weekends.

- **Weather-Sensitive Promotions:** Implement weather-specific promotions or incentives to encourage bike usage during favorable weather conditions, addressing the impact of **temp**, **hum**, and **windspeed**.

- **New Market Insights:** Use the developed model to gain insights into demand dynamics in the American market, informing business strategies and positioning BoomBikes competitively.

- **Continuous Monitoring and Adaptation:** Regularly update the model with new data and adapt strategies based on evolving market conditions to ensure sustained revenue growth.

## Technologies Used

- [Python](https://www.python.org/) - version 3.11.4
- [Matplotlib](https://matplotlib.org/) - version 3.7.1
- [Numpy](https://numpy.org/) - version 1.24.3
- [Pandas](https://pandas.pydata.org/) - version 1.5.3
- [Seaborn](https://seaborn.pydata.org/) - version 0.12.2
- [Statsmodels](https://www.statsmodels.org/stable/index.html) - version 0.14.0
- [Scikit-Learn](https://scikit-learn.org/stable/) - version 1.3.0

## Acknowledgements

- This project was assigned as part of a graded module and was developed by [Shams CA](https://www.linkedin.com/in/shamshuddin-ca-15bb16144/)
- UpGrad tutorials on Linear Regression on the learning platform

## Contact

Created by [@Shams7264](https://github.com/Shams7264)

____
