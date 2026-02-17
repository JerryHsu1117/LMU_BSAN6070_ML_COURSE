# CA03 – Decision Tree Income Classification

## 📌 Project Overview

This project applies a Decision Tree classifier to predict whether an individual earns more than $50K per year using Census demographic and employment features.

The objective of this project is to:

- Build a baseline Decision Tree model
- Perform systematic hyperparameter tuning
- Evaluate model performance
- Analyze model interpretability
- Assess overfitting risk
- Generate prediction for a new individual

The entire notebook is structured as a modular, function-based pipeline.

---

## 📊 Dataset

Dataset: Census Income Dataset  
Source:  
https://github.com/ArinB/MSBA-CA-03-Decision-Trees/blob/master/census_data.csv?raw=true

### Target Variable

- 1 → Income > $50K  
- 0 → Income ≤ $50K  

### Feature Examples

- Age  
- Education  
- Occupation  
- Workclass  
- Hours per week  
- Capital gain/loss  
- Marital status  
- Race/Sex group  

---

## 🏗 Project Structure

The notebook is organized into the following layers:

### 1. Project Summary

High-level overview of objective and final results.

---

### 2. Data Foundation Process

- Data loading  
- Data quality analysis  
- Data cleaning  
- Target detection  
- Train/test split  

All preprocessing steps are implemented as reusable functions.

---

### 3. Modeling Layer

- Build baseline Decision Tree
- Generate evaluation metrics
- Plot confusion matrix
- Visualize decision tree
- Measure runtime

#### Hyperparameter Tuning

- Criterion (gini vs entropy)
- Min samples per leaf
- Max features
- Max depth
- Best model selection

---

## 📊 4. Model Evaluation

The model is evaluated using:

- Accuracy  
- Precision  
- Recall  
- F1 Score  
- Confusion Matrix  

Evaluation helps:

- Measure performance
- Detect weaknesses
- Compare baseline vs tuned model
- Support tuning decisions

---

## 🔎 5. Model Interpretation

- Tree visualization  
- Depth analysis  
- Leaf count  
- Overfitting assessment  

Tree complexity:

- Depth = 10  
- Leaves = 307  

Model constraints:

- max_depth = 10  
- min_samples_leaf = 20  

These constraints help reduce overfitting risk.

---

## ⚙️ Model Development Details

### Discretization

Continuous variables were converted into categorical bins before training to:

- Reduce noise  
- Improve interpretability  
- Control tree complexity  
- Prevent excessive splitting  

---

### Best Model Parameters

- criterion = entropy  
- max_depth = 10  
- min_samples_leaf = 20  
- max_features = None  

Training runtime ≈ 0.0604 seconds  

The model remains computationally efficient.

---

## 🎯 6. Final Prediction

For the selected individual:

- Predicted class: Income ≤ $50K  
- Prediction probability: 93.88%  

This indicates high confidence in the classification result.

---

## 🧠 7. Key Takeaways

- Decision Trees provide strong interpretability.
- Discretization improves stability.
- Hyperparameter tuning significantly impacts performance.
- Controlled depth prevents fully grown trees.
- Confusion matrix reveals model weaknesses.
- The model is computationally efficient.

---

## 🛠 Technologies Used

- Python  
- Pandas  
- NumPy  
- Scikit-learn  
- Matplotlib  

---

## 📌 Conclusion

This project demonstrates a complete Decision Tree modeling workflow:

Data preprocessing → Modeling → Evaluation → Hyperparameter Tuning → Interpretation → Prediction

The final model balances:

- Accuracy  
- Interpretability  
- Generalization  
- Computational efficiency  

It reflects a structured and practical machine learning implementation.
