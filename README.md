# **Sentiment Analysis for Airline Tweets**

## **Introduction**
Sentiment analysis, also called opinion mining, is a technique that uses natural language processing (NLP) to determine the emotional tone or sentiment expressed in a piece of text. In this project, we analyze tweets directed at major US airline companies to understand public sentiment.

## **Problem Statement**
Airline companies face the challenge of managing many customer comments and feedback. An effective sentiment analysis model is crucial for evaluating public sentiment and providing actionable insights to enhance operational efficiency and improve customer satisfaction.

## **Data Collection**
### **Source of Data**
- **Twitter US Airline Sentiment dataset on Kaggle**
- **Tweets directed to major US airline companies (United, US Airways, Delta, etc.)**

### **Collection Timeframe**
- **Data scraped from Twitter in February 2015**

### **Labeling**
- **Contributors manually labeled tweets into three categories: Positive, Neutral, or Negative sentiment**

### **Data Columns**
- **tweet_id:** Unique identifier for each tweet
- **airline_sentiment:** Sentiment label (Positive, Neutral, Negative)
- **airline:** Mentioned airline in the tweet (e.g., United, US Airways, Delta)
- **text:** Actual text content of the tweet

## **Data Preprocessing**
Several essential preprocessing and normalization techniques were applied:
- **Transforming text to lowercase**
- **Removing duplicate rows**
- **Dropping missing values**
- **Tokenizing tweets into individual words**
- **Removing stop words**
- **Applying stemming**

## **Feature Engineering**
### **Sampling Using SMOTE**
To address class imbalance, we implemented the Synthetic Minority Over-sampling Technique (SMOTE).

### **TF-IDF Vectorization**
We employed the TF-IDF (Term Frequency - Inverse Document Frequency) vectorization technique to extract meaningful features from the textual data.

### **One-Hot Encoding**
For efficient encoding of the target column, we utilized one-hot encoding, adding three additional features: 'positive,' 'negative,' and 'neutral.'

## **Models Used**
### **Gradient Boosting**
- **Achieved an accuracy of 81.1353%**
- **Hyper-parameters:** 200 estimators and a tree depth of 6

### **Support Vector Machine (SVM)**
- **Achieved 79% accuracy with solid precision and recall for negative sentiment**

### **Neural Network**
- **Deep learning models capable of automatically learning intricate patterns**

## **Results**
The models were evaluated for their performance in sentiment classification, with Gradient Boosting showing the highest accuracy.

## **Conclusion**
The sentiment analysis model provides valuable insights into public opinion about major US airlines, which can help improve customer satisfaction and operational efficiency.

## **References**
- **Twitter US Airline Sentiment dataset on Kaggle**


