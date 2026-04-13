# 😴 Sleep Health & Lifestyle — Disorder Prediction

## 🔍 Problem
Can we predict whether a person has a Sleep Disorder (None, Insomnia, 
or Sleep Apnea) based on their lifestyle and health data?
Early detection of sleep disorders can help healthcare providers 
intervene before conditions worsen.

## 📊 Dataset
- 374 records, 13 features
- Source: Kaggle — Sleep Health and Lifestyle Dataset
- Features: Age, Gender, Occupation, BMI, Stress Level, 
  Blood Pressure, Physical Activity, Daily Steps
- Target: Sleep Disorder (None / Insomnia / Sleep Apnea)
- Challenge: Class imbalance — 219 healthy vs 77-78 disorder cases

## 🛠️ Approach
- Performed EDA using pandas, matplotlib and seaborn
- Split Blood Pressure into Systolic and Diastolic features
- Encoded categorical variables using LabelEncoder
- Trained 3 models: Logistic Regression, Random Forest, XGBoost
- Selected XGBoost as best model (90.6% accuracy)
- Tuned hyperparameters using GridSearchCV

## 📈 Results
| Model | Accuracy |
|---|---|
| Logistic Regression | 88% |
| Random Forest | 88% |
| XGBoost | 90.6% ✅ |

- BMI Category was the single most important feature
- Model correctly identified 42/43 healthy individuals
- F1 Score of 0.97 on majority class (None)

## 🔮 Next Steps
- Apply SMOTE to handle class imbalance
- Deploy model as a web app using Streamlit
- Collect more data to improve minority class detection

## 🧰 Tech Stack
Python | Pandas | Seaborn | Matplotlib | Scikit-learn | XGBoost

## 👤 Author
Vineet Prakash
[LinkedIn](https://linkedin.com/in/vineetprakash03) | 
[Kaggle](https://kaggle.com/vin1bun) | 
[GitHub](https://github.com/vin1bun)
