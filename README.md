# DataChallengeXINF554
A data challenge course work for INF554 "Machine/Deep Learning" Course

## Team (ID: Hawks):
    - Imad Eddine MAROUF, KaggleID: @maroufimad
    - Anton EMELCHENKOV, KaggleID: @antonemelchenkov
    - Ali KESHAVARZI, KaggleID: @ali2066

### Required Libraries:
- Create a new conda environement using "Hawks_env.yml"

## Exploratory Data Analysis:
We provided a notebook, with insights about the dataset provided, most useful features 

## Features Selection/Generation:
- Notebook provided to see the correlation, the range, variance of each numerical feature extracted.
- Features Notebook: to generate more categorical, numerical features.

## Models:
- **Logistic Regression:** using only standard features
- **XGBoost Regressor:** using numerical features 
- **DistilledBERT Model:** Regression using distilledBERT model
- **BERT with XGBoost:** Using BERT for binary classification (tweet get 0/not-zero retweet), then we apply regression on tweets classified as non-retweet by BERT.
- **NNsforRegression:** Trying different neural network architecutre for regression.
- **CarRegressor_XGBoost_NeuralNets:** We ensembled all the three models, using the generated features (48 features) in order to improve the accuracy.
- **LogisitcRegression_with_XGBoost:**: We ensembled all the two models.
- **NN with Tfidf vectorizer:** with used Tfidf embeddings as input for NN of 4 layers.
- **LSTMs:*** using only text features
- **LSTMs with Logistic Regressor:** using only text features for LSTMs, then we average the output of Logisitc Regressor with results from LSTM.
- **CarRegressor_XGBoost_NeuralNets:** It contains the three models trained on 13 numerical features generated from test. NeuralNet score is our best score (MAE: 154.44057)


## Usage:
- Dataset is not provided, it should be saved within the same folder as the notebooks.
- Pre-trained model named: "NN_BestNumFeatures20_epochs_143.pt" to prevent re-training, just need be upload in CarRegressor_XGBoost_NeuralNets notebook and it will be ready to go.



