Employee Sentiment Analysis Project
📊 Overview

This project analyzes employee messages to assess sentiment and engagement using Natural Language Processing (NLP) and statistical modeling.
It was completed as part of an internal AI evaluation assignment using the dataset test.csv (unlabeled).

The notebook processes raw text, labels sentiment automatically, calculates employee sentiment scores, ranks employees, detects potential “flight risks,” and builds a predictive regression model to study sentiment trends.

🎯 Project Objectives

Sentiment Labeling: Classify each message as Positive, Negative, or Neutral using TextBlob and VADER hybrid analysis.

Exploratory Data Analysis (EDA): Explore the dataset, visualize sentiment trends, and understand engagement patterns.

Employee Score Calculation: Compute monthly sentiment scores per employee.

Employee Ranking: Rank employees by positive and negative sentiment scores.

Flight Risk Identification: Identify employees who sent 4+ negative messages in a month.

Predictive Modeling: Build a Linear Regression model to predict sentiment trends using behavioral features.

🧩 Dataset

File: test.csv

Unlabeled employee messages dataset.

Preprocessed and cleaned during the analysis pipeline.

Augmented with new columns:

clean_message

sentiment_label

polarity_score

month

avg_sentiment

⚙️ Tools & Libraries

Python 3.x

Libraries:

pandas, numpy, matplotlib, seaborn

textblob, nltk, vaderSentiment

scikit-learn (for Linear Regression)

Environment: Jupyter Notebook

🧾 Key Tasks Summary
🧮 Task 1: Sentiment Labeling

Used a hybrid model combining TextBlob and VADER for accurate classification into Positive, Negative, or Neutral.
A new column sentiment_label was added to the dataset.

🔍 Task 2: Exploratory Data Analysis (EDA)

Visualized sentiment distribution and employee engagement trends.

Identified top contributors and patterns in monthly sentiment activity.

💬 Task 3: Employee Score Calculation

Each message was scored as:

Positive → +1

Negative → -1

Neutral → 0
Monthly average sentiment scores were then calculated per employee.

🏆 Task 4: Employee Ranking

Generated top 3 Positive and Negative employees per month using the calculated sentiment scores.

🚩 Task 5: Flight Risk Identification

Flagged employees as flight risks if they sent 4 or more negative messages in a single month.

📈 Task 6: Predictive Modeling

Developed a Linear Regression Model using features like:

Number of messages

Average message word count

Percentage of negative messages

Model performance metrics:

R² Score: ~0.57

RMSE & MAE: Acceptable error margins showing moderate predictive power.

📊 Visualizations

All visualizations (EDA charts, sentiment trends, and ranking plots) are saved in the /visualizations folder.
Examples include:

Sentiment distribution plot

Monthly sentiment trend per employee

Top positive vs. negative employee charts

🧠 Insights

Majority of employee messages had neutral or positive sentiment.

Few employees consistently produced negative messages → potential disengagement.

Flight risk employees correlated strongly with frequent negative sentiment over short periods.

The regression model indicates message frequency and negativity ratio significantly influence overall sentiment.

