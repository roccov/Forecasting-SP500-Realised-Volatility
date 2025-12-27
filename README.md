

# Learning from Missingness: Enhancing imputation with the NN3 architecture to predict monthly US stock returns


## Highlights: 

- Forecasted one-day-ahead S&P 500 realized volatility using econometric (GARCH, EGARCH), machine-learning (Elastic Net, XGBoost, LSTM), and hybrid models

- Constructed a rich feature set combining high-frequency realized volatility measures, implied volatility (VIX), market microstructure indicators, momentum and distributional features, and macro–financial variables

- Implemented a strict walk-forward rolling-window evaluation protocol, ensuring fully out-of-sample and real-time forecasting comparability across models

- Demonstrated that XGBoost delivers the strongest predictive performance, particularly during volatility spikes, by learning nonlinear and regime-dependent interactions rather than relying on new predictors

- Provided interpretability through SHAP values, revealing how nonlinear interaction effects explain performance differences between linear and nonlinear models

- Found no performance gains from hybrid ML–EGARCH specifications, indicating that machine-learning models internalize volatility persistence and asymmetry when the information set is sufficiently rich



## Repository Structure:

00_Report : 

01_Data_Downloading_Merging : Data Acquisition and Merging

02_Features_Engineering : Feature Engineering and Variable Construction

03_GARCH_EGARCH : GARCH and EGARCH Volatility Models

04_ElasticNet : Elastic Net Regression for Volatility Forecasting + Building EGARCH features

05_XGBoost : XGBoost Nonlinear Volatility Forecasting

06_LSTM : LSTM-Based Volatility Forecasting

07_ML_Plot : Machine learning performance visualisation


## Running the NN3 code:

To run the code, make sure the data file is inside of the folder. CHange the parameters as you wish in the config.py file.

Then, Simply execute the main.py file in the terminal.

## Collaborators: 
This project was carried out as part of the Machine Learning for Finance course taught by Professor Semyon Malamud at the Ecole Polytechnique Fédérale de Lausanne (EPFL), in collaboration with:

Rocco Pio Lorenzo Ventruto [https://github.com/roccov]

Tallula Graber [https://github.com/Tallulaa]

Noah Louis Truttmann [https://github.com/NoahTruttmann]

Piotr Kleymenov [https://github.com/PiotrKley259]

This repository is a personal, cleaned-up version of the original group project, with additional comments and refinements for portfolio purposes.
