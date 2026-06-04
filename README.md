# FitPred AI Model

Repository ini berisi source code, dokumentasi, dan file pendukung model AI untuk aplikasi **FitPred**. Model AI digunakan untuk memprediksi kategori **Recommended Meal Plan** berdasarkan data kesehatan, gaya hidup, dan preferensi makanan pengguna.

## Project Overview

FitPred adalah aplikasi berbasis web yang membantu pengguna mendapatkan rekomendasi meal plan berdasarkan data kesehatan dan kebiasaan harian. Model AI pada repository ini berperan untuk melakukan klasifikasi meal plan ke dalam tiga kategori:

- High-Protein Diet
- Low-Carb Diet
- Low-Fat Diet

Model dikembangkan menggunakan **TensorFlow Functional API** dan proses training dipantau menggunakan **TensorBoard**.

## Repository Structure

```text
fitpred-ai-model/
├── notebook/
│   └── Model_AI_Meal_Plan_Final_FunctionalAPI_TensorBoard.ipynb
├── model-files/
│   ├── feature_columns.json
│   ├── meal_plan_mapping.json
│   ├── scaler_info.json
│   ├── model_metadata.json
│   └── tensorboard_logs.zip
├── requirements.txt
└── README.md
```

## Model AI

File model AI disimpan pada Google Drive agar dapat diakses dan diunduh.

Google Drive Model AI:
https://drive.google.com/drive/folders/1At5jlbGjEYGN8Pa0SRNAzm5CJtV46lWq?usp=sharing

## Dataset and Features
Model menggunakan data kesehatan, gaya hidup, dan preferensi makanan pengguna. Beberapa fitur yang digunakan antara lain:
- Age
- Height
- Weight
- Blood Pressure
- Cholesterol Level
- Blood Sugar Level
- Daily Steps
- Exercise Frequency
- Sleep Hours
- Caloric Intake
- Protein Intake
- Carbohydrate Intake
- Fat Intake
- Gender
- Chronic Disease
- Genetic Risk Factor
- Allergies
- Alcohol Consumption
- Smoking Habit
- Dietary Habits
- Preferred Cuisine
- Food Aversions

## Evaluation
Model dievaluasi menggunakan metrik klasifikasi berikut:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## TensorBoard
TensorBoard digunakan untuk memantau dan memvisualisasikan metrik perlatihan model, seperti:
- Training loss
- Training accuracy
- Validation loss
- Validation accuracy

## How to Run Notebook
Install dependencies:
'''
pip install -r requirements.txt
'''
Buka notebook berikut di Google Colab atau Jupyter Notebook:
'''
notebook/FitPred_Model_AI.ipynb
'''

## Requirements
Library utama yang digunakan:
- TensorFlow
- Pandas
- Numpy
- Scikit-learn
- Matplotlib
- Seaborn

## AI API Deployment
Model AI juga telah dibuat dalam bentuk REST API menggunakan FastAPI dan dideploy ke Railway.

API Documentation:
https://model-api-production-9ded.up.railway.app/docs 
