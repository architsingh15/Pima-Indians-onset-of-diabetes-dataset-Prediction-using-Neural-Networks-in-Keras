# Pima-Indians-onset-of-diabetes-dataset-Prediction-using-Neural-Networks-in-Keras

This is a simple Neural Network Implementation using Keras. 
I have used the Pima-Indians-onset-of-diabetes-dataset which you can find on this link: http://archive.ics.uci.edu/ml/datasets/Pima+Indians+Diabetes
You can also fit other data sets of the same type, which can be downloaded from the UCI Machine Learning Repository 

Pre-Requisities: 
    1) Python 2 or 3 installed and configured.
    2) You have SciPy (including NumPy) installed and configured.
    3)You have Keras and a backend (Theano or TensorFlow) installed and configured.

Algorithm:
    1) Initialize the random number generator with any seed you like(I have taken 10)
    2) Download the data set in .csv format and put it in the local working directory as NN.py
    3) Load the data set using loadtxt()
    4) Split the data set into the Independent Variables and the Class to be predicted into Z and Q 
    5) Create a Sequential model and add layers: 
        ^First layer contains 12 neurons and will take 8 input variables(Activation Funtion=rectifier activation functio)
        ^Second layer contains 8 neurons(Hidden layer: Activation Funtion=rectifier activation function)
        ^Output layer will contain one neuron(Activation Funtion=Sigmoid Function:Because its a binary classification: 0 or 1)
    6)Fit the data in the model using fit()(The training process will run for a fixed number of iterations through the dataset called                                                   epochs, that we must specify using the nepochs argument)
    7)Set the number of instances that are evaluated before a weight update in the network is performed, called the batch size
    8)Used model.predict() to predict the class variables. 
