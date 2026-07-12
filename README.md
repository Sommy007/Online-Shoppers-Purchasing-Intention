# Project Overview  
This project aims to develop and evaluate machine learning classification algorithms to predict online shoppers' purchasing intention (whether a session ends in a transaction or not) based on real-time web browsing behavior and session attributes. The dataset consists of 12,330 clickstream sessions gathered over a one-year period, representing unique users to eliminate bias from specific marketing campaigns, holiday periods, or user profiles.

The dataset contains 12,330 observations and 18 variables (17 predictor variables and 1 target variable) with no missing values. The features are composed of 10 numerical and 8 categorical attributes. The predictor variables encompass page-view metrics and session durations across three primary page types (Administrative, Informational, and Product Related), core Google Analytics metrics (Bounce Rates, Exit Rates, and Page Values), temporal markers (Month, Weekend indicator, and closeness to a Special Day), and user environment details (Operating System, Browser, Region, Traffic Type, and Visitor Type). 

The primary objective of this project is to analyze the data, identify patterns, and compare the performance of different classification algorithms to identify the model that most accurately predicts purchasing intent in real time based on behavioral and web analytics characteristics. Accurately predicting buyer intent allows e-commerce platforms to deploy automated, dynamic intervention strategies such as personalized discounts, trust badges, or simplified checkout flows to capture high-intent users before they abandon their sessions. Furthermore, this study demonstrates the application of predictive analytics to maximize conversion rates, optimize user experience, and drive digital retail revenue.

## Project Goal
This project aims to use supervised machine learning (binary classification) to predict the Revenue outcome (whether a session ends in a purchase or not) of online shoppers using real-time behavioral features, session metrics, and web analytics indicators.

## Variables
Target (Output): Revenue  
Features (Input): Administrative, Administrative_Duration, Informational, Informational_Duration, ProductRelated, ProductRelated_Duration, BounceRates, ExitRates, PageValues, SpecialDay, Month, OperatingSystems, Browser, Region, TrafficType, VisitorType, Weekend.

## Data Source
This project uses a publicly available dataset that follows standard academic citation practices.  
Dataset Name: Online Shoppers Purchasing Intention Dataset  
Source: UCI Machine Learning Repository  
Authors: C. O. Sakar and Yomi Kastro  
Year: 2018  
DOI / Reference: https://doi.org/10.24432/C5F88Q

## Methodology
The project follows a structured machine learning workflow:  
* Data Overview/collection
* Data Preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Feature Analysis
* Model Selection and Evaluation

## Key Findings
* Customers are likely to shop during the workday than during the weekend. Purchases are highly seasonal, with the highest revenue occuring in November, suggesting a strong end-of-year shopping effect. May also shows high visitor activity, but with a lower purchase conversion compared to November.
* Returning visitors accounts for most purchases, showing a stronger tendency to convert compared to the new visitors. This highlights the importance of customer retention in increasing online shopping revenue.
* Business appears to depend heavily on few traffic channels and a few geographic markets to generate revenue. Marketing efforts should prioritize optimizing the highest-performing traffic sources while exloring opportunities to grow customer engagement in underrepresented regions.
* Browser2 and Operating system 2 represent the primary platforms through which customers access the website, contributing the largest share of both visitor sessions and purchases. This implies that optimiziing the website for these platforms could enhance user experience, improve customer satisfaction, and support higher conversion rate.
* While product page views and sessions duration strongly predict conversion, a distinct segment of highly engaged, non-converting users exists as extreme outliers. Addressing user friction within these prolonged, non-converting sessions represents our highest-leverage opportunity to unlock bottlenecked funnel velocity and capture unrealized revenue.
* The value of the page customers visited strongly deterrmine whether they end up shopping online.
* There is a strong, linear positive correlation between Bounce and exit rates. From the data analysis, keeping both rates strictly below 5% is a mandatory prerequisite for conversion.
* Informational pages are necessary for customer trust, but dragging users deep into informational content correlates with lower conversion rates. Also, visiting administrative pages is necessary to complete a purchase, but excessive time spent on them is a major indicator of checkout friction.
* Proximity to a holiday causers a surge in window-shopping, which dilutes the overall conversion rate.

## Tech Stack
Programming Language: Python  
Libraries: NumPy, Pandas, Matplotlib, Seaborn  
Machine Learning: Scikit-Learn  
Model Used: Logistic Regression, RandomForest, K-Nearest Neighbors (KNN) Classifier  
Environment: Jupyter Notebook
