# HW2 — Spam Classification & Language ID

**Name:** Anvith Vobbilisetty  
**SID:** 1988935

## What’s Included
- **`main.ipynb`** — single notebook that trains & evaluates all models.
- **`spambase.data`** — UCI Spambase dataset (loaded in the notebook).
- *(Language ID only)* Text files:
  - `english.txt`, `dutch.txt`
  - `developmenteng.txt`, `developmentdutch.txt`
  - `test_en.txt`, `test_du.txt`

## Notebook Contents
### 1) Spambase (Spam vs. Ham)
- **1.1** Linear SVM  
- **1.2** Logistic Regression  
- **1.3** Custom Perceptron (from scratch)

Outputs: accuracy + readable (normalized/annotated) confusion matrices.

### 2) Language Identification (Dutch vs. English)
- **2.1** All three models (Linear SVM, Logistic Regression, Custom Perceptron) on line-level sentences using **TF-IDF character n-grams**.

## How to Run
1. Open **`main.ipynb`**.
2. Ensure dataset paths are correct (see **Data Paths** below).
3. **Kernel → Restart & Run All.**  
   The notebook handles vectorization, training, and evaluation end-to-end.

## Data Paths (Edit if Needed)
Update these variables near the top of the Language ID section if your files live elsewhere:
- `EN_PATH`, `DU_PATH` — training files  
- `dev_en_PATH`, `dev_du_PATH` — development files  
- `test_EN_PATH`, `test_DU_PATH` — test files

`spambase.data` is read from the project folder; update its path in the notebook if moved.

## Requirements
- Python 3.9+
- Libraries:
  - `numpy`, `pandas`
  - `scikit-learn`
  - `matplotlib`

Install (if needed):
```bash
pip install numpy pandas scikit-learn matplotlib