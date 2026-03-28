# FYP-II: Anomaly Detection Dashboard

## Project Overview
- Detect anomalies using Autoencoder, PCA+Autoencoder, and LSTM Autoencoder
- Compare models using Accuracy, Precision, Recall, F1-score, ROC-AUC
- Best model saved for deployment

## How to Run
1. Clone repository
2. Install dependencies:
   pip install -r requirements.txt
3. Open `section_A_to_G.ipynb` in Colab/Jupyter
4. Run sections A–G to reproduce experiments
5. Load best model:
   ```python
   from tensorflow.keras.models import load_model
   import joblib

   best_model = load_model("best_model_ae_no_pca.h5")
   scaler = joblib.load("scaler_exp.save")
   
---

## **Step 6: Create GitHub Repository**

1. Go to GitHub → Click **New Repository**  
2. Name: `FYP-II-Anomaly-Detection`  
3. Description: `Anomaly detection FYP-II project with Autoencoder, PCA and LSTM models`  
4. **Public / Private** select karo (public recommended for demo)  
5. Initialize repository **without README** (hum local README push karenge)  
6. Click **Create repository**

---

## **Step 7: Upload Your Project**

### Option A — Using Git (Local PC)

1. Open terminal inside project folder:
```bash
git init
git add .
git commit -m "Initial FYP-II project commit"
git branch -M main
git remote add origin https://github.com/<username>/FYP-II-Anomaly-Detection.git
git push -u origin main