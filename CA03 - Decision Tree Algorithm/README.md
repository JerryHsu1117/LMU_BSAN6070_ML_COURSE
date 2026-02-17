# CA03 – Decision Tree Income Classification

## 📌 Project Overview

This project applies a Decision Tree classifier to predict whether an individual earns more than $50K per year using Census demographic and employment features.

GitHub Link: 

The objective is to:

- Build a baseline Decision Tree model
- Perform systematic hyperparameter tuning
- Evaluate model performance
- Analyze model interpretability
- Assess overfitting risk
- Generate a prediction for a new individual

The entire project is structured in a modular, function-based pipeline.

---

## 📊 Dataset

The dataset used is:

Census Income Dataset  
Source:  
https://github.com/ArinB/MSBA-CA-03-Decision-Trees/blob/master/census_data.csv?raw=true

The dataset includes demographic and work-related attributes such as:

- Age
- Education
- Occupation
- Workclass
- Hours per week
- Capital gain/loss
- Marital status
- Race/Sex group

The target variable is binary:
- 1 → Income > $50K
- 0 → Income ≤ $50K

---

## 🏗 Project Structure

The notebook is organized into the following layers:

### 1. Project Summary  
High-level overview of the objective and results.

### 2. Data Foundation Process  
- Data loading  
- Data quality analysis  
- Data cleaning  
- Target detection  
- Train/test split  

All preprocessing steps are implemented as reusable functions.

### 3. Modeling Layer  
- Baseline Decision Tree  
- Evaluation metrics  
- Hyperparameter tuning (4 runs)
  - Criterion (gini vs entropy)
  - Min samples per leaf
  - Max features
  - Max depth
- Best model selection
- Runtime measurement  

### 4. Model Interpretation  
- Tree visualization  
- Tree complexity analysis  
- Overfitting assessment  

### 5. Final Prediction  
- Create a new individual  
- Predict income class  
- Compute prediction probability  

### 6. Assignment Questions (Q1–Q8)  
Conceptual and analytical explanations supported by code outputs.

### 7. Discussion & Conclusions  
Final summary of findings and model performance.

---

## ⚙️ Model Development

### Discretization

Continuous variables were converted into categorical bins before training.  
This helped:

- Reduce noise
- Improve interpretability
- Control tree complexity
- Prevent excessive splitting

---

### Hyperparameter Tuning

The following hyperparameters were tuned:

- criterion: gini vs entropy  
- min_samples_leaf  
- max_features  
- max_depth  

### Best Model Parameters

The best-performing tree used:

- criterion = entropy  
- max_depth = 10  
- min_samples_leaf = 20  
- max_features = None  

Tree complexity:
- Depth = 10  
- Leaves = 307  

---

## 🚀 Model Performance

- Training runtime ≈ 0.0604 seconds  
- Tree depth = 10  
- Leaves = 307  

The model demonstrates moderate complexity while remaining computationally efficient.

---

## 🔎 Overfitting Analysis

The tree is not fully grown because:

- max_depth is limited to 10  
- min_samples_leaf is set to 20  

These constraints reduce overfitting risk.

Although the tree contains 307 leaves, hyperparameter tuning helped control variance and improve generalization.

---

## 🎯 Final Prediction

For the selected individual:

- Predicted class: Income ≤ $50K  
- Probability: 93.88%  

This indicates high confidence in the classification result.

---

## 🧠 Key Takeaways

- Decision Trees provide strong interpretability.
- Discretization improves stability and reduces overfitting.
- Hyperparameter tuning significantly impacts performance.
- Controlled tree depth prevents fully grown trees.
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

This project demonstrates a complete Decision Tree modeling workflow, including preprocessing, tuning, evaluation, interpretability analysis, and prediction. The final model balances accuracy, interpretability, and computational efficiency.


