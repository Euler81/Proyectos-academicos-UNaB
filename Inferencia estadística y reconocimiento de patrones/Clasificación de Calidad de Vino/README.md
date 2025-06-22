# Proyecto de Clasificación de Calidad de Vino

## Descripción del Proyecto

Este proyecto se enfoca en el análisis y la predicción de la calidad del vino utilizando técnicas de machine learning. A partir de un conjunto de datos con características fisicoquímicas de vinos, se aplicaron y evaluaron diversos algoritmos de clasificación para determinar cuál es el más efectivo para distinguir entre vinos de calidad "buena" y "mala".

Este trabajo fue desarrollado como parte del primer parcial de la asignatura **Inferencia Estadística y Reconocimiento de Patrones**.

* **Universidad:** Universidad Nacional Guillermo Brown (UNaB)
* **Asignatura:** Inferencia Estadística y Reconocimiento de Patrones
* **Profesor:** Sebastian Simondi
* **Fecha de Entrega:** 22/10/2024

### Integrantes del Equipo

* Lucas León González
* David Lobos
* Euler Diego

---

## Objetivos

1.  **Aplicar** todos los algoritmos de clasificación estudiados en la asignatura.
2.  **Calcular y analizar** las métricas de rendimiento y las matrices de confusión para cada modelo.
3.  **Determinar** si existe un modelo que sea significativamente superior a los demás para la tarea de clasificación propuesta.

---

## Dataset

Se utilizó el conjunto de datos `calidadvino.csv`, que contiene 1599 registros y 12 variables (11 características fisicoquímicas y 1 variable objetivo de calidad).

Las características incluyen:
* `fixed acidity`
* `volatile acidity`
* `citric acid`
* `residual sugar`
* `chlorides`
* `free sulfur dioxide`
* `total sulfur dioxide`
* `density`
* `pH`
* `sulphates`
* `alcohol`

La variable objetivo `quality` (con valores de 3 a 8) fue transformada en una variable categórica binaria para el problema de clasificación:
* **Mala Calidad:** si `quality` <= 5
* **Buena Calidad:** si `quality` > 5

---

## Metodología y Flujo de Trabajo

El análisis se llevó a cabo siguiendo los siguientes pasos:

1.  **Carga y Exploración de Datos:** Se cargó el dataset y se realizó un análisis exploratorio inicial para entender la distribución de las variables.
2.  **Preprocesamiento de Datos:**
    * Transformación de la variable objetivo `quality` en una clase binaria.
    * División de los datos en conjuntos de entrenamiento (80%) y prueba (20%).
    * Estandarización de las características numéricas utilizando `StandardScaler` para asegurar que todos los atributos tengan una escala común.
3.  **Entrenamiento de Modelos:** Se implementaron y entrenaron los siguientes algoritmos de clasificación:
    * Regresión Logística
    * Máquinas de Soporte Vectorial (SVM) con `GridSearchCV` para optimización de hiperparámetros.
    * Árbol de Decisión
    * Random Forest (Bosque Aleatorio)
    * K-Nearest Neighbors (KNN) con búsqueda del `k` óptimo.
4.  **Evaluación:** Cada modelo fue evaluado en el conjunto de prueba utilizando:
    * **Matriz de Confusión:** Para visualizar el desempeño del clasificador.
    * **Métricas Clave:** Precisión (Precision), Sensibilidad (Recall) y Puntuación F1 (F1-Score).
5.  **Análisis de Componentes Principales (PCA):** Se aplicó PCA como técnica de reducción de dimensionalidad para visualizar la varianza explicada por los componentes principales.

