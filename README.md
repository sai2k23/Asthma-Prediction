# 🏥 Asthma Severity Prediction - Full Stack Project

This repository contains the complete **Asthma Severity Prediction** system, integrating **Node.js and Flask backends** with a **React frontend** for a seamless user experience. This project is designed to predict the severity of asthma using machine learning models, providing insights to healthcare professionals and patients.

## 🚀 Live Preview
[![Live Demo](https://img.shields.io/badge/Live%20Demo-Click%20Here-brightgreen)]([https://your-live-demo-link.com](https://asthmaseverityprediction.netlify.app/))

---

## 📌 Project Structure
```
Asthma-Prediction/
│── backend/
│   │── node-backend/  (Node.js API)
│   │── flask-backend/  (Flask API with ML Model)
│── frontend/          (React-based UI)
│── README.md
```

---

## 🚀 Tech Stack Used

### 📌 Backend:
- 🔹 **Node.js (Express.js)** - REST API development
- 🔹 **Flask (Python)** - Machine Learning Model Integration
- 🔹 **MongoDB** - Database for storing patient data & predictions
- 🔹 **Mongoose** - ODM for MongoDB
- 🔹 **TensorFlow/Keras** - Machine learning model for severity prediction
- 🔹 **Scikit-learn** - Data preprocessing and model training
- 🔹 **Razorpay** - Payment gateway for premium AI-assisted reports
- 🔹 **JWT Authentication** - Secure user authentication

### 🎨 Frontend:
- 🔹 **React.js** - Modern UI development
- 🔹 **Redux** - State management
- 🔹 **Tailwind CSS** - Responsive styling
- 🔹 **Chart.js/Recharts** - Data visualization for reports

---

## ✨ Key Features
✅ **User Authentication** - Secure login with JWT  
✅ **Asthma Severity Prediction** - Uses a trained ML model to predict asthma severity  
✅ **Dual Backend Architecture** -
   - **Node.js** for user management, payments, and database operations
   - **Flask** for running the ML model
✅ **Data Visualization** - Graphical representation of patient history  
✅ **Payment Gateway** - Razorpay integration for premium reports  
✅ **Downloadable Reports** - Generate PDFs with prediction results  
✅ **Real-time Notifications** - Alerts for high-risk asthma severity  

---

## 📜 Installation Guide

### 🔹 Clone the Repository
```bash
git clone https://github.com/your-username/Asthma-Prediction.git
cd Asthma-Prediction
```

### 🔹 Backend Setup

#### **Node.js API**
```bash
cd backend/node-backend
npm install
npm start
```

#### **Flask API**
```bash
cd backend/flask-backend
pip install -r requirements.txt
python app.py
```

### 🔹 Frontend Setup
```bash
cd frontend
npm install
npm start
```

---

## 🔐 GitHub Push Protection Issue (Secrets Detection)

If you encounter a **GitHub push protection error** due to secrets (e.g., Twilio API keys), follow these steps:

### **Option 1: Approve the Push via GitHub**
1. GitHub provides a way to **unblock the secret manually**.
2. Look at the error message in your terminal; it will contain a **GitHub Unblock URL**.
3. Open the URL in your browser and **click "Allow Push"** to bypass the protection.

> ⚠️ **Warning:** This will expose your API keys publicly. It's recommended to remove secrets before pushing.

### **Option 2: Remove Secrets from Commit History**

1. Remove the `.env` file from Git tracking:
   ```bash
   git rm --cached backend/node-backend/.env
   ```
2. Add `.env` to `.gitignore`:
   ```bash
echo "backend/node-backend/.env" >> .gitignore
   ```
3. Reset the last commit and push again:
   ```bash
   git commit --amend --no-edit
   git push origin main --force
   ```

### **Option 3: Temporarily Disable GitHub Secret Scanning**

1. Go to **GitHub Repository Settings** → **Security** → **Secret Scanning**.
2. Disable **Push Protection**.
3. Push your code:
   ```bash
   git push origin main
   ```
4. **Re-enable Secret Scanning** after the push.

---

## 📞 Support & Contact
For any issues, feel free to open an **Issue** or contact me at **your-email@example.com**.

---

**⭐ If you found this project helpful, please consider giving it a star!** 🌟

