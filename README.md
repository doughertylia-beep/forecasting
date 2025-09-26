***GDP Forecasting Case Study Using ARIMAX Overview***

This project explores the relationship between U.S. Gross Domestic Product (GDP) and two predictor variables:
Residential Building Permits and Consumer Confidence Index (CCI). The analysis applies time series visualization, 
statistical diagnostics, and an ARIMAX (AutoRegressive Integrated Moving Average with Exogenous Variables) model to forecast GDP based on the two predictors.

***Project Structure***
- Data import and preparation
- Exploratory Data Analysis (EDA)
- Plotting time series trends for GDP, Permits, and CCI
- Visualizing GDP seasonal patterns by year and quarter
- Overlaying normalized trends of all three variables for correlation comparison
- Generating ACF and PACF plots for to assess autocorrelation and partial autocorrelation
- First differencing to achieve stationarity before model fitting
- Building an ARIMAX model using differenced CCI and Permits as exogenous predictors
- Performing a stepwise search for the optimal ARIMA order (p, d, q) using AICc minimization
- Comparing actual vs. fitted GDP values
- Assessing model residuals for normality and autocorrelation

**Key Dependencies**
- pip install pandas matplotlib numpy seaborn statsmodels scikit-learn
- pandas	Data manipulation and cleaning
- matplotlib	Data visualization
- seaborn	Enhanced statistical plotting
- statsmodels	Time series modeling and ACF/PACF plotting
- scikit-learn	Model evaluation metrics

***Input Data***
- GDP.csv	U.S. GDP data by quarter (chained 2017 USD)
- Permits.csv	Residential building permits issued per quarter
- CCI.csv	Consumer Confidence Index (1985=100)
