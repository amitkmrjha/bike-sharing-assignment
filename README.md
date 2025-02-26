# BoomBikes Bike Sharing Assignment

## **Problem Statement**

A bike-sharing system is a service that provides bicycles for shared use, allowing individuals to rent them for a short period, either for a fee or free of charge. Many bike-sharing programs operate through computer-controlled docking stations, where users enter payment details to unlock a bike. The rented bike can then be returned to any other dock within the same system.

Recently, the US-based bike-sharing company BoomBikes has experienced a significant decline in revenue due to the ongoing COVID-19 pandemic. The company is struggling to stay afloat in the current market conditions. To address this challenge, BoomBikes is developing a strategic business plan to boost revenue as soon as lockdown restrictions are lifted and the economy recovers.

As part of this initiative, BoomBikes aims to analyze the anticipated demand for shared bikes once the quarantine period ends nationwide. By gaining insights into customer needs, the company hopes to position itself ahead of competitors and maximize profits.

To achieve this, BoomBikes has engaged a consulting firm to identify the key factors influencing bike-sharing demand in the U.S. market. Specifically, they seek to understand:

Which variables significantly impact the demand for shared bikes.
The extent to which these variables explain fluctuations in bike demand.
To support this analysis, the company has collected an extensive dataset on daily bike rentals across the American market, incorporating various meteorological and lifestyle factors.

**Business Goal**:

You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

## Table of Contents

- [General Info](#general-information)
- [Technologies Used](#technologies-used)
- [Conclusions](#conclusions)
- [Recommendations](#recommendations)
- [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information

**Issues to Address:**

1. **Revenue Decline:** BoomBikes faces substantial revenue declines due to the ongoing pandemic, necessitating a strategic solution.
2. **Market Sustainability:** The company struggles to sustain itself in the current market scenario, demanding a mindful business plan.
3. **Post-Lockdown Strategy:** BoomBikes aims to accelerate revenue post-lockdown, requiring an understanding of post-quarantine bike demand.

**Objectives:**
The objectives include predicting significant variables influencing American market shared bike demand, determining the crucial predictors, developing a model to understand demand variations, facilitating adaptive business strategies, and exploring demand dynamics for effective decision-making. This case study aims to achieve this goal by building a multivariate linear regression model using the provided [dataset](./day.csv).

The primary objective is to identify the key variables that significantly influence the prediction of shared bike demand and assess how effectively these variables describe the patterns in bike demands.

## Conclusions

- The equation of the best fit line is given by:
  -cnt = 0.53 + 0.25yr + 0.06workingday - -0.19windspeed - .26season_spring - 0.04season_summer - 0.07season_winter -0.1mnth_jan + 0.7mnth_Sep + 0.06weekday_Sat -0.30weathersit_Light Snow & Rain -0.09weathersit_Mist & Cloudy
- T- **Model Generalization:** The close alignment of **R²** and **Adjusted R²** values between the training and test sets (**R²: 0.78 vs. 0.77**, **Adjusted R²: 0.74) suggests effective generalization. This indicates that the model avoids overfitting and is likely to perform well on new data.  

- **Key Influencing Factors:** Bike demand is influenced by variables such as **yr, workingday, Light Snow & Rain, windspeed, Spring,**

- **Most Significant Features:** The variables ** yr, and Light Snow & Rain** have the highest coefficient values, highlighting their strong impact on bike demand.  

- Bike demand is influenced by features such as **yr**, **workingday**, **windspeed**, **Summer**, **Winter**, **September**, and **Sunday**.
- Three key feature variables, , **yr**, and **Winter**, exhibit the highest coefficient values, indicating their significant impact.

## Recommendations

- **Leverage High-Impact Features:** Focus on features such as  **yr**, and **Winter** as they exhibit the highest coefficient values, indicating significant impact on bike demand.

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

- This project was inspired by live session of upGrad on Industry Relevance of Linear Regression Models by [Shivam Garg](https://www.linkedin.com/in/shivam-garg-0494a2ab/)
- UpGrad tutorials on Linear Regression on the learning platform

## Contact

Created by [@akashkriplani](https://github.com/akashkriplani)