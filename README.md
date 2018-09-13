Model for identification of Positive/Negative Sentiments in texts using Multi-Layer Perceptron built using Keras API running on TensorFlow.

Explanation:

1. The tweets and their corresponding sentiments are read from 'Sentiment Analysis Dataset.csv'
2. The tweets are tokenized, vectorized and encoded using TfidfVectorizer from sklearn.feature_extraction.text
3. Then the K-Best Features are selected using chi2 statistical function which takes the encoded tweets and labels as input and calculates the importance score of feature.
4. Then the enocoded tweets are transformed so that only the K-Best features are retained.
5. Then MLP is defined and compiled which consists of 4 layers: 2 Dense and 2 Dropout
6. 1st Dense Layer consists of 32 neurons and uses 'relu' activation function.
7. 2nd Dense Layer consists of 1 neurons and uses 'sigmoid' activation function.
8. Then using the encoded tweets, we train the contructed model.
9. Once trained, this model can be used to predict the sentiment behind any text entered by the user.
