# Actividad 1.2: Las características que definen el nivel de felicidad.

## Descripción de la actividad.
Esta actividad consiste en un reporte técnico de los niveles de felicidad de diversos países en el mundo mediante la implementación de modelos de **regresión lineal simple** con una variable independiente y de **regresión lineal múltiple** con cuatro variables independientes. Se busca identificar qué factores socioeconómicos tienen mayor peso en el bienestar global.

## Base de datos.
* **Origen**: Los datos provienen del **World Happiness Report**, un estudio que clasifica la felicidad de las naciones basándose en diversos indicadores.
* **Fuente**: [Data sharing | The World Happiness Report](https://www.worldhappiness.report/data-sharing/)
* **Características**: 
    * El conjunto de datos incluye métricas anuales por país que miden el soporte social, libertad, generosidad y corrupción, entre otros.

## Variables de interés.
* **Variable dependiente**: `Life Ladder` (Puntaje de felicidad percibida).
* **Variables independientes principales**: 
    1. `Log GDP per capita` (Nivel de riqueza).
    2. `Social support` (Apoyo social).
    3. `Healthy life expectancy at birth` (Esperanza de vida).
    4. `Freedom to make life choices` (Libertad de decisión).

## Índice de archivos.
* **World_Happiness_Report.csv**: Archivo de datos fuente.
* **Felicidad.html**: Reporte en formato web.
* **Felicidad.ipynb**: Contiene el flujo completo de trabajo:
    1. Importación de las librerías.
    2. Carga de datos.
    3. Limpieza de datos.
    4. Análisis de regresión simple.
    5. Análisis de regresión múltiple.
    6. Conclusiones y referencias.
 * **WHR22_Data_Figure_2.1.xlsx**: Datos extras obtenidos por The World Happiness Report.
