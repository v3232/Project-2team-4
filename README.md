# Project-2team-4
## Machine Learning-Based Crypto Market Prediction

### Scope 

Scope of this project is to investigate whether machine learning models can effectively predict 'Trendy' or 'Sideway' states in the cryptocurrency market, specifically the Bitcoin market.

We aim to provide a data-driven approach to support trading decisions, focusing on various technical indicators like ADX, RSI, EMA and Bollinger Bands.


### Utility of our model 

Traders know different market conditions often favor different trading strategies.

1. For Treny Market:

*   Momentum Trading: Traders aim to catch stocks or cryptos in the act of accelerating, buying high   and selling higher. 
*   Breakout Trading: In a trendy market, levels of support and resistance are often tested. A breakout strategy involves entering a position as the asset breaks through these levels, anticipating that the trend will continue.

2.  For Sideway Market:

*   Mean Reversion: In a sideways market, prices tend to revert to the mean or average level. Traders aim to buy low and sell high within the range.


### Data Preparation

*   Data Source: Historical daily price data for Bitcoin from 2010 to 2023.
*   Technical Indicators Used:          
        1.Average Directional Index (ADX)
        2.Relative Strength Index (RSI)
        3.Bollinger Bands
        4.Exponential Moving Average (EMA)
*   Feature Scaling: Used Standard Scaler to normalize all the feature values.
*   Data Splitting: Data is divided into training, testing, and validation sets.
*   Model Training: SVM, GB, RF, LG, LSTM, NN

### Lables assigned using technical indicators 

![lables](/Plots/labelplot.png)

### Various machine learning models used for the projects with classification , backtesting reports and plots 

### Machine Learnings Models Used 

* Support Vector Machine 
* Gradient Boosting 
* Random Forest 
* LSTM 
* Neural Networks 


#### SVM Model 

##### Test Set Report 

![svm_report](/Plots/SVM_report.png)

##### Validation Report 

![svm_report](/Plots/SVM_validation.png)

##### Backtesting Plot 

![svm_report](/Plots/SVM_validation_plot.png)

#### Gradient Boosting  Model 

##### Test Set Report 

![gb_report](/Plots/GB_report.png)

##### Validation Report 

![gb_report](/Plots/GB_validation.png)

##### Backtesting Plot 

![gb_report](/Plots/GB_validation_plot.png)

#### Logistics Regression Model 

##### Test Set Report 

![lg_report](/Plots/LR_report.png)

##### Validation Report 

![lg_report](/Plots/LG_validation.png)

##### Backtesting Plot 

![lg_report](/Plots/LG_validation_plot.png)


#### Random Forest Model 

##### Test Set Report 

![rf_report](/Plots/RF_report.png)

##### Validation Report 

![rf_report](/Plots/RF_validation.png)

##### Backtesting Plot 

![rf_report](/Plots/RF_validation_plot.png)

#### LSTM Model 

##### Test Set Report 

![lstm_report](/Plots/LSTM_report%20.png)

##### Validation Report 

![lstm_report](/Plots/LSTM_validation.png)

##### Backtesting Plot 

![lstm_report](/Plots/LSTM_validation_plot.png)

#### Neural Networks Model 

##### Test Set Report 

![nn_report](/Plots/NN_report.png)


##### Validation Report 

![nn_report](/Plots/NN_validation.png)

##### Backtesting Plot 

![nn_report](/Plots/NN_validation_plot.png)


### Challenges faced 


1. Labelling:

In the context of predicting market labels, labeling the data was a critical step. The challenge there was determining which technical indicators were most relevant for predicting market behavior accurately.
Extensive research was needed to understand and select the appropriate technical indicators. In our case, we chose to use indicators like Average Directional Index (ADX), Relative Strength Index (RSI), Bollinger Bands, and Exponential Moving Average (EMA).


2. Backtesting:

Backtesting is an essential component of developing a trading or market prediction model. It involves testing the model's performance on historical data to assess its effectiveness. The challenge we faced was that the standard train-test split function randomly selected data for the training and testing sets, which was not suitable for backtesting. Backtesting required data to be arranged in chronological order to simulate real-world trading scenarios.To overcome this challenge, we created a separate validation set that maintained the sequential order of data, enabling us to assess the model's performance realistically in a historical context.

3. Optimizing the Model:

Model optimization was crucial for improving the accuracy and generalization of the ML models. This process often involved experimenting with various model and training techniques.One aspect of model optimization was tweaking the neural network architecture (Used in LSTM model aswell). This includes adding and removing layers, adjusting the number of neurons in each layer, changing activation functions and incorporating regularization techniques. Optimization also involved fine-tuning hyperparameters like learning rates, batch sizes, and dropout rates to achieve the best performance.


4. AWS SageMaker:

AWS SageMaker is a powerful platform for developing and deploying machine learning models. However, we faced a challenge related to finding a free API that provided all the required features in the dataset for training and for implementing a chatbot using SageMaker.This issue arose because some financial data sources or APIs charged for access to real-time or historical market data, and a free alternative might not have covered all the necessary data points.

In summary, we encountered these challenges while implementing our project for market prediction, and addressing them required careful consideration and problem-solving to develop an accurate and effective predictive model for financial markets.




