# Actividad 1.1: Análisis de obesidad.

## Descripción de la actividad.
Esta actividad consiste en un reporte técnico del análisis estadístico de 2,111 individuos para comprender qué variables influyen significativamente en el umbral de la obesidad en América Latina. 
Se aplican técnicas de limpieza, transformación de variables categóricas y análisis de correlación.

## Base de datos.
* **Origen**: Los datos fueron recolectados por investigadores de la **Universidad de la Costa, Colombia**.
* **Fuente**: [Dataset en GitHub](https://raw.githubusercontent.com/estefaniadelarosa/IA-I/refs/heads/main/A1.1%20Aprendizaje%20estad%C3%ADstico-autom%C3%A1tico/A1.1%20Obesidad.csv)
* **Características**:
    * **Registros**: 2,111 individuos.
    * **Variables (10)**: Sexo, Edad, Estatura, Peso, Historial familiar de sobrepeso, Consumo de calorías, Consumo de vegetales, Fumador, Consumo de agua y Nivel de obesidad.
    * **Población**: Individuos de entre 14 y 61 años (Promedio: 24 años).

## Variables de interés.
* **Variable dependiente**: `NivelDeObesidad` (Categorías desde Bajo Peso hasta Obesidad Tipo III).
* **Variable independiente principal**: `Peso` (Identificada mediante análisis de correlación con un valor de 0.387).

## Índice de archivos.
* `A1.1_Obesidad.csv`: Archivo de datos fuente.
* `Obesidad.html`: Reporte técnico exportado en formato web para su visualización.
* `Obesidad.ipynb`: Contiene el flujo completo de trabajo:
    1. Introducción y Objetivos.
    2. Exploración Estadística.
    3. Definición de Variables.
    4. Metodología y Limpieza de Datos (Label Encoding).
    5. Visualización (Histogramas).
