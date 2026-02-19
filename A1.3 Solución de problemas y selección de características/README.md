# Actividad 1.3: Predicción de Calificaciones Finales.

## Descripción de la actividad.
Esta actividad consiste en el desarrollo de un modelo de **Regresión Lineal Múltiple** para predecir las calificaciones finales de los estudiantes. Se trabaja con datos de dos instituciones educativas para comprender cómo factores demográficos, sociales y académicos impactan el resultado final, aplicando pruebas de multicolinealidad y manejo de datos atípicos.

## Base de datos.
* **Origen**: Los datos provienen del **UCI Machine Learning Repository** (Student Performance Dataset).
* **Fuente**: [UCI Machine Learning Repository - Student Performance](https://archive.ics.uci.edu/dataset/320/student+performance)
* **Características**: El conjunto de datos incluye variables sobre el entorno familiar, tiempo de estudio, fallas previas y consumo de alcohol, entre otros.

## Variables de interés.
* **Variable dependiente**: `G3` (Calificación final del estudiante).
* **Variables independientes**: Factores socio-académicos (evaluados mediante VIF para evitar colinealidad).

## Índice de archivos.
* **calificacionesFinales.csv**: Archivo de datos fuente.
* **calificacionesFinales.html**: Reporte en formato web.
* **calificacionesFinales.ipynb**: Contiene el flujo completo de trabajo:
    1. Importación de librerías.
    2. Carga y exploración de datos.
    3. Limpieza y manejo de outliers.
    4. Análisis de Multicolinealidad (VIF).
    5. Entrenamiento del modelo de Regresión Lineal Múltiple.
    6. Conclusiones y referencias.
