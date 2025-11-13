# 🍷 Wine Quality Prediction using Machine Learning

## 📘 Project Overview
This project aims to predict the **quality of white wine** based on its **physicochemical properties** using machine learning models.  
The dataset used originates from the **Vinho Verde region of Portugal**, containing chemical measurements such as acidity, pH, alcohol, sulphates, and sugar levels.  

By leveraging **classification algorithms**, the project demonstrates how data-driven insights can replace or support traditional sensory evaluations by wine tasters.

---

## 🧪 Dataset Description
The dataset used is the **White Wine Quality Dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wine+Quality).

| Feature Type | Example Attributes |
|---------------|--------------------|
| **Input Variables** | Fixed Acidity, Volatile Acidity, Citric Acid, Residual Sugar, Chlorides, Free & Total Sulfur Dioxide, Density, pH, Sulphates, Alcohol |
| **Output Variable** | Quality (score between 0–10, rated by wine experts) |

To simplify classification:
- Quality ≤ 4 → **Low**
- Quality 5–6 → **Medium**
- Quality ≥ 7 → **High**

---

## ⚙️ Methodology

1. **Data Preprocessing**
   - Handled missing values and normalized features.
   - Converted quality scores into categorical labels (Low, Medium, High).
   - Applied **resampling** to balance class distribution.

2. **Exploratory Data Analysis (EDA)**
   - Identified relationships between features using heatmaps and correlation matrices.
   - Found that **Alcohol** and **Volatile Acidity** are the most influential features.

3. **Model Training**
   - Implemented multiple classification algorithms:
     - Logistic Regression  
     - Decision Tree  
     - Support Vector Machine (SVM)  
     - Random Forest  
     - K-Nearest Neighbors (KNN)
   - Performed 80/20 train-test split and cross-validation.

4. **Evaluation Metrics**
   - Accuracy  
   - Precision, Recall, F1-score  
   - Confusion Matrix  

---

## 📊 Results

| Model | Accuracy (Before Resampling) | Accuracy (After Resampling) |
|--------|------------------------------|------------------------------|
| Random Forest | **83.63%** | **85.93%** |
| SVM | 80.83% | 82.20% |
| Decision Tree | 75.96% | 74.56% |
| KNN | 73.92% | 77.16% |

**Key Findings:**
- The **Random Forest** model achieved the best overall performance.  
- Resampling improved fairness across classes, especially for *Low* and *High* quality wines.  
- Alcohol content, sulphates, and volatile acidity were the top predictors of wine quality.

🖼️ *Visualization samples (add your images)*  
- Validation Accuracy Comparison  
- Confusion Matrices (Before & After Resampling)  
- Feature Importance Graph  
- F1-Score Table  

---

## 💻 Technologies Used
- **Programming Language:** Python 3.10+  
- **Libraries:** NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn  
- **Environment:** Google Colab / VS Code  
- **Dataset Source:** UCI Repository / Kaggle  

---

## 🚀 How to Run the Project

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/<your-username>/Wine-Quality-Prediction.git
cd Wine-Quality-Prediction
