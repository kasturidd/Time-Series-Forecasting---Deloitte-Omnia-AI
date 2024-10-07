# Time-Series-Forecasting---Deloitte-Omnia-AI
Cortex AI aims to empower Deloitte by leveraging AI and data to enhance client solutions. The project focuses on compiling reputable public and private data sources to create curated industry-specific datasets. It also identifies and develops algorithms for these datasets, with documented use cases to ensure value.



## Use Case Descriptions for CortexAI Platform
### 1.1 Use Case: Recession
This use case aims to forecast recession indicators based on economic activities in Canada. Leveraging datasets from the Canadian government and the Organization for Economic Cooperation and Development (OECD), the analysis identifies various factors influencing recessions, such as the Consumer Price Index (CPI), Toronto Stock Exchange (TSX), employment changes, treasury bonds, unemployment rate, GDP, industrial production rate, and overnight interest rate. The findings reveal that while the unemployment rate has a direct proportional relationship with recession, other indicators like CPI and TSX exhibit inverse relationships. The need for a recession forecasting model is underscored by economic uncertainties in the post-lockdown environment.

### Findings
Key Indicators: Unemployment rate, CPI, TSX, employment changes, treasury bonds, and GDP.
Relationships: Unemployment rate is directly proportional to recession; other indicators (CPI, TSX, etc.) are inversely proportional.
Forecasting Model: A hybrid approach utilizing both long-term (10-year treasury bond) and short-term (2-year treasury bond and overnight interest rates) data is essential for accurate predictions.
### Methodologies Used
Dataset Research: Valid datasets obtained from governmental and reputable financial sources.
Formulating Use Case: Identified the impact of economic factors on recession using relevant datasets.
Data Pre-processing: Cleaning, concatenation, and transformation of datasets, including normalization of values.
Develop Algorithm and Model: Explored various supervised learning models (Decision Tree, Random Forest, etc.) with Random Forest yielding the best results using the SMOTE technique for class imbalance.

## 1.2 Use Case: CPI Forecasting
This use case focuses on forecasting inflation through the Consumer Price Index (CPI) and its components. Traditional inflation models typically predict overall inflation, but this use case emphasizes the benefits of granular inflation forecasting, utilizing time series models like VAR and ARIMAX.

### Findings
Sectoral Insights: Granular inflation predictions can aid government and fiscal authorities in adjusting policies, helping investors and firms mitigate risks.

### Methodologies Used
Dataset Research: Compiled CPI datasets from Stats Canada, including various components like food, shelter, and transportation.
Data Preprocessing: Applied statistical tests (e.g., Granger’s causality) to ensure data validity and stationarity.
Develop Algorithm and Model: Employed VAR and ARIMAX models to predict inflation, with ARIMAX demonstrating superior accuracy.

## 1.3 Use Case: Housing Prices
The prediction of housing prices using the New Housing Price Index (NHPI) examines factors influencing real estate values in Canada.

### Findings
Key Variables: The model includes various credit products and TSX values, highlighting their impact on housing prices.
### Methodologies Used
Dataset Research: Gathered data from Government of Canada, CMHC, and Yahoo Finance.
Data Preprocessing: Cleaned and aligned datasets to facilitate multivariate time series analysis.


## 1.4 Use Case: Oil Prices
This use case predicts oil prices using both univariate and multivariate time series approaches, leveraging datasets from the Government of Canada and other financial sources.

### Methodologies Used
Dataset Research: Historical crude oil price indexes were used, focusing on Western Canada Select crude oil prices.
Data Preprocessing: Addressed missing values and standardized the dataset for analysis.
### Model Development
Univariate Model: Auto ARIMA and Moving Average Linear Regression were utilized, with the latter achieving a 93.42% accuracy on the test set.
Multivariate Model: Linear Regression with Bayesian penalties yielded the best predictive performance.
