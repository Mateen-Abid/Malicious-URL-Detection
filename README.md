# 🔐 Malicious URL Detection using Machine Learning and Temporal Analysis

This project implements a machine learning system to detect **malicious URLs** using a hybrid approach combining **lexical**, **host-based**, and **temporal** features. It uses both traditional ML models (Random Forest, Logistic Regression, XGBoost) and a custom **Deep Neural Network** trained on TF-IDF vectors.

## 📌 Project Highlights

- ✅ Supervised machine learning approach
- ✅ Feature engineering across lexical, host-based, and simulated temporal domains
- ✅ Real-time URL classification interface (Google Colab-based)
- ✅ Visualization of model evaluation (confusion matrix, ROC-AUC, classification report)
- ✅ Built-in support for scalable retraining and future API integration (WHOIS, DNS)


## 🛠️ Technologies Used

- Python 3.x  
- Scikit-learn  
- XGBoost  
- Pandas, NumPy  
- TLDExtract  
- TF-IDF (from scikit-learn)  
- Matplotlib / Seaborn  
- Google Colab (T4 GPU support)

## 📁 Folder Structure

/project
│
├── data/
│ └── malicious_phish.csv # Labeled dataset
├── model/
│ └── trained_model.pkl # Saved ML/DNN model
├── results/
│ ├── confusion_matrix.png
│ ├── roc_curve.png
├── notebooks/
│ └── Malicious_URL_Detection.ipynb # Main Colab code
├── docs/
│ └── presentation.pptx # Slides
│ └── report.docx # Final report


## 🧠 Feature Engineering

Features are grouped into:

- **Lexical Features**:  
  - URL length  
  - Count of special characters  
  - Suspicious keywords (e.g., 'login', 'verify', 'secure')

- **Host-Based Features**:  
  - Domain age (simulated)  
  - Presence of IP addresses  
  - WHOIS-derived flags (mocked)

- **Temporal Features**:  
  - Frequency of domain appearance  
  - Simulated timestamp-based trends

- **Semantic Features**:  
  - TF-IDF n-gram vectorization of URL structure

## 🤖 Models Trained

| Model                | Notes                       |
|---------------------|-----------------------------|
| Logistic Regression | Baseline, interpretable     |
| Random Forest       | Tree-based, non-linear      |
| XGBoost             | Gradient boosting ensemble  |
| Dense Neural Net    | TF-IDF + deep learning      |


## 📊 Evaluation Metrics

- Accuracy
- Precision, Recall, F1-score
- AUC-ROC
- Confusion Matrix


## 🚀 How to Run

1. Upload the dataset to Google Colab  
2. Run the notebook step-by-step  
3. Use the **"Test a URL"** cell to classify any custom input URL in real-time  
4. Export model predictions or metrics for visualization/reporting

## 📌 Future Improvements

- Integration with live WHOIS/DNS APIs  
- Deployable web app (Flask or Django interface)  
- Real-time retraining pipeline with new data  
- SHAP or LIME explainability modules  


## 📄 License

This project is for educational and academic purposes. Feel free to fork, modify, and contribute.
