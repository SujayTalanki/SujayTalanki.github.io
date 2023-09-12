# Sujay Talanki's Portfolio

# Movie Recommender System
* Content-based recommender system using NLP that takes in a movie and recommends 10 similar movies based on movie attributes and rating
* Considered movies' description, cast, director, genre, and average rating to suggest movies that the user would enjoy
* Conducted preprocessing and feature engineering to ensure data quality and enhance model performance
* Employed CountVectorizer and cosine similarity metric to suggest many similar movies. Retrieved the top 10 highest rated movies from this selection
  to suggest to the user
* Utilized Python pandas, nltk, sklearn

# Top 10 Property Essentials
* Produced a Power BI dashboard that allows business analysts to extract information from 5,000+ inspectors’ comments regarding the condition of 5,000+ 
  properties. (Each property had 10 areas that inspectors were required to assess; inspectors left comments regarding the condition of each area.)
• Leveraged Python (pandas, nltk, sentence_transformers, sklearn), Snowflake (SQL), Power Query, and Power BI to create a pipeline that produced
  meaningful conclusions from raw text data
• Implemented a key phrase extraction feature, sentiment analysis classifier (NLP), and Power BI visualizations to analyze
  comments on an aggregate level according to user-selected attributes
• Analysts could filter the results based on the market, region, property type, property manager, etc. in order to visualize the performance
  of select facilities

# Operating Expense Variance Analysis

(NLP) Used Key Phrase Extraction (develped in Top 10 Project) and Clustering on submitted OpEx Variance comments to better categorize the reasons for OpEx variance. The new categories give analysts a better insight as to the reasons for OpEx variance. For the Clustering I used sentence transforms to embed comments as high dimensional vectors, and these vectors were entered into the K-Means Algorithm for clustering. The two processes made it easy to infer the meaning of comments without having to scan every comment multiple times (25,000+ comments!)



• Introduced the BERT LLM with K-Means clustering to categorize the reasons that operational expenses missed the proposed
budgets (25,000+ entries). Reduced workload by ~60% and achieved ~80% accuracy
* 


#


