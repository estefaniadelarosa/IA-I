# Actividad 2.1: Estatus de la Salud Mental en Adultos — Regresión Logística.

## Descripción de la actividad.

Esta actividad consiste en el desarrollo de un reporte técnico de un modelo de **Regresión Logística** para clasificar el estado de salud mental en adultos dentro de la población en edad económicamente activa (18–65 años) que residen en el municipio de San Pedro Garza García. Se analizan variables demográficas y clínicas para predecir si un individuo pertenece a alguno de los dos grupos de clasificación, aplicando limpieza de datos, selección de características y manejo del desbalance de clases.

## Base de datos.

- **Origen**: Los datos provienen del Portal de Datos Abiertos del Gobierno del Estado de Nuevo León, dentro del periodo de octubre del 2024 a agosto del 2025.
- **Fuente**: [Portal de Datos Abiertos de Nuevo León](https://datos.nl.gob.mx/)
- **Filtrado**: Se delimita únicamente a adultos de entre 18 y 65 años residentes en San Pedro Garza García.
- **Características**: El conjunto de datos incluye información por individuo sobre fecha de consulta, edad, sexo, peso, altura, municipio, institución médica, y grupo/descripción de enfermedad.

## Variables de interés.

- **Variable dependiente**: `descripcion_grupo_enfermedad_num` — Clasificación binaria del grupo de enfermedad:
  - `0`: Factores que influyen en el estado de salud y contacto con los servicios de salud.
  - `1`: Trastornos mentales y del comportamiento.
- **Variables independientes** (tras análisis VIF y ANOVA):
  - `edad`: Edad del individuo.
  - `sexo_num`: Sexo codificado numéricamente.
  - `institucion_unidad_medica_num`: Institución médica codificada numéricamente.
  - `descripcion_enfermedad_num`: Descripción de la enfermedad codificada numéricamente.

## Flujo de trabajo.

1. Importación de librerías.
2. Carga y exploración del dataset.
3. Limpieza de datos y filtrado (municipio y rango de edad).
4. Análisis del desbalance de clases.
5. Transformación de variables categóricas (LabelEncoder).
6. Ingeniería de características (cálculo de IMC).
7. Selección de características (Mapa de calor, ANOVA, VIF).
8. Entrenamiento del modelo — 4 variantes:
   - By Default.
   - Balanced.
   - Manual-Balanced.
   - **SMOTE** *(mejor desempeño)*.
9. Evaluación: Accuracy, F1-score, G-mean, AUC, validación cruzada y Matriz de Confusión.
10. Conclusiones y referencias.

## Índice de archivos.

- `regresionLogistica_SM-SPGG.ipynb`: Notebook con el flujo completo de trabajo.
- `saludMental_Avanzado.html`: Reporte en formato web.

## Autor.

- **Estefania Nájera de la Rosa** – estefania.najera@udem.edu
- **Fecha**: 2 de marzo del 2026
