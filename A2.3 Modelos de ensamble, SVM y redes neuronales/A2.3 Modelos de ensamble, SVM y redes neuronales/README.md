# Actividad 2.3: Estatus de la Salud Mental en Adultos — Ensamble, SVM y Red Neuronal.

## Descripción de la actividad.

Esta actividad consiste en el desarrollo de un reporte técnico que extiende el trabajo del segundo parcial, implementando cuatro modelos avanzados de clasificación: **Random Forest Classifier**, **Boosting**, **Support Vector Machine (SVM)** y una **Red Neuronal construida desde cero**. Cada modelo se entrena en dos escenarios: sin balanceo *(by Default)* y con la técnica **SMOTE** para evaluar el impacto del desbalance de clases en cada arquitectura.

## Base de datos.

- **Origen**: Portal de Datos Abiertos del Gobierno del Estado de Nuevo León, dentro del periodo de octubre del 2024 a agosto del 2025.
- **Fuente**: [Portal de Datos Abiertos de Nuevo León](https://datos.nl.gob.mx/)
- **Filtrado**: Adultos de entre 18 y 65 años residentes en San Pedro Garza García.
- **Desbalance original**: 547 registros de Trastornos mentales (75%) vs. 173 de Factores de riesgo (25%).

## Variables de interés.

- **Variable dependiente**: `descripcion_grupo_enfermedad_num` — Clasificación binaria:
  - `0`: Factores que influyen en el estado de salud y contacto con los servicios de salud.
  - `1`: Trastornos mentales y del comportamiento.
- **Variables independientes**:
  - `edad`
  - `sexo_num`
  - `institucion_unidad_medica_num`
  - `descripcion_enfermedad_num`

## Flujo de trabajo.

1. Importación de librerías.
2. Carga, filtrado y preparación del dataset.
3. Análisis del desbalance de clases.
4. Transformación de variables categóricas y creación del IMC.
5. Implementación de modelos por pares (by Default y SMOTE):
   - **Random Forest Classifier**
   - **Boosting**
   - **SVM** con StandardScaler
   - **Red Neuronal** desde cero (ReLU + Sigmoid, Binary Cross-Entropy, He initialization)
6. Evaluación: Accuracy, Matriz de Confusión, G-mean, Precision, Recall, F1-score y Curva de pérdida.
7. Tabla comparativa de los 8 modelos.
8. Discusiones, conclusiones y referencias.

## Índice de archivos.

- `saludMental_Avanzado.ipynb`: Notebook con el flujo completo de trabajo.
- `saludMental_Avanzado.html`: Reporte en formato web.

## Autor.

- **Estefania Nájera de la Rosa** – estefania.najera@udem.edu
- **Fecha**: 19 de marzo del 2026
