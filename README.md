# 🚗 Road Accident Severity Prediction

This repository contains a **Machine Learning model** for predicting the severity of road accidents in the United States. The project involves **data preprocessing, feature engineering, model training, and evaluation** using a **Random Forest Classifier**.

---

## 📌 Project Overview

This project aims to **predict accident severity** based on various factors such as **weather conditions, location, time of day, and road features**. The dataset used is **US Accidents (March 2023)**, which contains millions of traffic accident records.

🚀 **Main Steps in the Pipeline:**
1. **Data Cleaning & Processing**  
   - Handling missing values  
   - Converting categorical features to numerical  
   - Extracting time-based features (Hour, Day, Month, Weekday)  

2. **Feature Engineering**  
   - Removing unnecessary columns  
   - Encoding categorical variables  
   - Standardizing numerical features  

3. **Train-Validation-Test Split**  
   - **Train (75%)** | **Validation (15%)** | **Test (10%)**

4. **Machine Learning Model**  
   - **Random Forest Classifier** for accident severity prediction  
   - **Hyperparameter tuning and model evaluation**

5. **Feature Importance Analysis**  
   - Identifying key factors influencing accident severity  

---

## 📂 Dataset Information

The dataset can be downloaded from Kaggle:  
📌 **[US Accidents Dataset on Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)**  

The dataset contains **road accident records** from across the US with features related to **location, weather, traffic signals, and accident details**.

| Feature | Description |
|---------|------------|
| `Severity` | Accident severity level (1-4) |
| `Start_Lat`, `Start_Lng` | Latitude & Longitude of accident |
| `Distance(mi)` | Distance impacted by accident |
| `Weather_Condition` | Weather during accident (Rain, Fog, Snow, etc.) |
| `Temperature(F)`, `Humidity(%)`, `Wind_Speed(mph)` | Weather factors |
| `Junction`, `Traffic_Signal`, `Bump` | Road conditions |
| `Hour`, `Day`, `Month`, `Weekday` | Extracted time-based features |

🚀 **The goal is to predict the `Severity` of an accident using these features.**

---

## 📖 **Approach & Assumptions**

### **🛠 Approach**
1. **Data Cleaning**: Handled missing values by removing highly null columns and filling others using median/mode imputation.  
2. **Feature Engineering**: Extracted time-based features and encoded categorical variables using **Label Encoding**.  
3. **Data Splitting**: The dataset was split into **train (75%)**, **validation (15%)**, and **test (10%)** sets.  
4. **Model Training**:  
   - Used **RandomForestClassifier** with default hyperparameters.  
   - Trained the model on **training data** and evaluated on **validation data**.  
5. **Evaluation**:  
   - Used **Accuracy, Classification Report, and Confusion Matrix** for performance analysis.  
6. **Feature Importance Analysis**:  
   - Identified key factors affecting accident severity.

### **🧐 Assumptions**
- The dataset is assumed to be **representative of real-world accident patterns**.  
- Missing values were handled by **dropping columns with excessive missing data** and **filling missing values appropriately**.  
- The **severity of an accident is influenced by weather, time, and road conditions**, which were prioritized in feature selection.

---

## 📦 **Installation & Setup** 

To run this project locally, follow these steps:

### **🔹 Clone the Repository**
```bash
git clone https://github.com/YOUR_GITHUB_USERNAME/Road-Accident-Severity-Prediction.git
cd Road-Accident-Severity-Prediction
