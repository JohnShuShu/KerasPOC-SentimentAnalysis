Model for identification of Positive/Negative Sentiments in texts using Multi-Layer Perceptron built using Keras API running on TensorFlow.

Explanation:

1. The tweets and their corresponding sentiments are read from 'Sentiment Analysis Dataset.csv'
2. The tweets are tokenized, vectorized and encoded using TfidfVectorizer from sklearn.feature_extraction.text
3. Then the K-Best Features are selected using chi2 statistical function which takes the encoded tweets and labels as input and calculates the importance score of feature.
4. Then the enocoded tweets are transformed so that only the K-Best features are retained.
5. 
