# Wine Quality Prediction using Deep Learning

## Overview
This project uses a Deep Learning model built with TensorFlow/Keras to predict whether a wine is of **good** or **bad** quality based on its chemical properties.

The project demonstrates:
- Data preprocessing
- Feature scaling
- Neural network training
- Model evaluation
- Prediction using Deep Learning

---

## Technologies Used
- Python
- TensorFlow / Keras
- Pandas
- NumPy
- Scikit-learn
- Google Colab

---

## Dataset
The dataset contains chemical properties of red and white wines such as:
- Acidity
- Sugar
- pH
- Alcohol
- Sulphates

The `quality` column was converted into binary classes:
- `1` → Good Wine (`quality >= 7`)
- `0` → Bad Wine (`quality < 7`)

---

## Workflow

### 1. Data Preprocessing
- Encoded categorical values
- Handled missing values
- Normalized features using `StandardScaler`

### 2. Model Architecture

```text
Input Layer → Dense(64) → Dense(32) → Output Layer
```

---

## Optimizer and Loss Function

### Adam Optimizer
The **Adam optimizer** was used because it provides:
- Faster convergence
- Efficient weight updates
- Better performance for most Deep Learning tasks

Adam combines the advantages of:
- Momentum
- RMSProp

which helps the model learn more efficiently.

---

### Binary Crossentropy Loss
`binary_crossentropy` was used because this is a **binary classification** problem.

The model predicts:
- `0` → Bad Wine
- `1` → Good Wine

Binary Crossentropy measures how far the predicted probability is from the actual class label.

---

## Training
The model was trained using:
- Adam Optimizer
- Binary Crossentropy Loss
- 20 Epochs

---

## Model Prediction
The trained model predicts whether a wine is:
- Good Quality
- Bad Quality

based on input chemical properties.

---


---

## Future Improvements
- Hyperparameter tuning
- Dropout layers
- Better architectures
- Deployment as a web app

---
