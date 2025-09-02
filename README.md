# Pricing Optimization with Orange Juice Demand

## Overview
This project analyzes the Dominick’s orange juice dataset to estimate demand, optimize pricing, and understand the impact of promotions. It combines econometric models, machine learning, and causal inference (Double Machine Learning) to provide both predictive and causal insights.

## Objectives
- Estimate own- and cross-price elasticities across brands (Dominick’s, Tropicana, Minute Maid).
- Translate elasticity estimates into markup and pricing recommendations.
- Apply machine learning models (LASSO, Random Forest) to improve demand prediction.
- Use Double Machine Learning (DML) to estimate the causal effect of promotions on sales.

## Methods
- **Econometrics:** OLS regression with interactions, elasticity matrix construction, markup guidance.
- **Machine Learning:**
  - LASSO with cross-validation for variable selection.
  - Random Forest for nonlinear prediction.
- **Causal Inference:**
  - Double Machine Learning (Chernozhukov et al.) with sample splitting, cross-fitting, and orthogonalized moment conditions.
  - Treatment effect of promotions on sales.

## Key Insights
- Elasticities: Tropicana generally more elastic than Minute Maid, implying different markup strategies.
- Predictive performance: Random Forest improves accuracy compared to LASSO and OLS.
- Causal effect: Promotions significantly increase sales even after controlling flexibly for prices and brand heterogeneity.

## Project Structure
Both the original R Markdown (`.Rmd`) source files and rendered `.html` reports are included.
Open the `.Rmd` files in RStudio and knit them to reproduce results.

## Technologies
- R (tidyverse, glmnet, randomForest, DoubleML)
- Statistical modeling, machine learning, causal inference
