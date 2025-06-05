---
layout: default
title: "Sujay Talanki's Data Science Portfolio"
---
## [LLM-Powered Form Completion Engine](https://github.com/SujayTalanki/LLMFormCompletionEngine)
* Engineered a RAG pipeline using Llama3 8B LLM to automate maintenance request processing via an interactive form completion engine.
* Leveraged GPT-4o to generate synthetic data.
* RAG pipeline employs custom document object, VectorStoreIndex, QueryEngine, and Retriever.
* Tools used: Python (PyTorch, Replicate, OpenAI API, LlamaIndex), Llama3 8b, Mistral 7b.
* **NOTE**: Project isn't complete as the feedback feature hasn't been fully implemented and the Streamlit app code hasn't been fully developed. The real data was removed for privacy reasons.

## [Aerial Object Detection: Differentiating Drones, Birds, and Airplanes](https://github.com/SujayTalanki/DroneDetection)
* Curated a diverse dataset of 2000+ drone, bird, and airplane images/videos from various sources.
* Augmented the dataset with varied lighting conditions, angles, cropping, shear, and background noise to simulate real-world conditions.
* Fine-tuned a YOLOv8 model that achieved 91% precision, 89% recall, and 89% mAP for all classes
* Utilized RayTune to search for optimal hyperparameters and MLflow to track the results for different model configurations
* Validated the model using a test set comprising unseen aerial footage from different environments.
* Tools: Python (Cv2, PyTorch) YOLOv8 (Computer Vision model), Roboflow (Data preprocessing, augmentation, and annotation service)

**Prediction on Test Set Images:**  

