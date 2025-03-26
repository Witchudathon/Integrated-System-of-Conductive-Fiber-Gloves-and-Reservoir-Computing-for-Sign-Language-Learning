Library for Integrating the reservoir computing models (echo state networks) for Sign Language Learning Classification

Overview
This project implements a Reservoir Computing framework using Echo State Networks (ESNs) for time series classification, specifically for hand movement monitoring.
Input Data Requirements

Training and test data must be in the form of 3D NumPy arrays with shape [N, T, V]:
N: Number of samples
T: Number of time steps per sample
V: Number of variables per sample
Labels for training and test data should be provided in one-hot encoding format with shape [N, C], where C is the number of classes.

Step 1: Setting Up the Reservoir
Create an instance of the ESN class by specifying key parameters:
Number of input nodes
Number of reservoir nodes
Number of output nodes

Step 2: Training the Reservoir
Train the model using the training data:

Step 3: Testing the Model
Evaluate the model using the test data: y_pred = esn_model.predict(X_test)

Visualization
You can visualize the predictions using Matplotlib.

Additional Tips
Adjust the reservoir_size for larger datasets to improve performance.
Ensure input data is properly normalized before feeding into the ESN.
Experiment with different hyperparameters such as spectral radius and leaking rate.
