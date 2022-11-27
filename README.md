# Predicción-de-Stroke
Realizado por: Laura Sofía Gómez Lizarazo

El siguiente proyecto tiene como objetivo la predicción de Stroke en diferentes pacientes, a partir del dataset mostrado a continuación:
https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset 

En dicho Dataset aparecen las siguientes características:

1) "id: unique identifier"
2) "gende"r: "Male", "Female" or "Other"
3) "age": age of the patient
4) "ypertension": 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
5) "heart_disease": 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6) "ever_married": "No" or "Yes"
7) "work_type": "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8) "Residence_type": "Rural" or "Urban"
9) "avg_glucose_level": average glucose level in blood
10) "bmi": body mass index
11) "smoking_status": "formerly smoked", "never smoked", "smokes" or "Unknown"
12) "stroke": 1 if the patient had a stroke or 0 if not

Dado lo anterior se procedio a realizar el procesamiento de los datos, que en este caso incluia la limpieza de los mismos y la creación de un nuevo archivo con los nuevos datos. Así mismo se normalizó y se realizaron los siguientes modelos de predicción con su respectiva validación.

* SVM (Maquinas de soporte vectorial)
* Regresión logística
* KNN (K vecinos más cercanos)






