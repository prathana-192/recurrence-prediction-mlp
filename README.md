# Recurrence Prediction with Neural Networks

This project builds a feed-forward neural network (MLP) using TensorFlow/Keras to predict recurrence outcomes based on patient or event data.

# Dataset
- Input: Multiple features categorical + numerical
- Target: `Recurred` binary: Yes/No

 The dataset should include a column "Recurred" as the target variable.  

#  Workflow
1. **Preprocessing**
   - Label encoding of target variable  
   - One-hot encoding for categorical features  
   - Standardization of numerical features  

2. **Model Architecture**
   - Dense(32, relu) + Dropout(0.3)  
   - Dense(16, relu) + Dropout(0.3)  
   - Dense(1, sigmoid)  

3. **Training**
   - Optimizer: Adam  
   - Loss: Binary Crossentropy  
   - Metrics: Accuracy  
   - EarlyStopping callback to prevent overfitting  

4. **Evaluation**
   - Test Accuracy  
   - Classification Report  
   - Confusion Matrix  

5. **Visualization**
   - Training vs Validation Accuracy  
   - Training vs Validation Loss  

# Usage
Clone the repository and install dependencies:
```bash
git clone https://github.com/prathana-192/recurrence-prediction-mlp.git
cd recurrence-prediction-mlp
pip install -r requirements.txt
