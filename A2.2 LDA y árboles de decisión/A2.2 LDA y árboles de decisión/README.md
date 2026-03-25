
# Actividad 2.2: Estatus de la Salud Mental en Adultos — LDA y Árbol de Decisión.

## Descripción de la actividad.

Esta actividad consiste en el desarrollo de un reporte técnico que extiende el trabajo de la Regresión Logística (Actividad 2.1), incorporando dos nuevos modelos de clasificación: **Análisis Discriminante Lineal (LDA)** y **Árbol de Decisión** (inicial y podado). Se retoma el mismo dataset de salud mental del municipio de San Pedro Garza García, aplicando la técnica de balanceo **SMOTE** —identificada como la más efectiva en la actividad anterior— para preparar los datos de entrenamiento de ambos modelos.

## Base de datos.

- **Origen**: Portal de Datos Abiertos del Gobierno del Estado de Nuevo León, dentro del periodo de octubre del 2024 a agosto del 2025.
- **Fuente**: [Portal de Datos Abiertos de Nuevo León](https://datos.nl.gob.mx/)
- **Filtrado**: Adultos de entre 18 y 65 años residentes en San Pedro Garza García.
- **Nota**: Se aplica **SMOTE** sobre los datos de entrenamiento para corregir el desbalance de clases (75% Trastornos mentales vs. 25% Factores de riesgo).

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
2. Carga y preparación del dataset (filtrado y SMOTE).
3. **LDA**:
   - Codificación de la variable objetivo.
   - Pair Plot e Histogramas exploratorios.
   - Mapa de calor de correlación.
   - Implementación con 1 componente (clasificación binaria).
   - Visualización de la distribución lineal 1D.
4. **Árbol de Decisión Inicial**: generación, visualización, métricas y Matriz de Confusión.
5. **Árbol de Decisión Podado**: búsqueda del alpha óptimo (StratifiedKFold), generación, métricas y Matriz de Confusión.
6. Comparación de resultados entre modelos.
7. Discusiones, conclusiones y referencias.

## Índice de archivos.

- `LDA-Tree_SPGG.ipynb`: Notebook con el flujo completo de trabajo.
- `saludMental_Avanzado.html`: Reporte en formato web.

## Autor.

- **Estefania Nájera de la Rosa** – estefania.najera@udem.edu
- **Fecha**: 5 de marzo del 2026
