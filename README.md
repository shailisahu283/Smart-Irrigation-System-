# 🌱 Smart Irrigation System – Week 1

This project is the first step towards building an intelligent irrigation system using Machine Learning. It involves data preprocessing, feature analysis, and training a multi-output classifier to predict which parcels of land require irrigation based on sensor data.

## 📁 Project Structure

* `Irrigation_System.ipynb` – Jupyter Notebook containing the full data loading, preprocessing, training, and evaluation pipeline.
* `irrigation_machine.csv` – Dataset used, containing sensor values and parcel irrigation labels.

## 🧠 Objective

Develop a predictive model that takes in environmental sensor readings and accurately determines the irrigation needs (binary output) for three parcels of agricultural land.

## 📊 Dataset

* **Size:** 2000 rows × 23 columns
* **Inputs:** 20 sensor readings (`sensor_0` to `sensor_19`)
* **Outputs:** 3 binary labels (`parcel_0`, `parcel_1`, `parcel_2`) representing irrigation status (1 = irrigate, 0 = do not irrigate)

## 🔧 Technologies Used

* Python
* Pandas, Matplotlib, Seaborn
* Scikit-learn (RandomForest, MultiOutputClassifier)
* Joblib (for model saving)

## 🔍 Workflow Summary

1. **Data Preprocessing**

   * Removed unnecessary index column
   * Visualized distribution and correlation between features
   * Scaled data using `MinMaxScaler`
2. **Model Training**

   * Used `RandomForestClassifier` wrapped in `MultiOutputClassifier` to handle multiple labels
   * Performed train-test split (default 80-20)
3. **Evaluation**

   * Used `classification_report` to evaluate model performance on each parcel

## 📈 Results

The model outputs a separate prediction for each parcel. Each label is evaluated using precision, recall, and F1-score metrics.

## 💾 Model Export

The trained model can be saved and reloaded using `joblib`, enabling deployment for real-time inference in smart irrigation systems.

---

## 🚀 Future Scope

* Integrate real-time sensor inputs from IoT devices
* Deploy the model in embedded systems for automated irrigation
* Add temporal analysis (seasonal trends, time-series modeling)

---

## 🙋‍♀️ Author

**Shaili Sahu**
Final Year ECE Student, Amrita Vishwa Vidyapeetham – Bengaluru
🌐 GitHub: [shailisahu283](https://github.com/shailisahu283)
