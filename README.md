# Crop Recommendation Dataset
Maximize agricultural yield by recommending appropriate crops

Precision agriculture is in trend nowadays. It helps the farmers to get informed decision about the farming strategy. Here, I present you a dataset which would allow the users to build a predictive model to recommend the most suitable crops to grow in a particular farm based on various parameters.

# 🌾 Crop Classification Model

## 📌 Project Objective
Predict the most suitable **crop type** based on soil nutrients and environmental conditions using supervised machine learning.

### Data Source: https://www.kaggle.com/datasets/atharvaingle/crop-recommendation-dataset
## 🗂️ Dataset
- **Rows**: 2,200 samples
- **Features**:  
  - `N`, `P`, `K` (soil nutrients)  
  - `TC` (temperature °C), original feature name was: `temperature`.
  - `RH` (relative humidity %), original feature name was: `humidity`.  
  - `pH` (soil acidity)  
  - `RF` (rainfall mm), original feature name was: `rainfall`.   
- **Target**: `Crop` (22 classes), original feature name was: `label`. 

## 🧠 Model
- **Algorithm**: Random Forest Classifier
- **Preprocessing**: Label encoding for crop types; no missing values
- **Train/Test Split**: 80/20 and 70/30 (stratified)

## 📈 Results
- **Accuracy (80/20)**: 99.32%  
- **Accuracy (70/30)**: 99.54%  
- **Cross-Validation (5-fold)**: 99.41%

## 🔍 Feature Importance
Key features influencing crop prediction:
- Soil nutrients (`N`, `P`, `K`)
- Environmental factors (`TC`, `RH`, `pH`, `RF`)

## 📦 Dependencies
- Python 3.x
- pandas, scikit-learn, matplotlib, seaborn, plotly

## 📊 Visualizations
- Feature importance plots
- Confusion matrix
- Accuracy & F1-score reporting

## ✅ Conclusion
This model is accurate, robust, and ready for deployment in agricultural advisory tools.
