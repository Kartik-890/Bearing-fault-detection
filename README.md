# Bearing-fault-detection
This repository contains a machine learning program for detecting types of faults in bearings using vibration sensor data. The program is designed to process vibration data, prepare it for training, and then train a neural network model for fault classification.
# File Data Preparation
# Extracting file path
The data preparation starts by extracting file paths for both normal and faulty bearing data. The code uses a specified base path and iterates through different RPM values to create a list of file paths.
# Data Labeling
Loading and Labeling Data
The program loads data from MAT files, extracts titles, and creates DataFrames for each data file. It then combines these DataFrames, removes unnecessary rows, and adds labels to create a final labeled DataFrame. The resulting DataFrame is saved as labelled_data.csv.

# Data Preparation
Preparing Data for Model Training
The data is further processed to remove NaN values, create a count DataFrame, and generate a final DataFrame suitable for training. The final DataFrame is saved as labelled_data.csv.

# Model Training
Neural Network Model
The code defines and trains a neural network model using TensorFlow and Keras. The model architecture consists of convolutional layers with max-pooling, followed by fully connected hidden layers. The output layer uses softmax activation for multiclass classification.

# Usage Instructions
1.File Data Preparation: Execute the code in the "File Data Preparation" section to extract and label bearing data from MAT files.

2.Data Preparation: Execute the code in the "Data Preparation" section to further process the labeled data for model training.

3.Model Training: Execute the code in the "Model Training" section to train the neural network model using the prepared data.

4.Evaluation: Evaluate the trained model on the test set to assess its accuracy in bearing fault detection.
