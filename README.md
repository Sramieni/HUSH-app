# HUSH – Stress Monitoring & Mental Wellness App

HUSH is a mobile wellness app designed to help users understand and manage their mental and physical well-being. It combines real-time data from Fitbit with daily mood tracking and AI-generated calming suggestions. Built using Flutter and AWS serverless architecture, HUSH offers a seamless and supportive experience for stress awareness and self-reflection.

## 🌟 Features

- 🧠 **Daily Mood & Stress Check-In**  
  Users log their mood, energy, stress level, symptoms, and notes via an intuitive daily form.

- 📊 **Cross-Reference Analysis**  
  Visual comparison between self-reported stress and Fitbit-derived stress levels for deeper insight.

- 🧘 **Guided Breathing Exercises**  
  Animated breathing tool to help users pause and de-stress.

- 🤖 **AI-Powered Suggestions**  
  Personalized calming recommendations using Hugging Face NLP models.

- 💓 **Fitbit Integration**  
  Syncs heart rate, stress data, sleep, calories, and more using Fitbit’s API.

- 🔐 **Secure Authentication**  
  Sign-up and sign-in handled through AWS Lambda and DynamoDB with session persistence.

---

## 🛠️ Tech Stack

### Frontend
- **Flutter & Dart** – Clean UI, smooth navigation, and responsive experience
- **SharedPreferences** – For session persistence and auto-login

### Backend (Serverless)
- **AWS Lambda** – Backend logic for login, check-ins, and Fitbit data handling
- **API Gateway** – Exposing secure endpoints to the app
- **DynamoDB** – NoSQL database for storing users, check-ins, and heart data

### Third-Party APIs
- **Fitbit Web API** – For retrieving heart rate and stress metrics
- **Hugging Face Inference API** – AI model for personalized de-stress advice

---

## 📈 Architecture Overview

- User signs in or signs up → data sent to AWS Lambda via API Gateway  
- Daily check-ins stored in DynamoDB with timestamp indexing  
- Fitbit data fetched using OAuth tokens and stored for trend analysis  
- AI suggestions triggered via POST request to Hugging Face model  
- All endpoints tested and debugged using Postman

---

## 👩‍💻 Team Contributions

| Name | Role | Responsibilities |
|------|------|------------------|
| **Sesha Sai Ramineni** | Backend & UI | Developed AWS Lambda functions, API integration, Flutter UI, and report |
| **Kavya Sri Pachchava** | UI & AI Module | Built cross-reference screen, Hugging Face integration, and API flows |
| **Rashmitha Eri** | Fitbit & Daily Check-In | Designed check-in form, Fitbit integration, and backend storage logic |

---

## 🧪 Testing & Debugging

- All APIs tested with **Postman**
- Handled edge cases: malformed JSON, missing fields, token expiration
- Real-time error messages for better debugging and smoother UX

---

## 🚀 Future Improvements

- Real-time notifications and reminders  
- Community support forums  
- Deeper analysis of stress patterns over time  
- Sleep and recovery insights from Fitbit

---

## 📸 Screenshots (Coming Soon)
- Dashboard UI  
- Mood Check-in  
- AI Insight Screen  
- Fitbit Data Cards

---

## 📬 Contact

For any questions or collaboration requests, feel free to connect with us on [LinkedIn](https://www.linkedin.com/in/sesha-sai-ramineni/) or raise an issue in this repo!

---

