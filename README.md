# Sentiment Analysis using LSTM and CNN
Sentiment Analysis using LSTM with CNN.   
Using twitter's tweets, its a project to do sentiment analysis on the tweet and find whether it has positive mood or negative mood.   
Using, Keras as a library for the building the neural network to get the sentiment analysis.  

## preprocessing.ipynb
The preprocessing and cleaning of all the texts.   
Since people tend to tweet in all the languages, it is very necessary to translate it to english.   
After Translating it, it is neccesary to clean the data and remove unnecessary texts and characters from the tweet.     
There are various things we remove from the tweet. Here are few
1. Removing links (which removes images too because all images give us links).   
2. Removing all hastags.   
3. Removing all the tags.   
4. Removing the stop words.   
5. Stemming the word english. 
6. Removing all the special characters.  

## LSTM_CNN.ipynb
This is the actual notebook file which does the sentiment analysis.   
For pre-processing, nltk is used.   
For the neural networks, keras is used.     
LSTM is actually an RNN layer. But while training big texts using LSTM, the training time increases. Therefore, we convert the single line of integers into 2D matrix and convol a kernal matrix over the data and make the operations fasters.    
Therefore, we use a CNN model over an RNN model and make our more efficient.   