![image](https://github.com/user-attachments/assets/883f8ce8-2583-402f-a263-d0d88ac85508)

**Confusion Matrix:**  

![image](https://github.com/user-attachments/assets/8ad546a3-e687-4e60-8f44-93a0471f990e)

**F1 vs. Confidence Curve:**  

![image](https://github.com/user-attachments/assets/588f9542-fe14-47bd-8cfc-2a479791c8e0)

## [Enhancing NanoGPT via Squentropy Loss and Hyperparameter Tuning](https://github.com/sujen07/NanoGPT-Loss-Stop-Analysis)
* [**Report of Findings**](https://github.com/sujen07/NanoGPT-Loss-Stop-Analysis/blob/main/DSC180BFinalReport.pdf), [**Website**](https://akshatm1011.github.io/Optimizing-NanoGPT/), [**Poster**](https://github.com/sujen07/NanoGPT-Loss-Stop-Analysis/blob/main/NanoGPTPoster.pdf)
* Formulated a custom and hybrid squentropy loss function to minimize empirical risk via PyTorch methods
* Developed script to calculate model perplexity (metric that determines how "perplexed" a model is when predicting its next token; lower perplexity indicates better performance)
* Conducted large-scale hyperparameter tuning via distributed data parallel methods to attain 1.8 loss and 3.9 perplexity
  - Hyperparameters tuned include learning rate, dropout rate, and number of layers
* Tools: Python (Numpy, Pytorch, Pickle), AWS

**Poster:**  

![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/a9dc6010-040a-4204-90b7-4530035587c5)

**Formula and Code:**  

![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/cc1a3a78-3ff8-49a5-8668-755d9d001545)


## [Top 10 Property Essentials](https://github.com/SujayTalanki/Top10PropertyEssentials)
* Background: The company had many properties, each of which had 10 areas that inspectors were required to assess; inspectors left comments regarding the condition of each area.
* Result: Designed a Power BI dashboard using Python, Snowflake, and unsupervised learning algorithms to analyze 20,000+ facilities, communicating insights to non-technical stakeholders.
* Applied key phrase extraction, sentiment analysis classifier, and visualizations to uncover insights from 5,000+ inspector comments, enabling data-driven decisions and driving business improvements.
* Analysts can filter the results to analyze performance based on the market, region, property type, property manager, etc. in order to visualize the performance
  of select facilities.
* Tools used: Python (Numpy, Pandas, Nltk, Sentence_transformers, Sklearn), Snowflake (SQL), Power Query, and Power BI.
  
**Workflow Diagrams:**  

  ![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/c9d46a86-27ae-4474-a0b0-4ca1707138a0)
  *Diagram of sentiment encoding process*

  ![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/9a808bbb-8cdf-4a30-ba45-ce4f1dbb5b6d)
  *Diagram of key phrase extraction process*  

**Power BI Dashboard:**  
**NOTE**: I don't have access to the data warehouse anymore, so there is an error when using the Power BI dashboard (PowerBIDashboard.png). However, I have 
  attached an image of what the missing visuals should look like (check App.png)  
  
  ![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/bf054830-bb14-4dab-b42e-d37434779875)
  *Power BI Dashboard with error*

  ![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/08406169-9e29-4f00-ac05-82aedf09f7c9)
  *Image of the missing Power BI visual (created using Plotly and Dash packages)*

## [Operational Expense (OpEx) Variance Analysis](https://github.com/SujayTalanki/OperationalExpenseVarianceAnalysis)
* Background: The company had budgets for each operational expense (OpEx). If the actual expense for the quarter missed the budget, an accountant would leave a comment for the reason behind the
  "variance" (budget miss). I was tasked with categorizing the general reasons behind these variances.
* Result: Applied unsupervised learning algorithms (NLP and Clustering) to create 10 evenly distributed categories that classified 20,000+ OpEx variance comments. This project allowed accountants and analysts.
  to understand/analyze the reasons behind OpEx variances to prevent occurances in the future!
* Reduced workload significantly and achieved ~ 78% accuracy on hold-out set.
* Developed a python pipeline (pandas, nltk, sentence_transformers, sklearn) that embedded sentences into vectors (BERT LLM) and utilized K-Means clustering to categorize OpEx variance comments.
* Launched a local app (python: plotly and dash) to visualize the key phrases per category. This was used to help analysts summarize the content of the 20,000+ comments.
  
**Workflow Diagram:**  

  ![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/aca14f93-f34c-47b7-be88-faa24ccc679f)

## [Movie Recommender System](https://github.com/SujayTalanki/MovieRecommendationSystem)
* Engineered a content-based recommender system using NLP that takes in a movie and recommends 10 similar movies based on movie attributes and rating.
* Considered movies' description, cast, director, genre, and average rating to suggest movies that the user would enjoy.
* Conducted preprocessing and feature engineering to ensure data quality and enhance model performance.
* Employed CountVectorizer and cosine similarity metric to suggest many similar movies. Retrieved the top 10 highest rated movies from this selection
  to suggest to the user.
* Tools used: Python (Numpy, Pandas, Nltk, Sklearn).

## [Flight Delays Prediction](https://github.com/SujayTalanki/FlightDelaysPrediction)
* [**Report of Findings**](https://github.com/SujayTalanki/FlightDelaysPrediction/blob/master/report.pdf)
* Constructed a machine learning pipeline to predict the severity of a flight’s delay (1M+ flights).
* Performed EDA, feature engineering, cross validation, and hyperparameter tuning (GridSearchCV) to optimize an XGBoost model that achieved 94% accuracy.
* Tools used: Python (Numpy, Pandas, Sklearn, LightGBM, XGBoost, GridSearchCV).

**Report of Findings:**  

  ![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/064e25c8-dcc5-4e85-ad3d-6e7af827c064)  

**Metrics:**  

  ![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/21ace0ee-94c4-46b6-aa46-f252a691e280)  

## [Netflix Stock Price Prediction](https://github.com/SujayTalanki/Netflix-Stock-Prediction)
* Assembled an LSTM Neural Network to predict the closing price of Netflix stock using the last 60 days of time series data.
* LSTM Neural Network contained 3 LSTM layers of 50 neurons each, followed by 3 drouput layers (20%) and 1 dense layer.
* Tuned the batch size to 32 and number of training epochs to 50 in order to acheive optimal performance (~ 4.5 RMSE).
* Tools used: Python (Numpy, Pandas, Matplotlib, TensorFlow, Sklearn).

**Prediction:**  

  ![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/cf51caeb-3c63-4c3d-a28d-3663401856e4)

## [Lead Scoring Model](https://github.com/SujayTalanki/Lead-Scoring)
* Developed a lead scoring model using supervised machine learning algorithms to predict the probability that a loan ("lead") is funded with 93% accuracy.
* After performing cross validation and comparing with several models, the LightGBM classifier performed optimally.
* Led to a simulated profit of ~ $300,000 (in our scenario, assuming a converted lead yields $120 and the time/effort costs around $15).
* Tools used: Python (Numpy, Pandas, PyCaret, LightGBM, Sklearn).

**ROC Curve:**  

  ![image](https://github.com/SujayTalanki/SujayTalanki.github.io/assets/91350869/b69a5ebe-63f5-4cb1-b12b-9ab41831d09a)

