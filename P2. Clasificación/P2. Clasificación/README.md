## Proyecto 2: Clasificación del Estatus de la Salud Mental en San Pedro Garza García.

### Descripción de la actividad.
Esta actividad consiste en el desarrollo de un modelo de **clasificación supervisada** para analizar el estado de salud mental en adultos del municipio de San Pedro Garza García.  

A diferencia del análisis previo basado en regresión, en este proyecto se busca **clasificar a los individuos en dos categorías clínicas**:

- Trastornos mentales y del comportamiento  
- Factores que influyen en el estado de salud  

El estudio incorpora técnicas de **preprocesamiento de datos, selección de características y evaluación de modelos**, además de un enfoque comparativo entre modelos **con datos desbalanceados y balanceados mediante SMOTE**, con el fin de analizar el impacto del desbalance de clases en el rendimiento.

### Base de datos.
* **Origen:** Los datos provienen del portal de **Datos Abiertos del Gobierno de Nuevo León**, enfocados en indicadores de bienestar y salud pública.
* **Fuente:** [Datos Abiertos NL - Indicadores de Salud](https://www.nl.gob.mx/tags/datos-abiertos)
* **Características:** El conjunto de datos incluye información detallada sobre edad, género, niveles de estrés reportados, acceso a servicios de salud y factores del entorno urbano en el municipio.

### Variables de interés.

**Variable dependiente:**  
- `descripcion_grupo_enfermedad_num`  
  - Representa la clasificación del estado de salud mental en dos clases  

**Variables independientes finales:**  
- Edad  
- Sexo (codificado)  
- Institución médica (codificada)  

**Nota:**  
Se aplicaron técnicas de selección de características como:
- ANOVA.  
- VIF (Variance Inflation Factor).  

para evitar multicolinealidad y **data leakage**, eliminando variables redundantes como IMC y claves de enfermedad.

### Índice de archivos  
- `saludMental_spgg.html`  
  Reporte técnico exportado para visualización.
  
- `saludMental_spgg.ipynb`  
  Notebook principal que contiene:  
  - Carga y filtrado de datos (SPGG, 18–65 años).
  - Limpieza y transformación de variables.
  - Codificación con LabelEncoder. 
  - Ingeniería de características (IMC).  
  - Selección de variables (ANOVA, VIF).  
  - Entrenamiento de modelos de clasificación.
  - Evaluación de métricas.

### Metodología.

El análisis se centra en dos enfoques principales para cada modelo:

#### 1. Modelo desbalanceado.
Se entrena utilizando la distribución original de los datos, donde existe una mayor proporción de casos de trastornos mentales (~76%).  

#### 2. Modelo balanceado (SMOTE).  
Se aplica la técnica **SMOTE (Synthetic Minority Over-sampling Technique)** para generar datos sintéticos y equilibrar las clases, permitiendo un análisis más justo del desempeño del modelo.  

### Modelos implementados  

- Regresión Logística  
- Linear Discriminant Analysis (LDA)  
- Árbol de Decisión  
- Random Forest  
- Support Vector Machine (SVM)  
- Red Neuronal (implementación desde cero)  
