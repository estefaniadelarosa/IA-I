# Actividad 1.2: Las características que definen el nivel de felicidad.

## Descripción de la actividad.
Esta actividad consiste en un reporte técnico que analiza los niveles de felicidad en diversos países del mundo. El objetivo principal es identificar qué factores socioeconómicos tienen mayor impacto en el bienestar percibido, implementando modelos de:
1. **Regresión Lineal Simple**: Utilizando una variable independiente para predecir la felicidad.
2. **Regresión Lineal Múltiple**: Utilizando cuatro variables independientes para un modelo más robusto.

## Base de datos.
* **Origen**: Los datos provienen del **World Happiness Report**.
* **Fuente**: [Data sharing | The World Happiness Report](https://www.worldhappiness.report/data-sharing/)
* **Características**:
    * El conjunto de datos evalúa métricas globales de bienestar, tales como el PIB per cápita, apoyo social, esperanza de vida, libertad, generosidad y percepción de corrupción.

## Metodología Aplicada.
* **División de datos**: Se utilizó la técnica de `train_test_split` para entrenar los modelos y validar su precisión.
* **Librerías utilizadas**: `pandas`, `numpy`, `matplotlib`, `seaborn` y `sklearn.linear_model`.
* **Análisis**: Se evaluaron las líneas de tendencia y la correlación entre variables para determinar la validez de las predicciones.

## Índice de archivos.
Este directorio contiene los siguientes recursos:
1.  **[Felicidad.ipynb](./Felicidad.ipynb)**: Notebook con el análisis completo, la implementación de los modelos de regresión y las visualizaciones de los resultados.
2.  **Reportes Adicionales**: Cualquier archivo CSV o exportación HTML relacionada con este análisis.
