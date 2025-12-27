# Forecasting S&P 500 Realized Volatility

## Highlights: 

- Forecasted one-day-ahead S&P 500 realized volatility using econometric (GARCH, EGARCH), machine-learning (Elastic Net, XGBoost, LSTM), and hybrid models

- Constructed a rich feature set combining high-frequency realized volatility measures, implied volatility (VIX), market microstructure indicators, momentum and distributional features, and macro–financial variables

- Implemented a strict walk-forward rolling-window evaluation protocol, ensuring fully out-of-sample and real-time forecasting comparability across models

- XGBoost delivers the strongest predictive performance, particularly during volatility spikes, by exploiting nonlinear and state-dependent transformations of highly persistent volatility signals rather than by discovering new dominant predictors

- Provided interpretability through SHAP values, revealing how nonlinear interaction effects explain performance differences between linear and nonlinear models

- Found no performance gains from hybrid ML–EGARCH specifications, indicating that machine-learning models internalize volatility persistence and asymmetry when the information set is sufficiently rich



## Repository Structure:

00_Report : Academic Report

01_Data_Downloading_Merging : Data Acquisition and Merging

02_Features_Engineering : Feature Engineering and Variable Construction

03_GARCH_EGARCH : GARCH and EGARCH Volatility Models

04_ElasticNet : Elastic Net Regression for Volatility Forecasting + Building EGARCH features

05_XGBoost : XGBoost Nonlinear Volatility Forecasting

06_LSTM : LSTM-Based Volatility Forecasting

07_ML_Plot : Machine learning performance visualisation

08_Data : Datasets Used, All data can be downloaded automatically by running the code, except the Oxford–Man Institute Realized Volatility Indices, which were downloaded manually due to access restrictions.

09_Presentation : Video presentation of the project


## Running the code:

The full analysis can be reproduced by executing the notebooks in the numerical order indicated by their folder names.

