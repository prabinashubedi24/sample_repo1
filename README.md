# 🧠 Cyber Safety Detection System (Grooming & Bullying)

This project develops an AI-based cyber safety detection system that classifies text messages as **Normal**, **Grooming**, or **Bullying**. It uses a combination of classical machine learning (TF-IDF + Logistic Regression) and a fine-tuned **DistilBERT** transformer model for high-accuracy text classification.

---

## 🚀 Features

- Text preprocessing and cleaning  
- Feature engineering (length, punctuation, numerics, uppercase patterns)  
- Exploratory Data Analysis (EDA)  
- Handling class imbalance using SMOTE and Random Under-Sampling  
- Baseline ML model using TF-IDF + Logistic Regression  
- Fine-tuned DistilBERT models for grooming and bullying datasets  
- Unified prediction combining both models  
- **Streamlit web app** for real-time message classification  
- Visualizations: confusion matrices, performance comparison charts  

---

## 📊 Model Performance

| Task | Model | Accuracy |
|------|--------|----------|
| Grooming Detection | DistilBERT | **98.82%** |
| Bullying Detection | DistilBERT | **82.68%** |

DistilBERT significantly outperforms classical machine learning baselines.

---

## 📁 Project Structure

```
CyberSafety-Detection/
│
├── cyber_final.py
├── app.py
├── requirements.txt
├── README.md
│
├── data/
│   ├── grooming_train_sample.csv
│   ├── grooming_test_sample.csv
│   └── bullying_sample.csv
│
├── models/  (optional)
│   ├── grooming_model_distilbert/
│   └── bullying_model_distilbert/
│
└── outputs/
    ├── cm_grooming.png
    ├── cm_bullying.png
    └── metrics_comparison.png
```

---

## ▶️ How to Run

### **1. Install dependencies**
```
pip install -r requirements.txt
```

### **2. Run the main script**
```
python cyber_final.py
```

### **3. Run the Streamlit app**
```
streamlit run app.py
```

---

## 🌐 Streamlit App

The app provides a simple UI where users can input a message and receive a prediction showing whether it contains grooming, bullying, or normal content.

---

## 🙌 Author

**Prabina Subedi**

---

## 📌 Notes

- Only sample datasets are included for privacy reasons.  
- Full models may not be uploaded due to size limits; links can be provided if needed.

---

## 📜 License

MIT License 
