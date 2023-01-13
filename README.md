# NEXT-WORD-PREDICTION-ML

The objective is to predict the next word of the text using Long Short Memory (LSTM). Next-word
prediction is one field of natural language processing that can help to predict the next word. For the
dataset, web scrapping was used. For the libraries, TensorFlow, Keras, NumPy, matplotlib, and NLTK
were used.

Justification for using LSTM:
Vanishing gradient descent is a problem faced by neural networks when it’s for
backpropagation. It has a huge effect and the weight update process is widely affected and the
model becomes useless. So, we used LSTM which has a hidden state and a memory cell with three
gates that are forgotten, read, and input gates.

Dataset:
Web scraping -Web scraping is the process of extracting content and data from a website.

Method:
1) Import the required libraries:
TensorFlow with Keras is used for model building. The LSTM model is
imported from Keras. For NLP tasks, the NLTK library is used.
2) Read the dataset:
Checking the length of the corpus by using the len function on text after
reading and converting everything to lowercase to avoid duplication of
words.
3) Using tokenizers:
The tokenizers are required to split into each word and store them.
4) Getting unique words:
Getting all the unique words and a dictionary with each word in the data
within the list of unique words as the key and its significant portions as
value.
5) Feature Engineering:
Feature engineering will make the words into numerical representations so
that it is easy to process them.
6) Storing features and labels:
X will be used to get the features and Y to get the labels associated with
them.
7) Building the model:
An LSTM model is built and used a Softmax activation at the end to get a few
specific words predicted by the model.
8) Model compilation:
The compilation is done with three major attributes
i. Loss
ii. Optimizer
iii. Metrics – Accuracy
9) Model fitting:
Passing the processed input of two different dimensions with a batch input
size of 128 with a validation split of 5 %.
10) Evaluating the model:
One part of the user’s input statement is given as an input such that the
next word’s numerical vector is predicted.
11) Saving the model:
The model is saved using the save function and loaded. Save the model in
order to retain its updated state of metrics
12) Model validation:
Validating the model with new user input using functionalities like
prepare_input (text has been processed in order to feed into the model),
predict_completion, and predit_completions (newly processed data is being
predicted)

![image](https://user-images.githubusercontent.com/96876262/212297848-84a09c64-fe5c-482c-bf79-749e0122c110.png)
