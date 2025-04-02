# 🏥 Asthma Severity Prediction - Full Stack Project

This repository contains the complete **Asthma Severity Prediction** system, combining **Node.js** and **Flask** backends with a **React frontend** for a seamless user experience. The project predicts asthma severity using machine learning models, providing valuable insights for healthcare professionals and patients.

🔗 **Live Preview**: [Asthma Severity Prediction](https://asthmaseverityprediction.netlify.app/)

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
- **Node.js (Express.js)** - REST API development
- **Flask (Python)** - Machine Learning Model Integration
- **TensorFlow/Keras** - Machine learning model for severity prediction
- **Scikit-learn** - Data preprocessing and model training
- **Twilio** - SMS OTP verification for authentication
- **JWT Authentication** - Secure user authentication

### 🎨 Frontend:
- **React.js** - Modern UI development
- **Redux** - State management
- **Tailwind CSS** - Responsive styling
- **Chart.js/Recharts** - Data visualization for reports

---

## ✨ Key Features

✅ **User Authentication** - Secure login with JWT & OTP verification (Twilio)  
✅ **Asthma Severity Prediction** - Uses a trained ML model to predict severity  
✅ **Dual Backend Architecture:**  
   - Node.js for user management, payments, and database operations  
   - Flask for running the ML model  
✅ **Data Visualization** - Graphical representation of patient history  
✅ **Real-time Notifications** - Alerts for high-risk asthma severity  

---

## 📜 Installation Guide

### Clone the Repository
```bash
git clone https://github.com/your-username/Asthma-Prediction.git
cd Asthma-Prediction
```

### Backend Setup

#### Node.js API
```bash
cd backend/node-backend
npm install
npm start
```

#### Flask API
```bash
cd backend/flask-backend
pip install -r requirements.txt
python app.py
```

### Frontend Setup
```bash
cd frontend
npm install
npm start
```

---

## 🔐 Setting Up Twilio for OTP Verification

Twilio is used to send **OTP verification** messages for user authentication. To set up Twilio:

### 📌 Steps to Create a Twilio Account:
1. Go to [Twilio Signup Page](https://www.twilio.com/try-twilio)
2. Create an account and verify your email and phone number.
3. Navigate to the **Twilio Console**.
4. Copy the following details from the console:
   - **Account SID**
   - **Auth Token**
   - **Verify Service SID** (for OTP verification)
   - **Twilio Phone Number** (assigned to your account)

### 📌 Add the Credentials to the `.env` File
Create a `.env` file inside `backend/node-backend/` and add:

```
TWILIO_VERIFY_SID=your_verify_service_sid_here
TWILIO_ACCOUNT_SID=your_account_sid_here
TWILIO_AUTH_TOKEN=your_auth_token_here
TWILIO_PHONE_NUMBER=your_twilio_phone_number_here
```

> **Warning:** Never push your `.env` file to GitHub! Always add it to `.gitignore`.

---

## 🔐 GitHub Push Protection Issue (Secrets Detection)

If you encounter a **GitHub push protection error** due to secrets (e.g., Twilio API keys), follow these steps:

### Option 1: Approve the Push via GitHub

GitHub provides a way to unblock the secret manually.

1. Look at the error message in your terminal; it will contain a **GitHub Unblock URL**.
2. Open the URL in your browser and click **"Allow Push"** to bypass the protection.

⚠️ **Warning:** This will expose your API keys publicly. **It’s recommended to remove secrets before pushing.**

### Option 2: Remove Secrets from Commit History

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

### Option 3: Temporarily Disable GitHub Secret Scanning

1. Go to **GitHub Repository Settings → Security → Secret Scanning**.
2. Disable **Push Protection**.
3. Push your code:
```bash
git push origin main
```
4. **Re-enable Secret Scanning after the push**.

---

## 🌟 Additional Features & Future Enhancements

🔹 **Upcoming Features:**
- 🌍 **Multi-language Support** for wider accessibility.
- 📊 **Advanced Analytics** for asthma trends and severity insights.
- 📱 **Mobile App Integration** for Android & iOS.
- 🏥 **Integration with Electronic Health Records (EHR)**.
- 🔔 **AI-Based Personalized Alerts** for early intervention.

🔹 **Future Enhancements:**
- 🔍 **AI-powered Recommendations** for better asthma management.
- 💬 **Chatbot Support** for instant health guidance.
- 🛡️ **HIPAA Compliance** for enhanced data security.

---

## 🔗 Live Preview

🚀 Click below to view the **Live Preview** of the Asthma Severity Prediction System:

[![Live Preview](https://img.shields.io/badge/Live-Preview-blue?style=for-the-badge)](https://asthmaseverityprediction.netlify.app/)

---

## 📌 Contributing

Contributions are welcome! Follow these steps:
1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Submit a Pull Request.

---

## 📜 License

This project is **open-source** and available under the **MIT License**.

---

🚀 **Happy Coding!** 😃

