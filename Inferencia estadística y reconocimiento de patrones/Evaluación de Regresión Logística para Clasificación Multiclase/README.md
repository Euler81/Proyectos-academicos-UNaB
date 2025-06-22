# 🚀 Proyecto: Evaluación de Regresión Logística para Clasificación Multiclase

## 📝 Resumen del Proyecto

Este proyecto evalúa la efectividad de un modelo de **Regresión Logística** para un problema de clasificación multiclase. El objetivo es analizar su rendimiento, identificar sus limitaciones y determinar si es un modelo viable para el dataset proporcionado. El análisis revela un desempeño desigual, con el modelo mostrando un fuerte sesgo hacia una de las clases.

Este trabajo fue desarrollado para el **Parcial N°2** de la asignatura.

---

## 🎓 Información Académica

* **Universidad:** Universidad Nacional Guillermo Brown (UNaB)
* **Asignatura:** Inferencia estadística y reconocimiento de patrones
* **Profesor:** Sebastian Simondi

### 🧑‍💻 Integrantes del Equipo
* Lucas León González
* David Lobos
* Euler Diego

---

## 📊 Dataset: `regresion.csv`

El conjunto de datos utilizado contiene 154 registros y 5 columnas, donde el objetivo es predecir la variable `clase`.

* **Características (Features):**
    * `duracion`: Duración medida en tiempo (Float).
    * `paginas`: Número de páginas visitadas (Integer).
    * `acciones`: Número de acciones realizadas (Integer).
    * `valor`: Puntuación o valor numérico (Integer).
* **Variable Objetivo (Target):**
    * `clase`: Categoría a predecir, con 3 posibles valores: **Clase 0, Clase 1 y Clase 2**.

---

## ⚙️ Metodología Aplicada

El flujo de trabajo se estructuró en los siguientes pasos clave:

1.  **Análisis Exploratorio:** Carga e inspección inicial del dataset para entender su estructura y estadísticas descriptivas.
2.  **Preprocesamiento:**
    * Separación de variables predictoras (`X`) y la variable objetivo (`y`).
    * División de los datos en conjuntos de **entrenamiento (80%)** y **prueba (20%)**.
    * **Estandarización de características** con `StandardScaler` para normalizar los datos y mejorar el rendimiento del modelo.
3.  **Entrenamiento del Modelo:**
    * Implementación de un modelo de **Regresión Logística** configurado para clasificación multiclase (`multi_class='multinomial'`).
4.  **Evaluación de Rendimiento:**
    * Generación de predicciones sobre el conjunto de prueba.
    * Visualización de la **Matriz de Confusión** para analizar los aciertos y errores por clase.
    * Cálculo de métricas de rendimiento: **Precisión, Recall y F1-Score**.

