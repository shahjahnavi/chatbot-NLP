## Chatbot using TensorFlow and Natural Language Processing (NLP)

This repository contains code for a chatbot built using TensorFlow and NLP techniques. The chatbot can be trained on a dataset of intents and patterns, and it can then be used to generate responses to user queries.

## Dependencies

The code requires the following Python libraries:

1. nltk
2. tflearn
3. tensorflow

## Training the Chatbot

To train the chatbot, follow these steps:

1. **Data Preparation:** Create a JSON file named "intents.json" that contains the intents and patterns for the chatbot. The JSON file should have the following structure:

   ```json
   {
       "intents": [
           {
               "tag": "greeting",
               "patterns": ["Hi", "Hello", "Good morning"],
               "responses": ["Hi there!", "Hello!", "Good day!"]
           },
           ...
       ]
   }
   

2. **Data Processing:** Run the code to preprocess the data and generate the training and output matrices. This will create a pickle file named "data.pickle" that stores the processed data.

3. **Model Training:** Train the chatbot model using the "model.fit()" function. This will train the model to predict the correct intent for a given input.

4. **Model Saving:** Save the trained model using the "model.save()" function. This will create a TensorFlow model file named "model.tflearn".

## Using the Chatbot

To use the chatbot, follow these steps:

1. **Load the Model:** Load the trained model using the "model.load()" function. This will load the model into memory.

2. **Start Conversation:** Start the chatbot conversation using the "chat()" function. This will prompt the user for input and generate responses accordingly.

## Example Usage

python
import nltk
import os
from nltk.stem.lancaster import LancasterStemmer
import numpy
import tflearn
import tensorflow
from tensorflow.python.framework import ops
import random
import json
import pickle

chat()


This code will load the trained model and start the chatbot conversation. The user can then type in questions and the chatbot will generate responses.


Sources :
https://github.com/deadven7/Chatbot-Machine_Learning
https://github.com/JiteshRawat/Rawbot_the_chatbot

