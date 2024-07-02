# Next Basket Recommendation with Basket Size Prediction

A next basket recommendation model that incorporates basket size prediction, named **NBR-WBS** (**N**ext **B**asket **R**ecommendation **w**ith **B**asket **S**ize).

# Description

* The embedding module includes a basket encoder using attention mechanisms for item importance and a basket-size encoder using Long Short-Term Memory (LSTM) for basket size embeddings.
* The basket preference module combines basket and size embeddings, processed by a shared Transformer for multi-task learning to generate the final state vector.
* The prediction module utilizes the final state vector of baskets for two tasks: predicting basket items and sizes using separate predictors. The results from these predictors are then combined to provide users with dynamically sized basket recommendations.

# Datasets

* [Ta Feng](https://www.kaggle.com/datasets/chiranjivdas09/ta-feng-grocery-dataset)
* [Dunnhumby](https://www.kaggle.com/datasets/frtgnn/dunnhumby-the-complete-journey)
* [Instacart](https://www.kaggle.com/c/instacart-market-basket-analysis/data)

# Contributions

* To the best of our knowledge, this study is the first to take into account basket size dynamically in the next basket recommendation.
* The proposed NBR-WBS model serves as a framework for multi-task learning. It not only forecasts the probability of items within the baskets but also predicts the size of users' baskets at different time points.
* Extensive experiments were conducted on three real datasets, demonstrating that the proposed NBR-WBS model outperforms existing methods.


