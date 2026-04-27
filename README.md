# 📧 Spam Detection Model Evaluation

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.x-F7931E?logo=scikit-learn&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-2.x-150458?logo=pandas&logoColor=white)
![matplotlib](https://img.shields.io/badge/matplotlib-3.x-11557C?logo=matplotlib&logoColor=white)
![seaborn](https://img.shields.io/badge/seaborn-0.13-4C72B0)

A comparative evaluation of four machine learning classification algorithms
for spam message detection, built as part of an IT Academy Python course.

---

## 📁 Project structure

```
├── data/
│   ├── messages.csv              # Raw dataset
│   ├── messages_cleaned.csv      # Cleaned dataset
│   └── confusion_matrices.png    # Evaluation visualizations
├── venv/                         # Virtual environment (not tracked)
├── spam_model_evaluation.ipynb   # Main Jupyter notebook
├── requirements.txt              # Project dependencies
├── .gitignore
└── README.md
```

---

## 🤖 Models compared

| Model | Accuracy | F1 (spam) |
|-------|----------|-----------|
| Logistic Regression | 97.22% | 0.89 |
| Multinomial Naive Bayes | 96.02% | 0.82 |
| Decision Tree | 96.95% | 0.88 |
| **Linear SVC** ✅ | **98.98%** | **0.96** |

---

## 🏆 Result

**Linear SVC** was selected as the best model, achieving the highest accuracy
and F1 score across all evaluated algorithms. It caught 94% of all spam messages
while producing almost no false positives.

---

## 🚀 How to run

1. Clone the repository
   ```bash
   git clone https://github.com/ivanadjuricic/Spam-Detection-Model-Evaluation
   ```

2. Create and activate virtual environment
   ```bash
   python -m venv venv
   venv\Scripts\activate        # Windows
   source venv/bin/activate     # Mac/Linux
   ```

3. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

4. Register Jupyter kernel
   ```bash
   python -m ipykernel install --user --name=venv --display-name "Python (venv)"
   ```

5. Open the notebook
   ```bash
   jupyter notebook spam_model_evaluation.ipynb
   ```

---

## 📦 Dependencies

```
pandas
scikit-learn
ipykernel
matplotlib
seaborn
notebook
```

---

*IT Academy — Introduction to Machine Learning using Python*
