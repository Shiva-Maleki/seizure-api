# 🧠 Seizure Prediction API

A simple machine learning API that predicts seizures from EEG-like data using a RandomForestClassifier. Built with Flask.

## 🔧 Features
- Predict seizure (1) or no seizure (0) from 3 EEG features
- Built-in Flask REST API
- Easy to test with curl or Postman

## 🚀 How to Use

1. Clone the repo:
```bash
git clone https://github.com/yourusername/seizure-api.git
cd seizure-api
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the server:
```bash
python serve_model.py
```

4. Test it:
```bash
curl -X POST http://127.0.0.1:5000/predict -H "Content-Type: application/json" -d "{"mean_bandpower": 6.5, "spike_count": 3, "frequency_variation": 1.2}"
```

## 📂 Files
- `serve_model.py` – Flask server code
- `seizure_model.pkl` – Pretrained model
- `requirements.txt` – Dependencies
