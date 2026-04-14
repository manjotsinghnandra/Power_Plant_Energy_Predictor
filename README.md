# Power Plant Energy Prediction using ANN

## Project Overview
This project uses an Artificial Neural Network (ANN) to predict power plant energy output based on environmental conditions. It demonstrates a complete deep learning workflow including data preprocessing, model building, training, and evaluation.

---

## Dataset Information

Features used:
- AT: Temperature  
- V: Exhaust Vacuum  
- AP: Ambient Pressure  
- RH: Relative Humidity  

Target:
- PE: Energy Output  

Dataset size: 9568 rows × 5 columns

---

## Data Preprocessing

- No missing values in dataset
- Features and target separated
- Train-test split (80-20)
- Feature scaling using StandardScaler
- Data converted to PyTorch tensors

---

## Model Architecture

Artificial Neural Network with:
- Input layer: 4 features
- Hidden Layer 1: 6 neurons (ReLU)
- Hidden Layer 2: 6 neurons (ReLU)
- Output Layer: 1 neuron (Regression)

---

## Training Details

- Loss Function: Mean Squared Error (MSE)
- Optimizer: Adam
- Epochs: 100
- Batch Size: 32
- Best model saved using validation loss

---

## Model Performance

- Training MSE: 20.36  
- Testing MSE: 18.71  
- R² Score: 0.93  

The model shows strong predictive performance with high accuracy.

---

## Results

- Predictions closely match actual values
- Model generalizes well on unseen data
- Low validation loss indicates minimal overfitting

---

## Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn  
- PyTorch  
- Matplotlib  

---

## How to Run

```bash
# Clone repository
git clone https://github.com/your-username/power-plant-ann.git

# Install dependencies
pip install -r requirements.txt

# Run the notebook/script
