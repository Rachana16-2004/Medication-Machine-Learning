# 💊 Machine Learning Medication App

This project is a smart healthcare web/mobile application that uses **Machine Learning** to predict possible diseases based on user-inputted **symptoms**, and recommends relevant **medications**.This is a smart healthcare web application that uses a Machine Learning model to predict the most probable disease based on user-inputted symptoms and provides relevant healthcare suggestions including medications, diets, and precautions.
  
## 🌟 Features
 
- 🤒 Input symptoms through a simple text form (comma-separated)
- 🧬 Predict diseases using a pre-trained Support Vector Classifier (SVC) 
- 💊 Suggest medications, diets, and workout plans
- 🔐 Built-in support for multiple datasets including symptom severity and disease descriptions
- 👨‍⚕️ Future enhancement: contact a doctor or consult a chatbot
- 📊 Easy-to-understand results on the same web page 

## 🗂 Project Directory Structure

project-root/
│
├── app.py / main.p # Flask app entry point (use the correct one)
├── README.md # This file
├── Untitled.ipynb # Development Notebook
├── Untitled-checkpoint.ipynb # Auto-saved Jupyter Notebook
│
├── datasets/ # Dataset files
│ ├── Symptom-severity.csv
│ ├── Training.csv
│ ├── description.csv
│ ├── diets.csv
│ ├── medications.csv
│ ├── precautions_df.csv
│ ├── symtoms_df.csv
│ └── workout_df.csv
│
├── models/ # Trained ML model
│ └── svc.pkl
│
├── static/ # Static images or resources
│ ├── a.png
│ └── img.png
│
├── templates/ # HTML templates
│ ├── index.html
│ ├── about.html
│ ├── contact.html
│ ├── blog.html
│ └── developer.html
│
└── ipynb_checkpoints/ # Jupyter notebook autosaves

## ⚙️ Installation & Setup

### ✅ Requirements

Make sure Python 3.7+ is installed. You can install dependencies using:
pip install flask pandas numpy scikit-learn
🚀 Run the App

# If using app.py
python app.py
### The app:
Converts symptoms to a binary feature vector using symptoms_dict
Uses the pre-trained SVC model (svc.pkl) to predict the disease
Relevant information is retrieved:
Description from description.csv
Precautions from precautions_df.csv
Medications from medications.csv
Diet from diets.csv
Workouts from workout_df.csv
Output is displayed on the same page.

🔮 **Example Input**
Symptoms: fatigue, headache, vomiting
Predicted Disease: Migraine
Suggestions:

Description: A headache of varying intensity, often accompanied by nausea and sensitivity to light and sound.
Precautions: Avoid triggers, take rest, stay hydrated, use cold compress.
Medications: Ibuprofen, Sumatriptan
Diet: Avoid caffeine, eat at regular intervals
Workout: Light yoga/stretching
📸 Screenshots
(Optional: Add screenshots of your UI here)

**📈 Future Improvements**
Add chatbot or teleconsultation feature
Add confidence score from the model
Mobile app integration using REST API
Dynamic symptom suggestions using autocomplete
Improve UI/UX with animations or design libraries

### Application Interface Preview:
![My Logo](https://github.com/Rachana16-2004/Medication-Machine-Learning/blob/main/Screenshot%202025-07-11%20183757.png?raw=true)

![My Logo](https://github.com/Rachana16-2004/Medication-Machine-Learning/blob/main/Screenshot%202025-07-10%20132943.png?raw=true)
