# Gesture Maze - Research & Experimentation

This branch contains all training experiments and MLflow logs for building a hand gesture recognition model to navigate a maze game.

## 🧪 Project Scope

- Train and evaluate multiple classifiers (Random Forest, SVM, KNN)
- Log experiments using MLflow
- Normalize and preprocess hand landmark data
- Select the best-performing model for deployment

## 📊 Model Comparison

| Model     | Accuracy | Parameters                  | Notes                    |
|-----------|----------|-----------------------------|--------------------------|
| Random Forest | 0.94     | n_estimators=100           | Best performance overall |
| SVM       | 0.91     | kernel=rbf                  | Good, slower inference   |
| KNN       | 0.89     | n_neighbors=5               | Simple but less accurate |

✅ Selected Model: **Random Forest**

## 📁 Project Structure

gesture-maze-research/
├── notebooks/
│ └── training_with_mlflow.ipynb
├── models/
│ └── best_model.pkl
├── mlruns/ # MLflow experiment tracking logs
├── requirements.txt
└── README.md # This file


## 🔧 How to Run

1. Install dependencies:
   pip install -r requirements.txt
2. Run notebook:
   jupyter notebook notebooks/training_with_mlflow.ipynb
3. Start MLflow UI:
   mlflow ui
