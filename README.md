# French Auto Insurance GLM Analysis
*Comparative actuarial pricing analysis using Frequency x Severity and Tweedie GLMs*

## Project Overview
This project develops and compares generalized linear models (GLMs) for automobile insurance pricing using an annual portfolio of 650,000+ policies from France. Poisson and Gamma GLMs were used to construct a joint model used to estimate pure premium, while a Tweedie GLM was fitted to estimate it directly. The coefficient estimates obtained from each candidate GLM were used to compute and compare relativities as well as developing rating tables. Model performance was evaluated using residual diagnostics, predictive accuracy, and risk segmentation metrics. 

## Primary Objectives
* Clean and preprocess an extensive insurance portfolio
* Explore relationships between rating factors and claim frequency and severity
* Build Frequency x Severity and Tweedie pricing models
* Compare predictive performance on an in-sample validation set
* Evaluate risk inequality using Lift Charts, Ordered Lorenz Curves, and Gini coefficients

## Methods

### Preprocessing
* Joined and cleaned claim frequency and severity data
* Processed and handled missing values for 650,000+ policies
* Engineered categorical rating factors
* Prepare GLM analysis with a training (80%) and test (20%) set
### Models
* Poisson GLM, Exposure offset (Claim Frequency)
* Negative Binomial GLM, Exposure offset (Claim Frequency)
* Gamma GLM (Claim Severity)
* Frequency x Severity (Pure Premium)
* Tweedie GLM, Exposure weight (Pure Premium)
### Model Evaluation
* AIC/BIC
* Log-likelihood
* Pearson chi-squared
* Deviance
* Pearson Dispersion
* Residual diagnostics (Residual vs. fitted, QQ-plot, Residual distribution)
* Lift Charts
* Ordered Lorenz Curves
* Gini Coefficients
* Test set: MAE, WMAE, RMSE

## Notable Results
* The candidate models for measuring average pure premiums, Frequency × Severity and Tweedie, displayed comparable performance on the test data, with slight differences in the performance metrics.
* Residual diagnostics, lift charts, and ordered Lorenz curves consistently proved similar the ability to measure risk inequality between policies, even though the Tweedie model had a slightly higher Gini coefficient, thereby suggesting a modest increase in risk differentiation.
* BonusMalus is a very significant rating factor in identifying patterns in claim frequency and severity.
* Each of the two candidate models has an advantage in pricing. The Frequency × Severity model allows us to gather more information about the impact of rating factors on claim frequency and severity, whereas the Tweedie distribution only requires the construction of a single model for measuring the average pure premium



## Technologies
### Software
* Microsoft Excel 2021
* PowerQuery, often located in the Microsoft Excel ribbon
* RStudio, version 2024.9.0.375
### R Libraries/Packages


All code is ran using R-Studio. Be sure to install the relevant packages (see Code --> Date Overview and Preprocessing) before proceeding. 

Additionally, the dataset is installable through the link: https://drive.google.com/file/d/18VEg4Zn8HShVT0AOg3by3_D31AjKTKGM/view?usp=sharing. Make sure the .csv file is in the same folder as the .R or .qmd file used to run the code blocks.

Note that results may slightly vary due to a random train/test split.
