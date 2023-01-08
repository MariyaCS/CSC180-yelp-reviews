# CSC180-yelp-reviews
CSC 180-01 Intelligent Systems (Spring 2022)
Project 1: Yelp Business Rating Prediction using Tensorflow
Due at 2:00 pm, Friday, February 25, 2022

1. Problem Formulation <br />
In this project, we aim to predict a business's stars rating based on all the review text for that business
using neural network implementations in TensorFlow. Consider this problem as a regression problem. <br />
(1) Report the RMSE and plot the lift chart of the BEST neural network model you have obtained. <br />
(2) Choose 3-5 arbitrary businesses from your test data (preferably from different categories). <br />
Show the names, the true star ratings, and the predicted ratings (from your best model) of those
businesses. <br />
2. Dataset<br />
https://www.yelp.com/dataset <br />
The dataset contains several JSON files. You can find the format of the data here: <br />
https://www.yelp.com/dataset/documentation/main <br />
Example file formats are as follows. <br />
3. Data Cleaning <br />
In this project, we will only consider the businesses with at least 20 reviews. So remove all the
businesses with less than 20 reviews.
4. Requirements <br />
• You are required to split data to training and test. Use training data to train your models and
evaluate the model quality using test data. <br />

• Use TF-IDF to extract features from reviews. If you experience low memory issue when
using tfidfVectorzier, set parameters max_df, min_df, and max_features appropriately. <br />

• You must use EarlyStopping when training neural networks using Tensorflow. <br />

• Tuning the following hyperparameters when training neural networks using Tensorflow and
record how they affect performance in your report. Save all the models you have tried as a
proof in your notebook and tabulate your findings in your report. <br />

• Activation: relu, sigmoid, tanh <br />

• Number of layers and neuron count for each layer <br />

• Optimizer: adam and sgd.
