# Ratings Prediction – Deep Learning ⭐🎢

This project applies deep learning to predict review ratings based on natural language reviews and metadata. The dataset contains over 42,000 amusement park reviews, and the goal is to build a neural network that can learn patterns in review text and structured features to predict customer satisfaction scores.

---

## 📌 Objective

Build a regression model using deep neural networks to predict the **Rating** (1 to 5) given structured metadata and the full **ReviewText**. This helps businesses assess customer sentiment and anticipate satisfaction levels based on review content alone.

---

## 📊 Dataset Information

**Total records**: 42,656 theme park visitor reviews  
**Target variable**: `Rating` (from 1 = unsatisfied to 5 = satisfied)

### 🔑 Features:
| Column              | Description                                                       |
|---------------------|-------------------------------------------------------------------|
| `ReviewID`          | Unique numeric ID for each review                                |
| `Rating`            | Satisfaction score (1 to 5)                                       |
| `YearMonth`         | Date of visit (format: YYYY-MM)                                  |
| `ReviewerLocation`  | Country of origin of the reviewer                                |
| `ReviewText`        | Full text of the review (mean length: 130 words, max: 3963)       |
| `Branch`            | The park branch visited (3 possible branches)                    |

---

## 🧠 Model Overview

- **Type**: Deep Neural Network (DNN)
- **Architecture**:
  - Structured inputs (e.g., location, branch, date)
  - Text vectorization (TF-IDF or embeddings) of `ReviewText`
  - Dense layers with dropout and batch normalization
- **Loss Function**: Mean Squared Error (MSE)
- **Evaluation Metric**: Root Mean Squared Error (RMSE)

---

## 🔬 Pipeline Steps

1. **Data Preprocessing**
   - Clean and encode categorical variables
   - Process and tokenize `ReviewText`
   - Normalize numerical features

2. **Model Development**
   - Multi-input model handling both structured and unstructured features
   - Dropout and L2 regularization to combat overfitting

3. **Training & Evaluation**
   - Split dataset into training/validation
   - Tune hyperparameters (e.g., layers, activation, learning rate)
   - Evaluate with RMSE

---

## 🚀 How to Run

### 1- Clone the repo:
```bash
git clone https://github.com/Mariee03/Ratings-Prediction-Deep-Learning.git
cd Ratings-Prediction-Deep-Learning
```

### 2- Launch the notebook:
```bash
jupyter notebook ratings_prediction.ipynb
```

### 3- Run all cells to preprocess data, train the model, and make predictions.

## 📬 Author
Created by Marie Elyse Bassil
Feel free to explore, fork, or get in touch!
