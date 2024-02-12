## Twitter_sentiment_classification
This code implements sentiment analysis on Twitter data using a Long Short-Term Memory (LSTM) neural network model. Here's a brief overview of what each part of the code accomplishes:

# Data Loading and Preprocessing:

Loads the Twitter data from a CSV file and removes any rows with missing values.
Defines a function clean_text to preprocess the text data, including converting to lowercase, handling contractions, removing URLs, punctuation, numbers, and stopwords.
# Tokenization and Padding:

Tokenizes the cleaned text using Tokenizer from Keras and pads the sequences to a fixed length.
Assigns labels for sentiment analysis.
# Model Building:

Constructs an LSTM model using Keras Sequential API.
Embeds the tokenized sequences, adds a Bidirectional LSTM layer with 64 units, and includes two dense layers with ReLU and softmax activation functions for classification.
# Model Compilation and Training:

Compiles the model with sparse categorical cross-entropy loss and Adam optimizer.
Fits the model on the training data for a specified number of epochs.
# Evaluation:

Evaluates the model performance on the test data and prints the test accuracy.
# Prediction:

Defines a function predict_sentiment to predict sentiment for new input text.
Preprocesses the input text, tokenizes, pads, and then predicts sentiment using the trained model.
