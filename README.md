# CSC180-yelp-reviews
CSC 180-01 Intelligent Systems (Spring 2022)
Project 1: Yelp Business Rating Prediction using Tensorflow
Due at 2:00 pm, Friday, February 25, 2022

1. Problem Formulation
In this project, we aim to predict a business's stars rating based on all the review text for that business
using neural network implementations in TensorFlow. Consider this problem as a regression problem.
(1) Report the RMSE and plot the lift chart of the BEST neural network model you have obtained.
(2) Choose 3-5 arbitrary businesses from your test data (preferably from different categories).
Show the names, the true star ratings, and the predicted ratings (from your best model) of those
businesses.
2. Dataset
https://www.yelp.com/dataset
The dataset contains several JSON files. You can find the format of the data here:
https://www.yelp.com/dataset/documentation/main
Example file formats are as follows.
3. Data Cleaning
In this project, we will only consider the businesses with at least 20 reviews. So remove all the
businesses with less than 20 reviews.
4. Requirements
• You are required to split data to training and test. Use training data to train your models and
evaluate the model quality using test data.

• Use TF-IDF to extract features from reviews. If you experience low memory issue when
using tfidfVectorzier, set parameters max_df, min_df, and max_features appropriately.

• You must use EarlyStopping when training neural networks using Tensorflow.

• Tuning the following hyperparameters when training neural networks using Tensorflow and
record how they affect performance in your report. Save all the models you have tried as a
proof in your notebook and tabulate your findings in your report.

• Activation: relu, sigmoid, tanh

• Number of layers and neuron count for each layer

• Optimizer: adam and sgd.
