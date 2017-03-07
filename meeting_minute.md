# Group Meeting Minute

## Meeting #1 - Feb 27

1. Discussed the details about the three potential topic ideas

   - In all the problems, how to do feature engineering and selection

2. Investigation on LSTM and Antoencoder (by Mar 3)
3. Next meet at Mar 4/5th

## Meeting #2 - Mar 5

###Project final decision:

* The topic of the project lies in the stock screening strategy achieving active return. We will construct a portfolio with stocks and value the excess return of our portfolio relative to the benchmark index. In addition to the loss computation in the regular machine learning, we will also evaluate the portfolio excess return, which makes our model more applicable. The portfolio is rebalanced in certain period (1 week, 2 week, or 1 month etc.), the dataset comes from the beginning time *t* of each period, which is:
```
   - X: (num_stocks * num_features) 
        Stock historical data, including market data and fundamental data at time *t*
   - y: (num_stocks * 1) 
        Stock return in the period (ClosePrice_(t) - ClosePrice_(t-1))/ClosePrice(t-1)
 ```
* Building the prediction model (Feature selection)
   - To begin with, we will implement a stock selection strategy by SVM as a baseline. 
   - Secondly, we will research on kernelized SVM for potential improvement. Regularization will be carefully designed to avoid overfitting.
   - Also, we consider Neural Network as an alternative of SVM in the learning process.

* A further step is to investigate on the feature space. 
   - We propose to experiment with dimension reduction methods. 
   - Tranditional method such as PCA will be employed on the design matrix *X* before we go to the next step of SVM/Neural Network. 
   - Another method that has caught our interests is Autoencoder. 
   - *If time permits*, we will compare with some given features from existing models, such as the Fama/French 5-factor model and the Multiple-Factor Model from BARRA. 

  
