# Enhancing Happiness through Financial Well-being - Equinox

<p align="center"><img src="https://therightnewsnetwork.com/wp-content/uploads/2019/03/TRNN-Revelations-Finance.png" /></p>

Table of Contents :bookmark_tabs:
=================
- [Executive Summary](#executive-summary)
- [Introduction](#introduction)

## Executive Summary
This report aims to identify solutions and business recommendations to help the Ministry of Social and Family Development (MSF) better identify people with poor financial well-being which tends to lead to unhappiness. 

Singapore is reputed for its high Gross Domestic Product (GDP) per capita, life expectancy, and integrity. Yet, it has a relatively low happiness level at 31st ranking in the world. To improve happiness in Singapore, our team has chosen to target an aspect that the Singapore Government can likely influence and intervene in. The aspect is financial well-being in which freedom to make life choices is a significant factor.

We adopted a data-driven approach to analyze the personal data that the government collects to aggregate a more holistic judgment of one’s financial well-being through the usage of machine learning and artificial intelligence techniques. Data preprocessing steps such as data cleaning, discretization of the target variable (“At risk” and “Not at risk”), and feature selection were performed followed by data transformation before feeding into the machine learning models. Following that, we developed 7 machine learning models for binary classification: logistic regression, decision tree classifier, random forest classifier, XGBoost classifier, support vector classifier, Bernoulli naïve Bayes classifier, and neural network. A 70:30 train-test split was used to partition the data set for evaluation purposes. Hyperparameter tuning was performed on the training data set to extract the optimal performance out of the models.

The 7 machine learning models were evaluated using various evaluation metrics such as accuracy, precision, recall, and F1-Score. F1-Score was chosen as the final criteria for model selection to account for imbalanced data and the cost of misclassification. All the models managed to beat the baseline F1-Score which was calculated to be at 0.3333. Support vector classifier emerged as the winner providing the highest F1-Score at 0.7194. As such, the support vector classifier was chosen to be recommended to MSF. 

A few business recommendations were proposed to utilize the machine learning model. Firstly, ideas were developed to facilitate the application of the proof of concept to the actual dataset and identify the target group to assist. Secondly, to simplify the workflow for MSF’s transition into interacting with our machine learning model, a graphical user interface was proposed. They can directly export the collected data into the system and the candidates who belong to the “At risk” group along with the relevant information will be generated automatically. Thirdly, a longitudinal study can be conducted to evaluate the efficacy of the intervention by MSF.

The limitations of the data and models were discussed. Limitations of models include the tradeoff between interpretability and predictability and the difficulty in predicting social and dynamic systems. Suggested future work includes survey questions reduction using a randomized approach to reduce survey fatigue, change of target variable to happiness or health scores, and shift of focus from freedom to make life’s choices to social support and generosity, and the other factors which performed poorly when used to determine the Happiness Index in Singapore. 

## Introduction
### Business Problem Statement
Singapore is internationally recognized for its booming economy. We have amongst the world’s highest GDP per capita, healthy life expectancy, and integrity in government and businesses. Furthermore, according to the Programme for International Assessment (PISA), we also deliver one of the world’s best education systems. Yet, Singapore is only ranked 31st in terms of happiness according to the World Happiness Report (WHR) 2020. The top spots were secured by the Nordic countries, with Finland taking 1st place. 

<p align="center"><img src="https://user-images.githubusercontent.com/45563371/115279662-9225d600-a179-11eb-9b2e-4647d5337bd4.png" /></p>

In Singapore today, the government has extended various sorts of financial aid to help people suffering from poverty meet their daily needs for food, shelter, and education. These factors form the basis of happiness according to Maslow’s hierarchy of needs as shown above (Dr. Saul McLeod, 2009). Despite these government interventions, it seems that general happiness has not increased.

Out of the six factors that contributed to the Happiness Index score, Singapore ranked 1st and 2nd in GDP per capita, healthy life expectancy, and Perception of integrity in society. However, we are only ranked 14th in freedom to make life choices which definitely can be improved. 

<p align="center"><img src="https://user-images.githubusercontent.com/45563371/115279830-c5686500-a179-11eb-97ca-1dd95a5b386b.png" /></p>

The freedom to make life’s choices can be linked to a concept known as financial well-being. According to the Consumer Financial Protection Bureau (CFPB), financial well-being is defined as a state of being wherein a person can fully meet their financial obligations, can feel secure in their financial future, and can make choices that allow them to enjoy life (and thus be happy). 

A recent study by the University of Purdue (Andrew T. Jebb, Louis Tay, Ed Diener, Shigehiro Oishi, 2018) also supports the fact that happiness is impacted by financial well-being, beyond just income level and basic day-to-day living expenses. By improving a person’s financial well-being, they will be able to have greater freedom to make life choices, and hence their happiness. 

Therefore, it becomes critical that we can identify people who do not have this financial freedom and are hence unhappy, yet remain undetected by current measures for financial aid from the Singapore Government.

As analytics consultants to the Ministry of Social and Family Development (MSF)/Community Care Endowment Fund (ComCare), our team aims to study the Financial Well-Being Survey dataset to identify the people who are struggling to obtain financial well-being. This allows us to assist policymakers in easier identification of people who are unhappy and highlight potential reasons behind their struggles.

### Significance of the Business Problem 
Overall happiness is a subjective measure that is affected by a myriad of factors, thus it would be unrealistic to tackle the whole nationwide population of unhappiness. This is why we have decided to use financial well-being as a proxy for happiness as this would mean that our target group of people’s level of happiness can be partially fulfilled by financial aid. 

Studies have shown that poor financial well-being can adversely impact one’s physical, mental, and social health which can lead to other negative impacts such as poorer job performance, lower productivity, and absenteeism, all of which could lead to unhappiness (Human Resources Director). The OCBC Financial Wellness Index (OCBC, 2020), which is a measurement of Singapore’s financial wellness, has dropped from 63 in 2019 to 61 in 2020, especially due to the COVID-19 pandemic. With the current pandemic, more people are likely to have poor financial well-being which may result in decreased happiness levels. 

Given that Singapore’s main resource is its population, the government aims to bridge the income gap to ensure that all Singaporeans are given equal opportunities. The improvement of financial well-being will not only improve these people’s happiness but also their productivity and health. 

Therefore, identifying these people with poor financial well-being will allow the government to more efficiently allocate resources such as money, time and effort, towards those who require financial aid the most to achieve greater happiness. Thus, we need a systematic approach to identify these people through machine learning and artificial intelligence techniques. 

### Expected Business Outcome
Through the machine learning models developed by our team, we hope to improve the financial well-being and happiness of individuals in Singapore. This can be done by highlighting individuals that have low financial well-being so that more attention can be given to them, by better adjusting policies and budgeting to make them happier. Additionally, by identifying the underlying causes of their poor financial well-being, we can help to alleviate their pain points and concerns by recommending them for specialized programs to help them get back on their feet.
