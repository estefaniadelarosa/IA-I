# Estatus de la Salud Mental en adultos del municipio más acaudalado de América Látina.

Este repositorio contiene un reporte técnico detallado sobre el desarrollo de modelos de clasificación vistos en el segundo parcial para analizar y predecir el estado de la salud mental en adultos del municipio de San Pedro Garza García, Nuevo León. El estudio busca identificar cómo influyen diversos factores demográficos y socioeconómicos en la población en cuanto las enfermedades de salud mental registradas en el municipio más acaudalado de América Latina.

El proyecto utiliza técnicas de aprendizaje estadístico y automático para identificar variables determinantes en el bienestar emocional, basándose en datos obtenidos de portales de **Datos Abiertos del Gobierno de Nuevo León**.

### Estructura del repositorio.

* **saludMental_spgg.ipynb**: Notebook principal que contiene todo el flujo de trabajo:
    * Limpieza y preparación de datos.
    * Análisis Exploratorio de Datos (EDA).
    * Implementación de escalamiento de variables con `StandardScaler`.
    * Entrenamiento y evaluación de los modelos de Regresión Lineal y Random Forest.
* **Reporte Técnico Integrado**: Documentación detallada dentro del notebook que justifica la metodología, basada en lineamientos de la OPS/OMS y contexto regional de salud.
* **Fuentes de consulta**: Bibliografía que incluye datos gubernamentales y artículos de análisis socioeconómico.

### Metodología.

El análisis se centra en la comparación dos enfoques por cada modelo.
1. **Modelo desbalanceado**: Para ver el comportamiento original de los datos en sus clases sin ninguna modificación.
2. **Modelo balanceado**: Para manipular la cantidad de datos en las clases y obtener resultados de los análisis de forma controlada y consciente del desbalance que existe.
### Autor.

**Estefania Nájera de la Rosa** - [estefania.najera@udem.edu](mailto:estefania.najera@udem.edu)  
**Fecha**: 26 de febrero del 2026

