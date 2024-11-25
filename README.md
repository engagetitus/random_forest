# Random Forests  
_Titus Muthomi Kimaani C 004/600178/2024_

---

## Introduction  
- **Topics Covered:**  
  - What is Random Forest  
  - Decision Trees (Recap)  
  - Important Terminologies  
  - Working of Random Forests  
  - Practical Case Study  
  - Advantages and Disadvantages  
  - Applications and Summary  

---

## What is Random Forest  
- An ensemble machine learning algorithm combining multiple decision trees.  
- Applicable for both **classification** and **regression** tasks.  
- Aggregates predictions from multiple trees to improve accuracy.  

---

## Decision Trees (Recap)  
- A graphical representation for deriving all possible solutions to a problem based on conditions.  

---

## Important Terminologies  
- **Root Node:** Starting point of the tree, representing the dataset.  
- **Splitting:** Dividing nodes into sub-nodes to maximize homogeneity.  
- **Decision Nodes:** Intermediate nodes for further splits.  
- **Leaf Nodes:** Terminal nodes containing predictions.  
- **Feature:** A measurable attribute (e.g., age, height, weight).  

---

## Working of Random Forests  
1. **Random Sampling with Replacement:**  
   - Creates multiple subsets of the dataset (Bootstrap Sampling).  
   - Ensures diversity among trees.  

2. **Feature Selection:**  
   - A random subset of features is chosen to split nodes.  
   - Criteria:  
     - Square root of the number of features (classification).  
     - Number of features divided by 3 (regression).  

3. **Ensemble Technique:**  
   - Aggregates outputs (majority vote for classification, mean for regression).  

4. **Splitting Methods:**  
   - **Gini Impurity:** Minimizes misclassification probability.  
   - **Entropy & Information Gain:** Maximizes reduction in uncertainty.  

---

## Practical Case: Penguin Dataset 🐧  
1. **Initial Steps:**  
   - Handle missing values.  
   - Convert categorical data to numeric (e.g., One-Hot Encoding).  
   - Split dataset into training and testing sets.  

2. **Training the Model:**  
   - Train Random Forest with **Gini** and **Entropy** as criteria.  

3. **Evaluation Metrics:**  
   - **Accuracy:** Percentage of correct predictions.  
   - **Confusion Matrix:** Visualizes true vs. predicted outcomes.  
   - **Precision and Recall:** Essential for imbalanced datasets.  

> **GitHub:** [Random Forest Repository](https://github.com/engagetitus/random_forest)

---

## Advantages of Random Forest  
- **Low Variance:** Combines results of multiple trees with reduced overfitting.  
- **Versatile:** Suitable for both classification and regression.  
- **Robust:** Works with both continuous and categorical data.  
- **Normalization Unnecessary:** Operates on a rule-based approach.  
- **Scalable:** Performs well on large datasets.  

---

## Disadvantages of Random Forest  
- Higher **Training Time** compared to single decision trees.  
- Complex to interpret.  
- **Memory Intensive:** Requires more computational resources.  
- Parameter tuning (e.g., `n_estimators`, `max_depth`) needed for optimization.  

---

## Applications and Summary  
- **Healthcare:** Disease prediction.  
- **Finance:** Fraud detection.  
- **E-commerce:** Recommender systems.  
- **Manufacturing:** Predictive maintenance.  

> Random Forests balance accuracy and overfitting through ensemble learning.  
> They are powerful, versatile, and suitable for structured datasets with both categorical and numeric features.  
