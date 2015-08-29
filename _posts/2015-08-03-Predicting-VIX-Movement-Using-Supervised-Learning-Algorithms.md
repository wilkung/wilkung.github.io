---
layout: post
title: YouTube Video Recommendation via Sentiment Analysis
---

I use various supervised learning algorithms to predict the short term movement of VIX, the implied volatility of the S&P500 based on market prices of options on the S&P 500.  

Having an edge in predicting VIX would allow profitable trading of VIX futures, and perhaps to better hedge equity portfolios.

The features used included: change in closing prices and volume of:
–  S&P 500􏰄􏰄
–  VIX
–  Treasury Yields: 13 week, 5, 10, 30 Year 
–  Oil
–  Gold
–  U.S. Dollar Index
-  Garmin Klass Volatility

The data used was from January 1, 2010 to present. Models were trained on a rolling basis and test on the next day's data.

I did not include precision recall analysis as I assumed a correct prediction up or down were equally helpful and an incorrect prediction up or down were equally bad.  

Among the various algorithms used (KNN, Logistic regression, Gaussian Naive Bayes, SVM, Decision Trees, Random Forest, and Gradient Boosting), KNN and Random Forest seemed to perform the best, especially with short window training.  Accuracy decreased as the training window increased.

The optimal K for the KNN algorithm turned out to be 4.




