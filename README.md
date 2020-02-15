# Higgs-Boson-Challenge
My solution to the Higgs Boson Machine Learning Kaggle Challenge.

In [this Kaggle challenge](https://www.kaggle.com/c/higgs-boson/overview), we are given two types of entries in a numerical dataset; rows representing significant signals that has features of a tau-tau decay, and rows representing background signals that has no significance. The signal is usually deeply buried in the noise, so is difficult to identify. The goal is to use machine learning to help distinguish the significant traces that contain meaningful data from the background traces with nothing of significance. The (labeled) dataset provided had a number of missing entries, and these missing entries were arbitrarily provided a value of -999.0, so I had to implement data cleaning and normalizing steps to prevent these from unduly influencing the data. The details of my implementation can be found in the code. I implemented a deep neural network architecture with a cross entropy loss function to perform binary classification: does a particular data vector represent signal or noise? With my architecture, I was able to distinguish meaningful signals from background noise with an accuracy of over 99.5%.
