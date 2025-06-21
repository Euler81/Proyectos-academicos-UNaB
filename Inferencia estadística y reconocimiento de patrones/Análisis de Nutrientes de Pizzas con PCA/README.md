# 🍕 Análisis de Nutrientes de Pizzas con PCA

Este proyecto analiza los componentes nutricionales de diferentes marcas de pizzas utilizando técnicas de análisis exploratorio y **Análisis de Componentes Principales (PCA)**. El objetivo es identificar patrones entre las marcas y determinar cuál ofrece un mejor perfil nutricional.

---

## 📊 Dataset

El conjunto de datos `Pizza.csv` incluye 300 observaciones con las siguientes variables:

- `brand`: Marca de la pizza (variable categórica)
- `id`: Identificador de muestra
- `mois`: Porcentaje de humedad
- `prot`: Cantidad de proteína por 100g
- `fat`: Cantidad de grasa por 100g
- `ash`: Cantidad de ceniza por 100g
- `sodium`: Cantidad de sodio por 100g
- `carb`: Cantidad de carbohidratos por 100g
- `cal`: Cantidad de calorías por 100g

---

## 🧪 Metodología

1. **Carga y limpieza de datos**
   - Revisión de valores nulos.
   - Conversión de tipos de datos si es necesario.

2. **Análisis Exploratorio de Datos (EDA)**
   - Visualización de distribuciones por marca.
   - Estadísticas descriptivas.

3. **Análisis de Componentes Principales (PCA)**
   - Estandarización de los datos.
   - Reducción de dimensiones.
   - Visualización de los componentes principales para encontrar agrupaciones de marcas.

4. **Visualización**
   - Diagramas de dispersión.
   - Cargas de las variables en los componentes.
   - Identificación de marcas con perfiles similares.

---

## 🔍 Objetivos

- Reducir la dimensionalidad del dataset manteniendo la mayor varianza posible.
- Detectar agrupaciones o patrones ocultos entre las marcas de pizza.
- Determinar qué variables (nutrientes) son más determinantes en la diferenciación entre marcas.

---

## 🛠️ Herramientas utilizadas

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Scikit-learn

---

## 📈 Resultados esperados

- Visualización clara de cómo se agrupan las marcas de pizza en función de su perfil nutricional.
- Interpretación de los ejes principales que explican la mayor parte de la variabilidad del conjunto de datos.
- Conclusiones sobre qué marca puede ser "mejor" desde el punto de vista nutricional.

---


## 📌 Notas

Este análisis es exploratorio y no pretende sustituir recomendaciones nutricionales profesionales. Se busca generar información útil para comprender mejor las diferencias nutricionales entre marcas.

---

