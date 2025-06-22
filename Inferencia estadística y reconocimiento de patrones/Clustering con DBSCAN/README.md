# 🧠 Proyecto de Clustering con DBSCAN



## 📚 Descripción del Proyecto 

Este proyecto tiene como objetivo explorar, analizar y agrupar un conjunto de datos bidimensional (`x`, `y`) mediante técnicas de aprendizaje no supervisado, específicamente el algoritmo **DBSCAN**. Además, se utiliza **Análisis de Componentes Principales (PCA)** para reducir la dimensionalidad y facilitar la visualización de los clusters.

---

## 📁 Dataset

El dataset utilizado es `dbscan.xlsx`, que contiene:

| Columna | Tipo de Dato | Descripción           |
|--------|--------------|-----------------------|
| x      | `float64`    | Dimensión X            |
| y      | `float64`    | Dimensión Y            |

- **Total de registros:** 500 entradas
- **Preprocesamiento:** Eliminación de duplicados, valores nulos y detección/remoción de outliers.

---

## 🔍 Análisis Exploratorio de Datos (EDA)

- **Histogramas:**
  - La variable `x` muestra una distribución simétrica con ligera inclinación positiva.
  - La variable `y` también es simétrica, centrada cerca de 0.5.
- **Boxplots:**
  - Se detectaron algunos valores atípicos en ambas variables.
  - Ambas tienen dispersión comparable.
- **Correlación:**
  - Correlación negativa moderada entre `x` e `y`: **-0.43**.

---

## 📊 Reducción de Dimensionalidad con PCA

- Se aplicó **PCA** manteniendo las 2 primeras componentes principales.
- Estas dos componentes explican aproximadamente:
  - **PC1**: ~70% de la varianza
  - **PC2**: ~30% de la varianza  
  → Total acumulado: **~100%**

---

## 🧮 Agrupamiento con DBSCAN

- **Búsqueda de parámetros óptimos:**
  - `eps = 0.35`
  - `min_samples = 15`
- **Silhouette Score:** `0.34` (indicador de calidad de clustering)
- **Número de clusters identificados:** 2
- **Puntos clasificados como ruido:** Identificados y excluidos de los grupos finales.

---

## 📈 Visualizaciones Incluidas

- Histogramas de cada variable
- Diagramas de caja (boxplots)
- Heatmap de correlaciones
- Gráfico de varianza explicada por PCA
- Scatter plot de los clusters resultantes tras PCA

---

## 🛠️ Herramientas y Librerías Utilizadas

- **Python** 🐍
- **Pandas** 📊: Para manipulación de datos
- **NumPy** 🧮: Operaciones numéricas
- **Matplotlib & Seaborn** 🎨: Visualizaciones
- **Scikit-learn** 🤖: Algoritmos de ML, PCA y DBSCAN
- **Jupyter Notebook** 📘: Entorno de desarrollo interactivo

