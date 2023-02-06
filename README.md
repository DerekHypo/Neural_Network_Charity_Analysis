# Neural_Network_Charity_Analysis

# Overview of the analysis
The purpose of this project is to use deep-learning neural networks with the TensorFlow platform in Python, to analyze and classify the success of charitable donations.
Use the following methods for the analysis:

* Preprocessing the data for the neural network model,
* Compile, train and evaluate the model,
* Optimize the model.
# Results

# Data Preprocessing
* What variable(s) are considered the target(s) for your model?
What variable(s) are considered the target(s) for your model? We can see in the picture above that the target variable in this "IS_SUCCESSFUL" column.

* What variable(s) are considered to be the features for your model?
The feature variables would be the remaining variables in our database. They are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, and ASK_AMT.

* What variable(s) are neither targets nor features, and should be removed from the input data?
The two variables of EIN and NAME. Each variable was dropped from our data set.

# Compiling, Training, and Evaluating the Model
* How many neurons, layers, and activation functions did you select for your neural network model, and why?
This deep-learning neural network model is made of two hidden layers with 80 and 30 neurons. The input data has 43 features and 25,724 samples.
The output layer is made of a unique neuron as it is a binary classification.
To speed up the training process, I used the activation function ReLU for the hidden layers. As our output is a binary classification, Sigmoid is used on the output layer. For the compilation, the optimizer is adam and the loss function is binary_crossentropy.

* Were you able to achieve the target model performance?
The model accuracy is under 75%. This is not a satisfying performance to help predict the outcome of the charity donations.

* What steps did you take to try and increase model performance?
To increase the performance of the model, I applied bucketing to the feature ASK_AMT and organized the different values by intervals, increased the number of neurons on one of the hidden layers and used a model with three hidden layers, and tried a different activation function (tanh). None of these steps improve the model's overall performance.

# Summary
