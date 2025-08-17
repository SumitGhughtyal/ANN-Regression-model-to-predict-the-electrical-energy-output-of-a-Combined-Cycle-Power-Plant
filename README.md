# Power Plant Energy Output Prediction using an Artificial Neural Network

This project is an implementation of an Artificial Neural Network (ANN) to solve a regression problem. The goal is to predict the net hourly electrical energy output (PE) of a combined cycle power plant.

The model is built using TensorFlow's Keras API and trained on a dataset containing hourly average ambient variables.

## Dataset

The project uses the **Combined Cycle Power Plant** dataset, which is provided in the `Folds5x2_pp.xlsx` file. The dataset contains 9568 data points collected over a six-year period.

The features are:
- **Ambient Temperature (AT)**
- **Ambient Pressure (AP)**
- **Relative Humidity (RH)**
- **Exhaust Vacuum (V)**

The target variable is:
- **Net hourly electrical energy output (PE)**

## Model Architecture

The ANN is a sequential model with the following structure:
- **Input Layer**
- **Two Hidden Layers:** Each with 6 neurons and the ReLU (Rectified Linear Unit) activation function.
- **Output Layer:** A single neuron to predict the continuous value of PE.

The model is compiled using the **Adam optimizer** and the **Mean Squared Error** loss function, which is suitable for regression tasks.

## Requirements

The project requires Python and the following libraries:
- NumPy
- Pandas
- TensorFlow
- Scikit-learn

You can install the necessary libraries using pip:
```bash
pip install numpy pandas tensorflow scikit-learn openpyxl
