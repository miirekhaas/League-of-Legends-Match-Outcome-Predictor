
# 🎮 League of Legends Match Outcome Predictor

Predict the outcome of League of Legends matches using key game features and a Logistic Regression model implemented in PyTorch.

---

## 📊 Project Overview

This project analyzes 171,239 League of Legends match records to predict whether **Team 1 (Blue)** or **Team 2 (Red)** will win. It uses early-game indicators like first blood, tower kills, dragon kills, and champion selections. The model is built from scratch using **PyTorch** and evaluated with accuracy, loss curve, and confusion matrix visualizations.

---

## 📁 Dataset

- **Name**: `games.csv`
- **Size**: ~17 MB
- **Rows**: 171,239
- **Path**: `/datasets/_deepnote_work/20250731-171239/games.csv`

### Features Used:
| Feature | Description |
|--------|-------------|
| `firstBlood` | Which team drew first blood |
| `firstTower`, `firstBaron`, `firstDragon` | Early-game objectives |
| `t1_*`, `t2_*` | Champion IDs, spells, bans, kills, etc. |
| `winner` | Target column (1 if team1 wins, 0 otherwise) |

---

## 🧠 Model Summary

| Item | Details |
|------|---------|
| **Model** | Logistic Regression |
| **Framework** | PyTorch |
| **Loss Function** | Binary Cross-Entropy |
| **Optimizer** | Adam |
| **Epochs** | 10 |
| **Batch Size** | 128 |
| **Learning Rate** | 0.001 |

---

## 📈 Results & Visuals

### 🎯 Accuracy
- Achieved around **71% validation accuracy**

### 📊 Loss & Accuracy Curves
<img src="images/accuracy_curve.png" width="500"/>

### 🧩 Confusion Matrix
<img src="images/confusion_matrix.png" width="400"/>

### 🔍 Insightful Plots
#### Win Rate by First Baron
<img src="images/winrate_baron.png" width="400"/>

---

## ▶️ How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/league-match-predictor.git
   cd league-match-predictor
   ```

2. Install requirements:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch the notebook:
   ```bash
   jupyter notebook notebooks/match_outcome_prediction.ipynb
   ```

---

## 🔧 Requirements

See `requirements.txt`. Major packages:
- torch
- pandas
- matplotlib
- seaborn
- scikit-learn

---

## 📄 License

This project is licensed under the MIT License.

---

## 👤 Author

Made by [Mir](https://github.com/miirekhaas) — aspiring AI engineer exploring applied machine learning with real-world datasets.

---
