# QSS45 Final Project: Effect of NHL Game Outcome on Fan Sentiment on Social Media

## Description

This project focuses on analyzing and modeling the sentiment of hockey-related social media posts to uncover insights about fan behavior, sentiment trends, and game outcomes. 

### Executing program

#### Pre-processing
Begin by running ```cleaning.ipynb``` to clean/pre-process the data. The file takes in two csv files, one containing all social media posts to do with the NHL and one containing game statistics for all NHL teams.
The program does the following:
* Filters and preprocesses hockey-related posts within a specific time frame and language
* Matches posts to hockey games based on team mentions and game details
* Extracts and classifies fan sentiment based on post content
* Calculates additional insights, including game outcome, scoring details, and team performance metrics

Outputs:
* a cleaned dataset ```hockey_cleaned.csv``` 

#### Sentiment Analysis
Performs sentiment analysis on a dataset of hockey-related social media posts. It uses a pre-trained BERT model to classify the sentiment of each post, generating an output dataset with sentiment labels. Begin by inputting the ```hockey_cleaned.csv``` dataset.

The program does the following:
* Processes a dataset of hockey-related posts
* Truncates text to fit within the model's input length
* Classifies each post's sentiment using a pre-trained transformer model

Outputs:
* a dataset ```hockey_sentiment.csv``` with sentiment labels

#### Statistical Analysis
Performs statistical analysis and machine learning modeling on a dataset of hockey-related social media sentiment. Begin by inputting the ```hockey_sentiment.csv``` dataset.

The program does the following:
* Visualizes overall sentiment distribution and sentiment based on game outcome
* Calculates and compares proportions of positive and negative sentiments for winning and losing posts
* Generates heatmaps for sentiment proportions
* Performs Z-tests to determine the significance of sentiment differences
* Builds predictive models using OLS regression and XGBoost
* Evaluates model performance with metrics like Mean Squared Error (MSE) and R-squared values
* Visualizes feature importance using XGBoost and SHAP

## Authors

Kevin Guo
