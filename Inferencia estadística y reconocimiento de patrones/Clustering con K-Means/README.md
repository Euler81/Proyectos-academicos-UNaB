# 🧠 Proyecto de Clustering con K-Means


## 📚 Descripción del Proyecto 

Este proyecto tiene como objetivo explorar, analizar y agrupar un conjunto de datos tridimensional (X, Y, Z) mediante técnicas de aprendizaje no supervisado, específicamente el algoritmo **K-Means**. Además, se utiliza **Análisis de Componentes Principales (PCA)** para reducir la dimensionalidad y facilitar la visualización de los clusters.

---

## 📁 Dataset

El dataset utilizado es `kmeans.csv`, que contiene:

| Columna | Tipo de Dato | Descripción           |
|--------|--------------|-----------------------|
| X      | `float64`    | Dimensión X            |
| Y      | `float64`    | Dimensión Y            |
| Z      | `float64`    | Dimensión Z            |

- **Total de registros:** 100 entradas
- **Preprocesamiento:** Eliminación de duplicados, valores nulos y detección/remoción de outliers.

---

## 🔍 Análisis Exploratorio de Datos (EDA)

- **Histogramas:** Se observó sesgo en las variables X y Z, mientras que Y mostró una distribución simétrica cercana a cero.
- **Boxplots:** Se detectaron valores atípicos y se eliminaron utilizando el método del rango intercuartílico (IQR).
- **Correlaciones:**
  - Fuerte correlación negativa entre X e Y.
  - Débil correlación positiva entre X-Z y Y-Z.

---

## 📊 Reducción de Dimensionalidad con PCA

- Se aplicó **PCA** manteniendo las 2 primeras componentes principales.
- Estas dos componentes explican aproximadamente el **90% de la varianza total**, lo cual permite simplificar el análisis sin perder gran parte de la información.

---

## 🧮 Agrupamiento con K-Means

- **Método del Codo:** Se determinó que el número óptimo de clusters es **4**.
- **Visualización:** Los clusters fueron graficados en el espacio reducido por PCA, mostrando una buena separación entre grupos.

---

## 📈 Visualizaciones Incluidas

- Histogramas de cada variable
- Diagramas de caja (boxplots)
- Heatmap de correlaciones
- Gráfico del método del codo
- Scatter plot de los clusters resultantes

---

## 🛠️ Herramientas y Librerías Utilizadas

- **Python** 🐍
- **Pandas** 📊: Para manipulación de datos
- **NumPy** 🧮: Operaciones numéricas
- **Matplotlib & Seaborn** 🎨: Visualizaciones
- **Scikit-learn** 🤖: Algoritmos de ML y PCA
- **Jupyter Notebook** 📘: Entorno de desarrollo interactivo

