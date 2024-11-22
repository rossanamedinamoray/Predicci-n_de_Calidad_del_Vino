# Análisis de Calidad del Vino: Clasificación Multiclase

Este proyecto utiliza técnicas de machine learning para predecir la calidad del vino basándose en características físico-químicas. Se entrenaron y evaluaron tres modelos de clasificación (Random Forest, K-Nearest Neighbors, y Regresión Logística) utilizando un dataset de vinos tintos y blancos.

---

## Propósito del Proyecto

El objetivo principal de este proyecto es:
- Predecir la calidad del vino (en una escala del 4 al 8) utilizando modelos de clasificación.
- Comparar el rendimiento de diferentes modelos y analizar su eficacia.
- Desarrollar un flujo de trabajo completo que incluye preprocesamiento, entrenamiento, evaluación y análisis de resultados.

---

## Dataset Utilizado

- **Fuente:** El dataset contiene características físico-químicas de muestras de vino y su calidad.
- **Características:** 
  - `fixed acidity`, `volatile acidity`, `citric acid`, `residual sugar`, `chlorides`, `free sulfur dioxide`, `total sulfur dioxide`, `density`, `pH`, `sulphates`, `alcohol`
  - `quality` (etiqueta de la calidad del vino)

---

## Técnicas Utilizadas

1. **Preprocesamiento de Datos:**
   - Escalado de características utilizando `StandardScaler`.
   - Tratamiento de outliers mediante el método del rango intercuartílico (IQR).
   - División de los datos en conjuntos de entrenamiento y prueba (80/20).

2. **Modelos de Clasificación:**
   - **Random Forest Classifier:** Modelo basado en árboles de decisión para capturar relaciones complejas.
   - **K-Nearest Neighbors (KNN):** Clasificación basada en la proximidad de instancias.
   - **Regresión Logística:** Modelo lineal utilizado como línea base.

3. **Evaluación de Modelos:**
   - Métricas: `precision`, `recall`, `f1-score`, y `accuracy`.
   - Curvas ROC y valores AUC para evaluar el rendimiento multiclase.

4. **Visualización:**
   - Gráficos Boxplot para análisis de outliers.
   - Curvas ROC para interpretar el rendimiento por clase.

---

## Requisitos Previos

- Bibliotecas necesarias: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`


- Cargar el Dataset: Asegúrate de que el archivo WineQT.csv esté en el mismo directorio que el notebook.

Resultados del Análisis:

Cuenta con gráficos de boxplots para outliers.
Informes de clasificación para cada modelo.
Curvas ROC con AUC para interpretar el rendimiento multiclase.
