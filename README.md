# 🏥 AI-Powered Disease Predictor Web App

<div align="center">
  <img src="static/img.png" alt="App Logo" width="160"/>
</div>

---

## 🚀 Overview

Welcome to the **AI-Powered Symptom-Based Disease Predictor** – your intelligent healthcare assistant that predicts possible diseases based on symptoms you provide.  
Leverage the power of **Machine Learning** (SVC Model) and get enriched medical suggestions instantly!

> ⚠️ **Note:**  
> This project is for **educational and informational** use—a real healthcare model needs much more data and medical validation!  
> Help us improve: contribute large, diverse datasets for real-world use.

---

## 💫 Why Use This App?

- **Instant Disease Prediction** from your symptoms
- **Description, Precautions, Medications, Diet, and Workout** info, all in one place
- **Speech recognition** for hands-free input
- **Beautiful, Responsive Interface** built with Bootstrap

---

## 🧠 Features

- **💡 Smart Disease Prediction**  
  Use a trained Support Vector Classifier (SVC) to predict likely diseases.

- **📝 Comprehensive Medical Info**  
  - Description (quick explanation)
  - Precautions (preventive steps)
  - Medications (possible drugs)
  - Diet (food to eat)
  - Workouts (healthy exercises)

- **🎤 Smart Input Handling**
  - Normalizes symptoms (spaces, hyphens, case, punctuation)
  - Speech-to-Text supported

- **✨ Modern and Responsive UI**
  - Built with Flask, Jinja, HTML5, Bootstrap 5

---

## 📂 Project Structure

```
├── main.py
├── Model/
│   └── svc.pkl
├── Data/
│   ├── symptoms_df.csv
│   ├── precautions_df.csv
│   ├── workout_df.csv
│   ├── description.csv
│   ├── medications.csv
│   └── diets.csv
├── templates/
│   ├── index.html
│   ├── about.html
│   ├── contact.html
│   ├── developer.html
│   └── blog.html
└── static/
    └── img.png
```

---

## ⚙️ Technologies Used

| Backend             | Frontend              | Machine Learning  | Data Handling       | Speech Input                  |
|---------------------|----------------------|-------------------|---------------------|-------------------------------|
| Flask               | HTML, Bootstrap      | scikit-learn SVC  | Pandas, NumPy       | webkitSpeechRecognition()     |

---

## 🛠 Installation & Setup

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/medical-disease-predictor.git
   cd medical-disease-predictor
   ```

2. **Install Dependencies**
   ```bash
   pip install flask pandas numpy scikit-learn
   ```

3. **Place Model & Data Files**
   - Put `svc.pkl` in the `Model/` folder
   - All CSVs go in the `Data/` folder

4. **Run the App**
   ```bash
   python main.py
   ```
   **App will be live at:** [http://127.0.0.1:5000/](http://127.0.0.1:5000/)

---

## 🔍 How Prediction Works

1. **Input:** You type symptoms (e.g., _itching, headache, nausea_) or use voice
2. **Normalization:** App auto-formats symptoms, checks for errors
3. **Vectorization:** Input vectorized for ML model (122 symptoms features)
4. **Prediction:** SVC Model predicts possible disease
5. **Response:** App returns description, precautions, medicines, diet, workouts

---

## 🌟 Screenshots

| Home Page | Main Prediction Page |
|-----------|---------------------|
| ![Home](https://github.com/user-attachments/assets/d0c19a3d-cc2e-4033-ab38-9167974aec5b) | ![Prediction](https://github.com/user-attachments/assets/2b875512-99de-44ec-b030-54372c8501f3) |

| **Disease**                                                                                                   | **Description**                                                                                                | **Precautions**                                                                                                 |
|--------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| ![Disease](https://github.com/user-attachments/assets/cf07a823-8626-43aa-8bdf-2f94d3fcf576)                  | ![Description](https://github.com/user-attachments/assets/1b4f83ce-b6a2-4297-aa1a-312a8bdd8324)               | ![Precautions](https://github.com/user-attachments/assets/4ea5a115-bda8-4c94-8471-709cedcc80fd)               |

| **Medications**                                                                                              | **Workouts**                                                                                                   | **Diets**                                                                                                      |
|--------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|
| ![Medications](https://github.com/user-attachments/assets/b5ce98ec-11f0-432c-8315-bb7e699e621e)              | ![Workouts](https://github.com/user-attachments/assets/2210e44d-e670-4fd5-92a8-1a5ea645cc2e)                  | ![Diets](https://github.com/user-attachments/assets/19e02469-dd58-4d1e-9c28-536b1b54823d)                     |
## 👨‍💻 About the Developer

**Sumit Kumar**  
_AI & ML Engineering Student | Healthcare AI Enthusiast_

- 📧 [sumitrajkumar2003@gmail.com](mailto:sumitrajkumar2003@gmail.com)
- 📍 Bhubaneswar, Odisha, India

---

## 📜 License

This project is licensed under the **MIT License**.

---

## 🌈 Special Notes

- This is **not a substitute for real medical advice or diagnosis.**
- For actual health concerns, **always consult a licensed doctor.**
- Contributions to improve dataset and accuracy are **highly welcome!**

---

<div align="center">
  <strong>
    ❤️ If you found this useful, please ⭐ star the repository and share your feedback. Collaborators & contributors always welcome!
  </strong>
</div>
