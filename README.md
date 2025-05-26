# DR-TB Prediction App

A Streamlit-based web application for predicting drug-resistant tuberculosis (DR-TB), specifically Rifampicin resistance, powered by a pre-trained RandomForest pipeline. Clinicians and researchers can securely log in, enter patient details and laboratory results, view a clear positive/negative prediction, and generate a professional PDF report.

## 🚀 Features

- **User Authentication**  
  Simple username/password login gate to protect patient data.

- **Interactive Input Form**  
  - Demographics: Age, Gender  
  - Vital Signs: Heart Rate, Respiratory Rate, Weight  
  - Lab Results: Sputum Culture, AFB Microscopy  
  - Clinical History: Prior TB history, Fever, Weight loss, HIV status & CD4 count  

- **Machine Learning Prediction**  
  - Loads a `model_rf_pipeline.pkl` (RandomForest pipeline)  
  - Binarizes inputs and outputs a clear 🟥 Positive / 🟩 Negative prediction

- **Results Dashboard**  
  - Displays prediction message and all input parameters  
  - Highlights low CD4 count if HIV-positive

- **PDF Report Generation**  
  - “ResistX TB Report” with timestamp, patient details, and prediction  
  - Downloadable directly from the results page

## 🛠️ Technologies

- **Streamlit** for rapid UI development  
- **scikit-learn** (RandomForest) for ML inference  
- **pandas** for data handling  
- **ReportLab** for dynamic PDF creation  
- **Python 3.8+**

## 📥 Getting Started

1. **Clone the repo**  
   ```bash
   git clone https://github.com/youruser/drtb-prediction-app.git
   cd drtb-prediction-app
