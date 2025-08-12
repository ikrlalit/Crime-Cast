# CrimeCast: Forecasting Crime Categories

**CrimeCast: Forecasting Crime Categories** is a machine learning project that predicts the type of crime based on historical incident reports. By leveraging classification algorithms and time series analysis, the system identifies hidden patterns in criminal activities to aid in proactive law enforcement and crime prevention strategies.

---
## 📌 Project Overview

This project focuses on building a predictive model for **Crime Category** using real-world crime datasets. The dataset contains various features such as **location details, time of incident, victim details, crime modus operandi, and weapon information**.  

The goal is to develop a robust classification model capable of accurately predicting the crime category given these features.

---
## 📂 Dataset Description
The dataset contains the following columns:

- **Location**: Street address of the crime incident.  
- **Cross_Street**: Cross street of the rounded address.  
- **Latitude**: Latitude coordinates of the crime incident.  
- **Longitude**: Longitude coordinates of the crime incident.  
- **Date_Reported**: Date the incident was reported.  
- **Date_Occurred**: Date the incident occurred.  
- **Time_Occurred**: Time the incident occurred in 24-hour military time.  
- **Area_ID**: LAPD's Geographic Area number.  
- **Area_Name**: Name designation of the LAPD Geographic Area.  
- **Reporting_District_no**: Reporting district number.  
- **Part 1-2**: Crime classification.  
- **Modus_Operandi**: Activities associated with the suspect.  
- **Victim_Age**: Age of the victim.  
- **Victim_Sex**: Gender of the victim.  
- **Victim_Descent**: Descent code of the victim.  
- **Premise_Code**: Premise code indicating the location of the crime.  
- **Premise_Description**: Description of the premise code.  
- **Weapon_Used_Code**: Weapon code indicating the type of weapon used.  
- **Weapon_Description**: Description of the weapon code.  
- **Status**: Status of the case.  
- **Status_Description**: Description of the status code.  
- **Crime_Category**: The category of the crime (Target Variable).

---
## 🛠️ Data Preprocessing & EDA

Before building the model, the following steps were performed:

1. **Exploratory Data Analysis (EDA)**  
   - Visualizing crime trends over time.  
   - Identifying most common crime locations and time windows.  
   - Analyzing victim demographics and crime patterns.

2. **Handling Missing Values**  
   - Null values were identified and imputed where applicable.  

3. **Feature Engineering**  
   - Extracted **hour, day, month, year** from `Date_Occurred` and `Time_Occurred`.  
   - Geospatial clustering to group crime-prone areas.  
   - Encoding categorical features using **OneHotEncoder**.  
   - Scaling numerical features using **StandardScaler**.

---
## 🧰 Tools & Libraries Used

- **Python** (Data Processing & Modeling)
- **pandas** – Data manipulation & cleaning
- **numpy** – Numerical computations
- **matplotlib**, **seaborn** – Data visualization
- **scikit-learn** – Model building & evaluation
- **xgboost** – XGBClassifier
- **StandardScaler** – Feature scaling
- **OneHotEncoder** – Encoding categorical variables

---
## 🤖 Models Tried

We experimented with multiple machine learning algorithms to identify the best-performing model:

- **Logistic Regression**
- **Random Forest Classifier**
- **Support Vector Machine (SVM)**
- **XGBClassifier**
- **Multi-Layer Perceptron (MLP)**
- **K-Nearest Neighbors (KNN)**

---
## 📊 Model Evaluation

For each model, a **detailed classification report** was generated, containing:

- **Precision**
- **Recall**
- **F1-score**
- **Support**
- **Accuracy**
- **Macro Avg**
- **Weighted Avg**

The results allowed us to compare the models based on both **accuracy** and **balanced performance across classes**.

---
## 🚀 How to Run the Project

1. **Clone the repository**
   ```
   https://github.com/ikrlalit/Crime-Cast.git
   cd CrimeCast

2. **Open your terminal or command prompt and run notebook using**
   ```
   jupyter notebook 21f3003123-notebook-t22024.ipynb

