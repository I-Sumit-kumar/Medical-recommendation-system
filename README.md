🏥 AI-Powered Symptom-Based Disease Prediction Web App

A Flask-based healthcare assistant that predicts diseases from user symptoms, using Machine Learning and a rich medical recommendation system.

<img src="static/img.png" alt="App Logo" width="160"/>

🚀 Project Overview

This project is an intelligent AI-driven healthcare web application that predicts possible diseases based on user symptoms.
It integrates:

✔ Machine Learning (SVC Model)

✔ Symptom → Disease Prediction

✔ Disease Description

✔ Precautions

✔ Medications

✔ Diet Recommendations

✔ Workouts

✔ Speech-to-text symptoms input

✔ Complete Frontend using HTML, Bootstrap, and Flask Jinja templates

This system helps users quickly understand their potential health issues and take informed early steps.

⚠ Not a medical diagnosis tool — it is for educational & informational purposes only.

🧠 Features
🔹 Disease Prediction

Predicts disease using a trained Support Vector Classifier (SVC) model.

Accepts comma-separated symptom input.

If symptoms are not recognized, the system flags them politely.

🔹 Full Medical Information

For each predicted disease, the app provides:

Information Type	Description
📝 Description	Short medical explanation
🛡️ Precautions	Preventive measures
💊 Medications	General medicines
🍎 Diet	Recommended foods
🏋️ Workouts	Suggested exercises
🔹 Smart Input Handling

Symptom normalization (handles spaces, hyphens, case sensitivity, punctuation).

Speech-to-Text input using browser speech recognition.

🔹 Clean UI with Bootstrap

Pages included:

Home

About

Contact

Developer

Blog

📂 Project Structure
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

⚙️ Technologies Used
Category	Tools
Backend	Flask
Frontend	HTML, CSS, Bootstrap
Machine Learning	Scikit-Learn
Data Handling	Pandas, NumPy
Model	SVC Classifier
Speech Recognition	webkitSpeechRecognition()
🛠 Installation & Setup
1. Clone the Repository
git clone https://github.com/yourusername/medical-disease-predictor.git
cd medical-disease-predictor

2. Install Dependencies
pip install flask pandas numpy scikit-learn

3. Ensure Model & Data Files Exist

Place:

svc.pkl inside Model/

all CSV files inside Data/

4. Run the App
python main.py


App runs at:

http://127.0.0.1:5000/

🔍 How the Prediction Works

User enters symptoms (e.g., itching, headache, nausea)

Symptoms are normalized (lowercased, cleaned, converted to keys).

A 122-dimensional symptom vector is constructed.

SVC model predicts a disease index.

The disease index maps to actual disease name.

Additional datasets provide:

description

diet

medications

workouts

precautions

📸 Screenshots:-
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/5e5ce71e-41d1-4ef7-a957-52e3ab64618f" />


After cleacking Disease:
<img width="1857" height="967" alt="image" src="https://github.com/user-attachments/assets/e0115868-66f8-41f1-a01e-dd2a7e30c9b0" />


After cleacking Description:
<img width="1854" height="974" alt="image" src="https://github.com/user-attachments/assets/cc58b103-0514-4a17-b244-53bfd0dbd274" />


After cleacking Precaution:
<img width="1854" height="965" alt="image" src="https://github.com/user-attachments/assets/a71a0491-3425-4fa2-bb03-f3e342c72a21" />


After cleacking Medications:
<img width="1854" height="966" alt="image" src="https://github.com/user-attachments/assets/15794263-bfe4-4de9-be69-4bb30f14d75c" />


After cleacking Workouts:
<img width="1856" height="966" alt="image" src="https://github.com/user-attachments/assets/e3e4502f-34e3-40fe-9c4e-b9514677802f" />


After cleacking Diets:
<img width="1855" height="966" alt="image" src="https://github.com/user-attachments/assets/4be91a28-7144-40e9-b82e-70647a7c2ab9" />


👨‍💻 Developer

Junaid Khan — AI & ML Engineer
Passionate about healthcare AI & developing impactful solutions.

📞 Contact

Email: junaidmehsuud035@gmail.com

Phone: 03477155035
Location: Dera Ismail Khan, KPK, Pakistan

📜 License

This project is licensed under the MIT License.

⭐ Special Notes

This app is an educational machine-learning demo.

Not intended to replace medical professionals.

Always consult a doctor for real medical concerns.
