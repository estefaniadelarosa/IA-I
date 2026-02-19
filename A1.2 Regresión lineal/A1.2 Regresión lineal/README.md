# Actividad 1.2: Las características que definen el nivel de felicidad.

## Descripción de la actividad.
Esta actividad consiste en un reporte técnico que analiza los niveles de felicidad en diversos países. Se implementan modelos de regresión para predecir el bienestar basado en factores socioeconómicos, evaluando la precisión y la relación entre variables mediante gráficas de dispersión y líneas de tendencia.

## Base de datos.
* **Origen**: Los datos provienen del **World Happiness Report**.
* **Fuente**: [Data sharing | The World Happiness Report](https://www.worldhappiness.report/data-sharing/)

## Variables del proyecto.

### Variable Dependiente (Target):
* **`Life Ladder` (o Score de Felicidad)**: Es la medida del nivel de felicidad percibida por los habitantes de cada país.

### Variables Independientes (Predictoras):
1.  **`Log GDP per capita`**: El nivel de riqueza económica por persona (en escala logarítmica).
2.  **`Social support`**: El respaldo social percibido (tener a alguien con quien contar).
3.  **`Healthy life expectancy at birth`**: La esperanza de años de vida con buena salud.
4.  **`Freedom to make life choices`**: La libertad percibida para tomar decisiones de vida.

## Metodología aplicada.
* **Regresión Lineal Simple**: Se analizó la relación directa entre el PIB (`Log GDP per capita`) y la felicidad.
* **Regresión Lineal Múltiple**: Se integraron las 4 variables mencionadas para mejorar la capacidad predictiva del modelo.
* **Validación**: Uso de `train_test_split` para separar datos de entrenamiento y prueba.

## Índice de archivos.
1.  **[Felicidad.ipynb](./Felicidad.ipynb)**: Notebook con la limpieza de datos, análisis de correlación y entrenamiento de modelos.
2.  **[Felicidad.html](./Felicidad.html)**: Exportación del reporte para lectura rápida.
