# Attention-in-DeepLearning
Simple usage of attention in deep learning. 


The concept with code is taken from https://www.analyticsvidhya.com/blog/2019/11/comprehensive-guide-attention-mechanism-deep-learning/
however, the code is revised for new changes and also made runnable end to end.

So we have data which has two columns, 
reviews (text) and sentiments( binary)

our goal is to predict the sentiment using reviews
X -> df['reviews']
y - df['senti']

In the first pass, we use a simple LSTM without attention, where the last layer of the LSTM output is fed to a dense layer which then predicts the output (0 or 1).

In the second round we use attention, where all the LSTM outputs at each timestep is linearly combined and then fed to a dense layer which predicts the output (0 or 1).


