# 🎓 Determinantes del Rendimiento Académico: Un Análisis de Variables Socioeconómicas

## 🏛️ UNaB: Universidad Nacional Guillermo Brown  
### 📘 Inferencia Estadística y Reconocimiento de Patrones  
#### 👨‍🏫 Profesor: Sebastián Simondi  
#### 👨‍🎓 Alumnos: Lucas León González, David Lobos, Euler Diego

---

## 📝 Descripción del Proyecto

Este proyecto tiene como objetivo analizar los factores que influyen en el rendimiento académico de los estudiantes, utilizando un enfoque basado en el análisis de variables socioeconómicas. Se exploran las relaciones entre características demográficas y socioeconómicas de los estudiantes y sus calificaciones en diversas asignaturas.

🔍 El análisis busca identificar patrones y determinantes clave que podrían explicar las diferencias en el desempeño estudiantil, proporcionando información valiosa para posibles intervenciones educativas o políticas de apoyo.

---

## 📊 Dataset

El dataset `exams.csv` contiene información detallada sobre **993 estudiantes** y su desempeño en asignaturas como matemáticas, física, química y álgebra.

### 🧮 Variables Incluidas:

- **📂 Variables Categóricas:**
  - 👤 `Género`
  - 🌍 `Raza/Etnicidad`
  - 🎓 `Nivel educativo de los padres`
  - 🍽️ `Almuerzo`
  - 🧑‍💼 `Empleo`
  - 📚 `Curso de preparación de exámenes`

- **📈 Variables Numéricas:**
  - ➕ `Notas en matemáticas`
  - 🧪 `Notas en física`
  - ⚗️ `Notas en química`
  - 🔢 `Notas en álgebra`
  - 📐 `Promedio` (calculado a partir de las notas de las asignaturas)

---

## 🧭 Metodología

Este proyecto sigue una metodología estructurada en las siguientes etapas:

1. **📥 Carga y Exploración Inicial de Datos**  
   Inspección general para detectar estructuras y anomalías.

2. **📊 Análisis Descriptivo**  
   Cálculo de estadísticas y exploración de distribuciones.

3. **📉 Visualización de Datos**  
   Uso de gráficos como histogramas, boxplots y countplots.

4. **⚙️ Ingeniería de Características:**
   - 🔄 *Codificación* de variables categóricas (One-Hot Encoding).
   - 🧮 *Cálculo del promedio* como métrica global de rendimiento.

5. **🧬 Análisis de Clústeres (K-Means):**
   - Agrupamiento por rendimiento promedio.
   - Método del "codo" para elegir número óptimo de clusters.
   - Caracterización socioeconómica de cada grupo.

6. **📚 Análisis del Curso de Preparación:**  
   Evaluación del impacto del curso en el rendimiento académico.



