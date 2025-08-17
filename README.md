
# 🩺 Diabetes Prediction App

This project integrates **Machine Learning** and **Web Development** to provide a user-friendly interface for diabetes prediction.  
The application is built with **Flask** (for the web interface) and a **KNN model** (for prediction).  

---

## 📊 Dataset
- **Source:** Pima Indians Diabetes Database (National Institute of Diabetes and Digestive and Kidney Diseases).  
- **Objective:** Predict whether a patient has diabetes based on diagnostic measurements.  
- **Details:**
  - Patients: Females ≥ 21 years old of Pima Indian heritage.  
  - **Features:** Pregnancies, Glucose, Blood Pressure, Skin Thickness, Insulin, BMI, Diabetes Pedigree Function, Age.  
  - **Target:** `Outcome` (0 → Non-diabetic, 1 → Diabetic).  

---

## ⚙️ Tech Stack
- **Python Libraries:** NumPy, Pandas, Matplotlib, Seaborn, Scikit-learn, Pickle  
- **Backend:** Flask  
- **Frontend:** HTML, CSS  

---

## 🚀 Features
- Data preprocessing & visualization (heatmaps, correlation analysis).  
- Trains a **K-Nearest Neighbors (KNN)** classifier.  
- Saves trained model and scaler (`classifier.pkl`, `sc.pkl`) using Pickle.  
- Web interface for user input & predictions.  
- Displays result dynamically (Diabetic / Non-diabetic).  

---

## 📂 Project Structure
```
├── diabetes.csv             # Dataset
├── model_training.py        # Data preprocessing & model training
├── app.py                   # Flask web application
├── classifier.pkl           # Saved ML model
├── sc.pkl                   # Saved StandardScaler
├── templates/
│   ├── index.html           # Input form page
│   └── result.html          # Prediction result page
└── static/                  # (Optional: add custom CSS/JS)
```

---

## 🔑 Workflow
1. **Data Preprocessing**
   - Handle missing values  
   - Feature scaling using `StandardScaler`  
   - Train-test split  

2. **Model Training**
   - Classifier: **KNN (k=25, metric = 'minkowski')**  
   - Evaluate with confusion matrix & accuracy score  

3. **Flask App**
   - `/` → Input form (index.html)  
   - `/predict` → Processes input & shows result  

---

## ▶️ Run Locally
1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/diabetes-prediction.git
   cd diabetes-prediction
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run Flask app:
   ```bash
   python app.py
   ```
4. Open in browser:
   ```
   http://127.0.0.1:5000/
   ```

---

## 📸 Screenshots
- **Home Page (index.html)** – User inputs medical details.  
- **Result Page (result.html)** – Displays prediction (Diabetic / Non-diabetic).  

---

## 📌 About
This project demonstrates the integration of **machine learning models with web applications** using Flask.  
It helps in early detection of diabetes based on medical parameters and provides a simple, interactive prediction tool.
