# Lung Cancer Prediction using Deep Learning (FNN)

This project aims to predict the presence of lung cancer using a deep learning model built with TensorFlow and Keras. The model is trained on a balanced dataset (`lungCancerDataset_balanced.csv`) and achieves high accuracy using a feedforward neural network architecture.

## 📁 Dataset

- **Input File**: `lungCancerDataset_balanced.csv`
- The dataset is preprocessed to:
  - Encode categorical features using `LabelEncoder`
  - Normalize features using `StandardScaler`
  - Encode the target (`LUNG_CANCER`) as binary (YES → 1, NO → 0)

## 🧠 Model Architecture

- **Model Used** : Feedforward Neural Network (also known as a Multilayer Perceptron or MLP)
- **Input Layer**: Dense(64, ReLU)
- **Dropout**: 30%
- **Hidden Layer**: Dense(32, ReLU)
- **Dropout**: 20%
- **Output Layer**: Dense(1, Sigmoid) – for binary classification

## 🛠️ Training Details

- Optimizer: Adam
- Loss Function: Binary Crossentropy
- Metrics: Accuracy
- Early Stopping used to avoid overfitting with patience of 5

## 📊 Performance

- Achieved **~92.6% accuracy** on the test set.

## 💾 Model Saving

- The trained model is saved as `lung_cancer_model.keras`.

## 🔧 Installation

```
pip install -r requirements.txt
```
