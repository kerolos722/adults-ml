# Adult Income Prediction — ML Project (Deployment-Ready) 🚀

## 📌 Project Overview
This project builds a robust machine learning classification pipeline to predict whether a person's **annual income** is above or below **$50K**, based on various census demographic and employment attributes.[cite: 1]

This repository is strictly designed to be **deployment-ready**.[cite: 1] Every data preprocessing step—including imputation, encoding, and scaling—is fitted exclusively on the training split and immediately persisted using `joblib`.[cite: 1] This ensures that the exact same transformations can be seamlessly applied to any new raw data during real-time inference (e.g., via a Streamlit web application).[cite: 1]

## 📊 Dataset Description
The model is trained on the classic **UCI Adult / Census Income dataset**.[cite: 1] 

### Data Dictionary
| Feature | Description |
|---|---|
| `age` | Age of the individual (years).أهلاً بك يا كيرلس! إعداد ملف `README.md` احترافي على حسابك `kerolos722` هو خطوة ممتازة لإبراز مهاراتك في هندسة البيانات وتطوير نماذج تعلم الآلة. 

بناءً على الكود المرفق، قمت بتجهيز هيكل مبدئي لملف الـ `README` باللغة الإنجليزية (كما هو متعارف عليه في GitHub). هذا القالب يبرز الجانب العملي للمشروع وجاهزيته للعمل مع واجهة ويب تفاعلية.

### قالب `README.md` المقترح:

```markdown
# Adult Income Prediction — ML Project (Deployment-Ready)

## 📌 Project Overview
This project builds a classification pipeline to predict whether a person's **annual income** (`income`) is above or below **$50K**, based on census attributes (age, education, occupation, hours worked, etc.)[cite: 1]. 

A key focus of this project is making the pipeline **deployment-ready**[cite: 1]. Every preprocessing step—such as imputation, encoding, and scaling—is fit strictly on the training split and immediately persisted using `joblib`[cite: 1]. This ensures that the exact same transformations can be reliably applied to a single new row of raw input during inference (for example, through a Streamlit web application)[cite: 1].

## 📊 Dataset
The model is trained on the classic **UCI Adult / Census Income** dataset[cite: 1]. 
* **Total Records:** 32,561 rows and 15 columns[cite: 1].
* **Key Features:** `age`, `workclass`, `education`, `marital.status`, `occupation`, `race`, `sex`, `hours.per.week`, `native.country`, etc[cite: 1].
* **Target Variable:** `income` (<=50K or >50K)[cite: 1].

## ⚙️ Data Preprocessing & Cleaning
* **Missing Values Handling:** Missing values in the raw dataset were initially encoded as the literal string `"??"`[cite: 1]. These were converted to true `NaN` values to accurately measure missingness[cite: 1].
* **Imputation:** Columns with missing data (`occupation`, `workclass`, and `native.country`) were missing less than 10% of their values, allowing for efficient most-frequent-category imputation[cite: 1].

## 🛠️ Technologies & Libraries Used
* **Data Manipulation & Visualization:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`[cite: 1].
* **Preprocessing:** `sklearn.preprocessing`, `sklearn.impute`, `category_encoders`[cite: 1].
* **Machine Learning Algorithms:** Linear models, Tree Ensembles (Random Forest, Extra Trees), Boosting libraries (`XGBoost`, `CatBoost`, `LightGBM`)[cite: 1].
* **Model Serialization:** `joblib`, `pickle`[cite: 1].
