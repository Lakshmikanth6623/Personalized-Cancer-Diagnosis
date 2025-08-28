<<<<<<< HEAD
# Personalized-Cancer-Diagnosis
=======
# Personalized Cancer Diagnosis  

### Author: **LakshmiKanth**  

## 📌 Project Overview  
This project aims to build a **Personalized Cancer Diagnosis system** that classifies patients into different cancer types based on **genetic mutation data** and **clinical text data**. The goal is to assist doctors in recommending more accurate and **personalized treatments**.  

It is a **multi-class classification problem**, where each data point belongs to one of nine cancer classes.  

---

## 📊 Dataset  
- **training_variants.csv** → structured data (Gene, Variation, Class).  
- **training_text.csv** → unstructured data (clinical text from research literature).  

Each sample is described by both mutation information and associated text evidence.  

---

## ⚙️ Approach  
1. **Data Preprocessing**  
   - Text cleaning (stopword removal, tokenization, punctuation removal).  
   - Encoded categorical features (gene/variation).  
   - Handled class imbalance using **SMOTE**.  

2. **Feature Engineering**  
   - **TF-IDF** for text.  
   - **One-hot encoding** for gene and variation.  
   - **Dimensionality reduction** using SVD and t-SNE (for visualization).  

3. **Modeling**  
   - Algorithms tested:  
     - Naive Bayes  
     - Logistic Regression  
     - KNN  
     - SVM  
     - Random Forest  
     - SGD Classifier  
   - **Stacking Classifier (Ensemble)** improved performance.  

4. **Evaluation**  
   - Metrics: **Log Loss** (primary) and Accuracy (secondary).  
   - Best results achieved with **Stacking + Combined Features**.  

---

## ✅ Results & Key Insights  
- Combining **structured (mutation)** + **unstructured (text)** data significantly improved classification.  
- Ensemble methods (stacking) outperformed individual models.  
- This workflow demonstrates the potential of ML in **precision medicine**.  

---

## 📂 Project Structure  
```
Personalized-Cancer-Diagnosis/
│── 1.1. PersonalizedCancerDiagnosis.ipynb   # Main notebook
│── data/                                    # Dataset folder
│── requirements.txt                         # Dependencies
│── README.md                                # Project description
```

---

## 🚀 How to Run  
1. Clone the repository:  
   ```bash
   git clone https://github.com/<your-username>/Personalized-Cancer-Diagnosis.git
   cd Personalized-Cancer-Diagnosis
   ```
2. Install dependencies:  
   ```bash
   pip install -r requirements.txt
   ```
3. Open the Jupyter Notebook:  
   ```bash
   jupyter notebook 1.1. PersonalizedCancerDiagnosis.ipynb
   ```

---

## 🛠️ Tech Stack  
- **Python** (pandas, numpy, scikit-learn, nltk, imbalanced-learn, mlxtend)  
- **NLP** (TF-IDF, Bag-of-Words)  
- **Machine Learning** (classification models, ensemble learning)  
- **Visualization** (matplotlib, seaborn, t-SNE)  

---

## ✨ Author  
👤 **LakshmiKanth**  
- [GitHub](https://github.com/)  
- [LinkedIn](https://linkedin.com/) (add your profile link here)  
>>>>>>> caae411 (Initial commit - Personalized Cancer Diagnosis project)
