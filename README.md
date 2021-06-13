# PiBOT

It's a simple chatbot that recognizes emotions i.e. it is a software application used to conduct chat conversation via text. (This software is implemented in Python)

The dataset is in JSON format, where we loop through all the dictionaries (intents) of the dataset.

We apply some text preprocessing which includes:
    1. Converting the entire text into uppercase or lowercase
    2. Stemming to get the root of the word.
    3. Tokenization to convert hte normal text strings into a list of tokens.

We create a bag of words using one-hot encoding as an input for our neural network that we are going to use. This contains only 1s and 0s and therefore it can be used as an input for neural networks.

We are going to build our model using tflearn.
This model contains an input layer, 2 fully connected hidden layers and an output layer. We are going to add regression and apply that to our neural network. 