# ANN Regression Model - Combined Cycle Power Plant Energy Output Prediction

This project involves building an Artificial Neural Network (ANN) regression model using TensorFlow/Keras to predict the electrical energy output (in MW) of a Combined Cycle Power Plant based on environmental variables.

## 🌟 Project Objective

Predict the net hourly electrical energy output (PE) of a Combined Cycle Power Plant using the following input features:
- Ambient Temperature (AT)
- Ambient Pressure (AP)
- Relative Humidity (RH)
- Exhaust Vacuum (V)

## 📁 Dataset

- **Source**: UCI Machine Learning Repository  
- **Link**: [CCPP Dataset](https://archive.ics.uci.edu/ml/datasets/Combined+Cycle+Power+Plant)
- **Size**: 9568 data points collected over 6 years (2006–2011)
- **Features**:
  - `AT`: Temperature in °C
  - `V`: Exhaust vacuum in cm Hg
  - `AP`: Ambient pressure in millibar
  - `RH`: Relative humidity in %
  - `PE`: Net hourly electrical energy output (Target)

## 🧠 Model Architecture

- Input Layer: 4 neurons (one for each feature)
- Hidden Layers: 
  - Dense layer with 64 neurons (ReLU)
  - Dense layer with 32 neurons (ReLU)
- Output Layer: 
  - Dense layer with 1 neuron (Linear activation)
- Optimizer: `Adam`
- Loss: `Mean Squared Error (MSE)`

## ⚙️ Requirements

- Python 3.x
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib / Seaborn (for visualization)
- Scikit-learn (for preprocessing and evaluation)

## 🔧 Setup and Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/ccpp-ann-regression.git
   cd ccpp-ann-regression
