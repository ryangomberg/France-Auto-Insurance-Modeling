# French Auto Insurance GLM Analysis
* Comparative actuarial pricing analysis using Frequency x Severity and Tweedie GLMs *

This project develops and compares generalized linear models (GLMs) for automobile insurance pricing using an annual portfolio of 650,000+ policies from France. Poisson and Gamma GLMs were used to construct a joint model used to estimate pure premium, while a Tweedie GLM was fitted to estimate it directly. The coefficient estimates obtained from each candidate GLM were used to compute and compare relativities as well as developing rating tables. Model performance was evaluated using residual diagnostics, predictive accuracy, and risk segmentation metrics. 


## Technologies
- Microsoft Excel 2021
- PowerQuery, often located in the Microsoft Excel ribbon
- RStudio, version 2024.9.0.375

All code is ran using R-Studio. Be sure to install the relevant packages (see Code --> Date Overview and Preprocessing) before proceeding. 

Additionally, the dataset is installable through the link: https://drive.google.com/file/d/18VEg4Zn8HShVT0AOg3by3_D31AjKTKGM/view?usp=sharing. Make sure the .csv file is in the same folder as the .R or .qmd file used to run the code blocks.

Note that results may slightly vary due to a random train/test split.
