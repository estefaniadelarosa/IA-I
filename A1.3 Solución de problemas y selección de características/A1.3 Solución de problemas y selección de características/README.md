# Actividad 1.3: Predicción de Calificaciones Escolares.

## Descripción de la actividad.
Esta actividad consiste en el desarrollo de un reporte técnico de un modelo de **Regresión Lineal Múltiple** para predecir las calificaciones finales de los estudiantes. Se analizan datos de dos instituciones educativas para comprender cómo factores demográficos, sociales y académicos impactan el desempeño escolar, aplicando limpieza de datos, manejo de *outliers* y análisis de multicolinealidad.

## Base de datos.
* **Origen**: Los datos provienen del **UCI Machine Learning Repository**, específicamente del conjunto de datos sobre el desempeño de estudiantes en materias como matemáticas.
* **Fuente**: [UCI Machine Learning Repository - Student Performance](https://archive.ics.uci.edu/dataset/320/student+performance)
* **Características**: El conjunto de datos incluye información detallada sobre el entorno familiar, tiempo de estudio, fallas previas, salud y consumo de alcohol de estudiantes de secundaria.

## Variables de interés.
* **Variable dependiente**: `G3` (Calificación final del estudiante).
* **Variables independientes principales**:
    * **G1 y G2**: Calificaciones de los primeros dos periodos (analizadas para medir progresión).
    * **Absences**: Número de ausencias escolares.
    * **Studytime**: Tiempo de estudio semanal.
    * **Failures**: Número de clases reprobadas anteriormente.
    * *(Evaluadas mediante VIF para asegurar la validez del modelo).*

## Índice de archivos.
* **student-mat.csv**: Archivo de datos fuente original.
* **calificacionesFinales.html**: Reporte en formato web.
* **calificacionesFinales.ipynb**: Contiene el flujo completo de trabajo:
    1. Importación de las librerías.
    2. Carga y exploración de datos.
    3. Limpieza de datos y manejo de *outliers*.
    4. Análisis de Multicolinealidad (VIF).
    5. Entrenamiento del modelo de Regresión Lineal Múltiple.
    6. Conclusiones y referencias.
