# Sujay Talanki's Portfolio

## Movie Recommender System
* Engineered a content-based recommender system using NLP that takes in a movie and recommends 10 similar movies based on movie attributes and rating
* Considered movies' description, cast, director, genre, and average rating to suggest movies that the user would enjoy
* Conducted preprocessing and feature engineering to ensure data quality and enhance model performance
* Employed CountVectorizer and cosine similarity metric to suggest many similar movies. Retrieved the top 10 highest rated movies from this selection
  to suggest to the user
* Utilized Python pandas, nltk, sklearn

## Top 10 Property Essentials
* Background: The company had many properties, each of which had 10 areas that inspectors were required to assess; inspectors left comments regarding the condition of each area
* Result: Produced a Power BI dashboard that allows business analysts to extract information from 5,000+ inspectors’ comments regarding the condition of 5,000+ 
  properties. 
* Leveraged Python (pandas, nltk, sentence_transformers, sklearn), Snowflake (SQL), Power Query, and Power BI to create a pipeline that produced
  meaningful conclusions from raw text data
* Implemented a key phrase extraction feature, sentiment analysis classifier (NLP), and Power BI visualizations to analyze
  comments on an aggregate level according to user-selected attributes
* Analysts could filter the results based on the market, region, property type, property manager, etc. in order to visualize the performance
  of select facilities

## Operating Expense (OpEx) Variance Analysis
* Background: The company had budgets for each operational expense (OpEx). If the actual expense for the quarter missed the budget, an accountant would leave a comment for the reason behind the
  "variance" (budget miss). I was tasked with categorizing the general reasons behind these variances.
* Result: Applied unsupervised learning algorithms (NLP) to create 10 evenly distributed categories that classified 20,000+ OpEx variance comments. This project allowed accountants and analysts
  to understand/analyze the reasons behind OpEx variances to prevent occurances in the future!
* Reduced workload by ~ 60% and achieved ~ 80% accuracy on hold-out set
* Developed a python pipeline (pandas, nltk, sentence_transformers, sklearn) that embedded sentences into vectors (BERT LLM) and utilized K-Means clustering to categorize OpEx variance comments
* Launched a local app (python: plotly and dash) to visualize the key phrases per category. This was used to help analysts summarize the content of the 20,000+ comments.

## Flight Delays Prediction
* Pioneered a machine learning pipeline to predict the severity of a flight’s delay (1M+ flights)
* Performted EDA, feature engineering, cross validation, and hyperparameter tuning (GridSearchCV) to optimize a LightGBM model that achieved 95%
* Tools: Python (numpy, pandas, sklearn, LightGBM, XGBoost, GridSearchCV)

## Netflix Stock Price Prediction
* Assembled an LSTM Neural Network to predict the closing price of Netflix stock using the last 60 days of time series data
* LSTM Neural Network contained 3 LSTM layers of size 50 neurons, followed by 3 drouput layers (20%) and 1 dense layer
* Adjusting the batch size to 32 and training for 50 epochs resulted in the best performance (~ 4.5 RMSE)

## Lead Scoring Model
* Developed a lead scoring model with PyCaret to predict the probability that a loan ("lead") is funded with 97% accuracy
* Led to a profit of ~ $333,000 (in our scenario, assuming a converted lead yields $120 and the time/effort costs around $15)

* 
