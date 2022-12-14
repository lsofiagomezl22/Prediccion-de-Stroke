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

Dado lo anterior se procedió a realizar el procesamiento de los datos, que en este caso incluía la limpieza de los mismos y la creación de un nuevo archivo con los nuevos datos. Así mismo se normalizó y se realizaron los siguientes modelos de predicción con su respectiva validación.

* SVM (Máquinas de soporte vectorial)
* Regresión logística
* KNN (K vecinos más cercanos)

A continuación se muestran los resultados de los métodos utilizados, a partir de dos métricas, f1 y AUC_ROC:

# Para SVM 

<img width="704" alt="image" src="https://user-images.githubusercontent.com/118940749/204142068-db88211a-04eb-45a3-9b28-d92195ec93bc.png">

# Para regresión logística:

<img width="713" alt="image" src="https://user-images.githubusercontent.com/118940749/204118943-9a5df164-484f-4e3d-863d-fd35d97b66a6.png">

# Para KNN:

<img width="636" alt="image" src="https://user-images.githubusercontent.com/118940749/204118954-5fae1706-4e8d-4db1-b610-3884a0071f65.png">
<img width="634" alt="image" src="https://user-images.githubusercontent.com/118940749/204118967-3e98df9d-0681-4537-b3b0-340d6be0aade.png">

# Conclusiones
A partir de las diferentes métricas y modelos de predicción utilizados, es posible evidenciar que el mejor método para predecir si un paciente presenta Stroke es el de regresión logística con una métrica de AUC_ROC.

Algo a resaltar es que la métrica que daba más alto en todos los casos fue la de AUC_ROC. Por otra parte el reultada más bajo fue el obtenido con máquinas de soporte vectorial


En cuanto a los tiempos de ejecución es muy importante destacar que el método más demorado fue el de SVM, tardándose aproximandamente 1 hora.

Otro aspecto importante que vale la pena mencionar es que a lo largo del proyecto se utilizó Gridserch cv, evaluando cada método con dos métricas f1 y AUC-ROC, por lo que es importante que se especifique el "refit" dentro de los parámetros del Gridserch-cv, pues en caso contrario saldrá error.

# Enlace del video explicativo.

https://youtu.be/gYzbJUZCqzI
