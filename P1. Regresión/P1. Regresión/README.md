# Actividad 1.3: Estatus de la Salud Mental en San Pedro Garza García.

### Descripción de la actividad.
Esta actividad consiste en el desarrollo de un reporte técnico detallado y un modelo predictivo para evaluar el estado de **salud mental en adultos** del municipio de San Pedro Garza García. El estudio analiza cómo diversos factores demográficos y socioeconómicos influyen en el bienestar emocional de la población en edad de trabajar, aplicando técnicas de limpieza de datos, escalamiento con `StandardScaler` y una comparativa entre modelos de **Regresión Lineal Múltiple** y **Random Forest** para capturar relaciones complejas.

### Base de datos.
* **Origen:** Los datos provienen del portal de **Datos Abiertos del Gobierno de Nuevo León**, enfocados en indicadores de bienestar y salud pública.
* **Fuente:** [Datos Abiertos NL - Indicadores de Salud](https://www.nl.gob.mx/tags/datos-abiertos)
* **Características:** El conjunto de datos incluye información detallada sobre edad, género, niveles de estrés reportados, acceso a servicios de salud y factores del entorno urbano en el municipio.

### Variables de interés.
* **Variable dependiente:** `Salud_Mental` (Puntaje o indicador del estado de salud mental del individuo).
* **Variables independientes principales:**
    * **Edad:** Factor demográfico clave en la población activa.
    * **Estrés percibido:** Nivel de tensión reportado por el ciudadano.
    * *Nota:* Se aplicó un análisis de importancia de variables y tratamiento de multicolinealidad para asegurar la validez del modelo.

### Índice de archivos.
* **saludMental_spgg.ipynb:** Notebook principal que contiene el flujo completo de trabajo:
    1.  Importación de librerías (`pandas`, `scikit-learn`, `seaborn`).
    2.  Carga y exploración de datos gubernamentales.
    3.  Limpieza de datos y escalamiento de variables (`StandardScaler`).
    4.  Análisis de correlación y selección de características.
    5.  Entrenamiento y comparación de modelos (**Linear Regression** vs. **Random Forest**).
    6.  Conclusiones basadas en el contexto socioeconómico de SPGG y referencias bibliográficas (OPS/OMS).
* **saludMental_spgg.html:** Reporte técnico exportado en formato web para su visualización.
* **dataset_salud_mental.csv:** Archivo de datos fuente utilizado para el entrenamiento del modelo.
