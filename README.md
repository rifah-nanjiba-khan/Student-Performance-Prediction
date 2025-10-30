# 🎓 Student-Performance-Prediction
> A research-driven AI pipeline for education analytics (synthetic demonstration of a real-world project)

In today’s fast-paced world, data-driven prediction holds immense potential to optimize workflows, reshape business strategies, and accelerate growth. 
The **'Student Performance Prediction'** project represents a step toward that optimization — grounded in a comprehensive literature review, a deep understanding of organizational data and needs, and a commitment to precision and purpose.
This repository demonstrates three complete **machine learning pipelines** designed to predict student outcomes in an **educational programme** setting.  
The project focuses on a complex, real-world dataset with substantial variability and noise, achieving strong predictive performance and model explainability.

> ⚠️ All data in this repository is **synthetic** and **anonymized** to protect confidentiality. The original code and dataset are not included in this repository. This project summary reflects my independent work and methodology.

---

## 🧩 Overview

This project showcases an end-to-end workflow for building interpretable predictive models.  
It includes:
- Data preprocessing with custom pipelines  
- Feature engineering and transformation  
- Training and evaluation of three different models
- Model interpretability using **LIME**  
- Modular and reusable structure for real-world applications  

---

## 🚀 Key Features

- 🧹 **Preprocessing Pipeline**  
  Categorizes new inputs, handles missing values, encodes categorical variables, and scales numerical features.

- 🧱 **Custom Transformers**
  - Handles mistakes in manual data inputs.
  - Deals with multi-picklist values.
  - Drops unnecessary columns for dynamic feature removal during preprocessing.
    
- ⚖️ **Imbalance Handling**  
  Techniques like **SMOTE**, **class weighting**, and **undersampling** were tested for fairness and stability.
  
- 🤖 **Model Training and Evaluation**
  Multiple algorithms (e.g., Logistic Regression, Random Forest, XGBoost) and ensemble techniques have been tried and tested out in the building process to check competitive performance. 

- 🧠 **Model Explainability**  
  Integrated **LIME** for local-level interpretability and narrative generation of model predictions.

- 🔍 **Clean, Modular Codebase**  
  Organized structure following industry best practices for ML development.

---

## ⚙️ Workflow

1. **Data Preprocessing**
   - Addresses data gaps using systematic logic and Excel formulas to ensure dataset completeness
   - Standardizes manual inputs into predefined categorical values
   - Defines the logical order of categorical variables based on organizational requirements
   - Encodes categorical and numerical features
   - Drops irrelevant columns using a custom transformer
   - Outputs a clean, transformed dataset ready for model input

2. **Model Training**
   - Uses Scikit-learn’s pipeline for training and validation  
   - Saves the final model (`model.pkl`) for reproducibility  

3. **Model Testing**
   - Optimizes hyperparameters through validation testing
   - Performs model evaluation using classification metrics (accuracy, precision, recall, F1-score)
  
4. **Model Interpretation**
   - Aggregates feature contributions for cleaner interpretability
   - Generates **LIME explanations** to visualize how features influence predictions  
   - Allows localized insights for each individual prediction  

---

## ⭐️ Model Performance
The models demonstrated strong overall performance across all prediction tasks.
**Model 1** achieved balanced accuracy despite data complexity, while **Model 2** and **Model 3** showed exceptional precision and recall, reflecting high reliability in identifying at-risk and successful students. 
These results indicate the system’s robustness and adaptability across diverse educational outcomes.
> Figure: Model Performance Summary
<img width="769" height="172" alt="image" src="https://github.com/user-attachments/assets/0001637f-8787-4989-854f-3c1acd27a330" />


---

## 🧠 Example Usage

### Example Input (synthetic)
```
sample_input = {
    "column_1": 12,
    "column_2": "Urban",
    "column_3": "Female",
    "column_4": 0.75
}
```
### Eample Output
```
sample_output = {
    Prediction: Not selected
    probability: 84%,
    "lime_explanation": {
        "feature_1": "+0.12",
        "feature_2": "-0.08"
    }
}
```
> Figure: Demo Contribution Plot
<img width="628" height="480" alt="image" src="https://github.com/user-attachments/assets/ab31bc97-5b7e-46ae-9845-ef237980a68a" />


---

## 🧰 Requirements

Install dependencies:
pip install -r requirements.txt

---

## 🔒 Data Privacy Notice

All data, feature names, and program identifiers have been replaced with generic placeholders
(e.g., column_1, data_point_1, Model 1).
No confidential data or organizational references are stored or shared in this repository.

---

## 👩‍💻 Author

Developed by Rifah Nanjiba Khan — Research Assistant & Data Science Enthusiast
> Focused on applying data science and AI to real-world social impact projects.
