# 🌾 Smart Irrigation System using Machine Learning

A multi-stage machine learning project to build a smart irrigation system using environmental sensor data to predict the irrigation needs of different land parcels.

---

## 📋 Table of Contents
- [📌 Project Overview](#-project-overview)
- [📅 Week-wise Work Summary](#-week-wise-work-summary)
  - [✅ Week 1: Data Preprocessing and Random Forest Modeling](#week-1-data-preprocessing-and-random-forest-modeling)
  - [✅ Week 2: Model Evaluation and Visualization](#week-2-model-evaluation-and-visualization)
  - [✅ Week 3: Interactive App in Google Colab](#week-3-Interactive-App-in-Google-Colab)
  - [🔜 Future Work](#-future-work)
- [🧠 Why Random Forest?](#-why-random-forest)
- [🖼️ Sample Outputs](#-sample-outputs)
- [📂 Colab Link](#-colab-link)
- [🙏 Acknowledgement](#-acknowledgement)

---

## 📌 Project Overview

This project aims to assist farmers in automating irrigation decisions using sensor data. By analyzing real-time sensor inputs, the model predicts whether three separate land parcels need irrigation.

---

## 📅 Week-wise Work Summary

### ✅ Week 1: Data Preprocessing and Random Forest Modeling
- Imported and cleaned the dataset (`irrigation_machine.csv`)
- Removed unnecessary columns and handled basic EDA
- Split data into **features** (`sensor_0` to `sensor_19`) and **targets** (`parcel_0`, `parcel_1`, `parcel_2`)
- Normalized data using `MinMaxScaler`
- Trained a **MultiOutput Random Forest Classifier**
- Saved the trained model and scaler for future inference

### ✅ Week 2: Model Evaluation and Visualization
- Evaluated the model using `classification_report` (precision, recall, F1-score)
- Visualized feature importance
- Visualized decision tree structure (shallow level)
- Explored dataset statistics and distribution
- Gained insights into which sensors most affect irrigation decisions

### ✅ Week 3: Interactive App in Google Colab
- Built an interactive frontend using `ipywidgets` in Google Colab
- Created 20 sliders for scaled sensor input (range 0 to 1)
- Loaded the trained Random Forest model (`Farm_Irrigation_System.pkl`)
- Displayed prediction results for each parcel as ON/OFF
- Designed the interface for intuitive user control and testing

### 🔜 Future Work
- Integrate with **real-time IoT sensors**
- Add **time-series analysis** using LSTM or other temporal models
- Build a web dashboard or embedded interface for end-users
- Deploy model on microcontrollers (e.g., Raspberry Pi or Arduino with ML support)

---

## 🧠 Why Random Forest?

- Handles **non-linear interactions** between sensor inputs
- Supports **multi-label output** using `MultiOutputClassifier`
- **Robust to noise** and missing data
- **No heavy preprocessing** required
- Provides **feature importance insights**
- Easily tunable and scalable

---

## 🖼️ Sample Outputs

### 📊 Week 1 – Data Summary & Head

![Week 1 - Data Sample](<img width="1238" height="470" alt="Image" src="https://github.com/user-attachments/assets/af580e56-5c49-489b-9c20-f3ca095f9f9a" />)

---

### 🌳 Week 2 – Model Evaluation and Feature Importance

![Week 2 - Evaluation](<img width="1238" height="470" alt="image" src="https://github.com/user-attachments/assets/6834e572-efc0-4875-bd07-40703be1508c" />)

![Week 2 - Feature Importance](<img width="603" height="432" alt="Image" src="https://github.com/user-attachments/assets/badf10f6-0ceb-486a-b919-133b8f33ae3b" />)

![Week 2 - Model](<img width="1570" height="790" alt="Image" src="https://github.com/user-attachments/assets/a41787ab-d846-4fb1-9583-5fe8703fe542" />)

---

## 📂 Colab Link

Access and run the project in Google Colab:  
🔗 [Model Training Notebook (Week 1 & 2)](https://colab.research.google.com/drive/1i6CyUwJkXKdB2QUDS79csBs9P9zMyLM4?usp=sharing)

## 📲 Week 3 – Colab App

Run the interactive irrigation prediction app (with sliders) here:  
🔗 [Week 3 – Colab Interactive App](https://colab.research.google.com/drive/1kCgb5MZCXwlRNGajcTfaU3fHhcCWUWyN?usp=sharing)


---

## 🙏 Acknowledgement

This project was developed as part of a machine learning internship.  
Special thanks to mentors, peers, and the organizing institution for guidance and support.

---

**Author**: *Shaili Sahu*  
Final Year ECE Student, Amrita Vishwa Vidyapeetham – Bengaluru  
GitHub: [shailisahu283](https://github.com/shailisahu283)
