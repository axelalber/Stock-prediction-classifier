# Stock prediction classifier
 Simple stock prediction using Random Forest classifier

 This project was inpsired by Dataquest.

 In this project I'm doing the whole machine learning pipeline. Starting with collecting data from Yahoo finance, then some feature engineering on that.

 Then I create a simple train test split function and a custom grid search function to verify models. Then I'm using cross validation to tune the hyperparameters of the different models.

 From there, I chose the model that had the best results, and trained the model. Then i veryfied it with the test data. The goal was to beat the baseline and it did.

 One way to increase the precision (that was my main goal) was to use a custom threshold for the model to predict 1 (that the stock would go upp the next trading day). With having the threshold at 0.55 I reached a precision of around 68% compared to baseline at 54%. With a custom threshold the model predicts more zeroes, but that is not an issue since we want the model to be sure when it's predicting a 1.

 I tried this model on S&P 500 stocks one day and got a precision of around 70% compared to the 65% of stocks that actually went up the next day.