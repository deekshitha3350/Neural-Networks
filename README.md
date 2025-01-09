# Neural-Networks

This project utilizes the Keras and TensorFlow libraries to build an ANN for classifying letters from a given dataset. The process includes the following steps:

Data Preprocessing:

Loading the dataset.
Handling missing values and encoding categorical variables.
Splitting the data into features (X) and target (Y).
Normalizing the data for better model performance.
Model Building:

Building a simple ANN with two hidden layers.
Using ReLU activation for the hidden layers and sigmoid activation for the output layer.
Hyperparameter Tuning:

Using Keras Tuner to find the best hyperparameters for the model.
Searching for the best number of units in each layer and the optimal number of epochs.
Model Evaluation:

Evaluating the model performance on a test set and printing the classification report.
Data
The dataset used in this project is named Alphabets_data.csv. It consists of various features that represent characteristics of each letter of the alphabet. The target variable (letter) is categorical and represents the letter corresponding to each set of features.

Model
The model is built using the Keras Sequential API, consisting of:

Input Layer: Takes in the preprocessed data.
Hidden Layers: Two hidden layers with ReLU activation.
Output Layer: A softmax activation layer to classify the data into one of the letters.
The model is compiled using the Adam optimizer and binary crossentropy loss function for training.

Hyperparameter Tuning
The model is further optimized using Keras Tuner, which performs a Random Search to find the best combination of units for each hidden layer.

Results
The model's performance is evaluated on the test data, and the results are summarized using a classification report that includes precision, recall, and F1 score.

License
This project is licensed under the MIT License - see the LICENSE file for details.
