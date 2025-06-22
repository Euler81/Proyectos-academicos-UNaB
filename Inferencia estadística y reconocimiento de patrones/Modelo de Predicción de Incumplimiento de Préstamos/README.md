# 🏦 Modelo de Predicción de Incumplimiento de Préstamos

## 📋 Descripción del Proyecto

Este proyecto busca desarrollar un modelo de machine learning para predecir la probabilidad de que un cliente incumpla con el pago de un préstamo. Utilizando un conjunto de datos bancarios, se aplicaron diversos algoritmos de clasificación para identificar a los clientes que pagarán (`paid = 1`) frente a los que no pagarán (`paid = 0`).

⚠️ Un desafío central fue el **fuerte desbalance de clases**: la mayoría de los préstamos fueron pagados.

Este trabajo fue desarrollado como parte del primer parcial de la asignatura **Inferencia Estadística y Reconocimiento de Patrones**.

* 🎓 **Universidad:** Universidad Nacional Guillermo Brown (UNaB)  
* 📚 **Asignatura:** Inferencia Estadística y Reconocimiento de Patrones  
* 👨‍🏫 **Profesor:** Sebastian Simondi  


### 👥 Integrantes del Equipo

* 👨‍💻 Lucas León González  
* 👨‍💻 David Lobos  
* 👨‍💻 Euler Diego  

---

## 🎯 Objetivos

1. 🛠️ **Implementar** un rango de algoritmos de clasificación para predecir el incumplimiento de pago.  
2. 📊 **Evaluar** el rendimiento de cada modelo a través de métricas y matrices de confusión.  
3. 🔍 **Identificar** fortalezas y debilidades de cada modelo y proponer mejoras.  

---

## 🗂️ Dataset

Se utilizó el conjunto de datos `Clasificación banco.csv`, que contiene información sobre préstamos y clientes.

- 🎯 **Variable Objetivo:** `paid` (0 = No Pagado, 1 = Pagado)  
- 🧾 **Características:** Incluyen variables numéricas (`credit.policy`, `int.rate`, `installment`, `log.annual.inc`, etc.) y categóricas (`purpose`)



---

## 🔄 Metodología y Flujo de Trabajo

1. 📈 **Análisis Exploratorio de Datos (EDA):** Visualización de distribuciones y correlaciones  
2. 🧹 **Preprocesamiento:**  
   * ✳️ One-Hot Encoding de `purpose`  
   * 🔀 División de datos en entrenamiento (70%) y prueba (30%)  
   * 📐 Estandarización con `StandardScaler`  
3. 🤖 **Entrenamiento de Modelos:**  
   - Regresión Logística  
   - K-Nearest Neighbors (KNN)  
   - Árbol de Decisión 🌳  
   - Random Forest 🌲  
   - LDA / QDA  
   - SVM  
   - Naive Bayes  
4. 🧪 **Evaluación:**  
   - Matrices de Confusión  
   - Métricas: **Precision**, **Recall**, **F1-Score**  

