# Proyecto de Inteligencia Artificial - Modelo Predictivo de Dolor Lumbar

Este proyecto tiene como objetivo desarrollar un modelo predictivo de dolor lumbar a partir de datos biomecánicos de la columna lumbar y pelvis, utilizando técnicas de Machine Learning en Python. El enfoque combina conocimiento clínico en fisioterapia con análisis de datos para facilitar la identificación temprana de pacientes con alteraciones lumbares.

## Contenido

- `Proyecto_final_IA_DavidPradosMedina.pdf`: Documento completo del proyecto con explicaciones, métricas, visualizaciones y conclusiones.
- `Dataset_spine.csv`: Dataset utilizado para el entrenamiento de los modelos.
- `Proyecto_final_IA_DavidPradosMedina.ipynb`: Notebook con el EDA, ingeniería de características, entrenamiento y evaluación de los modelos.
- `README.md`: Este archivo, con el resumen del proyecto y las tecnologías utilizadas.

## Objetivos del proyecto

- Analizar datos biomecánicos de la columna vertebral y la pelvis.
- Identificar variables relevantes asociadas al dolor lumbar.
- Desarrollar un modelo predictivo capaz de clasificar pacientes como "Normal" o "Abnormal".
- Comparar distintos algoritmos de Machine Learning.
- Evaluar el rendimiento de los modelos mediante métricas de clasificación.
- Explorar la aplicabilidad clínica del modelo en fisioterapia.

## Dataset

Se ha utilizado el dataset `Dataset_spine.csv`, compuesto por:

- 310 observaciones
- 12 variables numéricas biomecánicas y morfológicas.
- 1 variable objetivo-binaria ("Normal" o "Abnormal")

Variables biomecánicas principales:

- Incidencia pélvica
- Inclinación pélvica
- Ángulo de lordosis lumbar
- Pendiente sacra
- Radio pélvico
- Grado de espondilolistesis
- Inclinaciones cervicales, torácicas y escoliosis etc...

## Tecnologías utilizadas

*Lenguaje de programación*: 

- Python 3.

*Análisis y manipulación de datos*:

- Pandas.
- Numpy.

*Visualización de los datos*:

- Matplotlib.
- Seaborn.

*Machine Learning*:

- Scikit-Learn.
    - Random Forest Classifier.
    - Logistic Regression.
    - Métricas de evaluación (accuracy, precision, recall, F1-score).

*Entorno de desarrollo*: 

- Google Colab.

*Control de versiones*:

- Git y GitHub.


## Arquitectura del proyecto

El proyecto se ha dividido en las siguientes fases:

### 1. Entendimiento del negocio

- Definición del caso de uso desde una perspectiva clínica.
- Identificación de los objetivos del negocio y los beneficios esperados.

### 2. Entendimiento de los datos (EDA)

- Preparación de los datos.
- Análisis descriptivo de las diferentes variables.
- Estudio de distribuciones y valores atípicos.
- Análisis de correlaciones entre variables biomecánicas.
- Identificación de variables clave relacionadas con alteraciones lumbares.

### 3. Preparación de los datos (Ingeniería de características)

- Codificación de la variable objetivo.
- Creación de nuevas variables relevantes (ratios biomecánicos y banderas de outliers).
- Eliminación de variables redundantes para reducir el ruido.
- Preparación del dataset para el entrenamiento de los modelos.

### 4. Modelado

- Entrenamiento de un modelo *Random Forest*.
- Entrenamiento de un modelo de *Regresión logística*.

### 5. Evaluación

Evaluación y comparativa de las siguientes métricas de los dos algoritmos:

- Accuracy.
- Precision.
- Recall.
- F1-score.
- Matrices de confusión.

## Conclusión

El proyecto evidencia que es posible predecir la presencia de alteraciones lumbares que provoquen a su vez dolor lumbar, a través de medidas biomecánicas. La regresión logística, por su simplicidad y capacidad de interpretación, parece ser más adecuada para aplicaciones clínicas donde la  predicción es la clave para el éxito del modelo. Sin embargo, Random Forest sigue  siendo útil para interpretar interacciones más complejas y evaluar la relevancia de  las variables. 
Como posible mejora, un dataset más amplio con mayor número de  observaciones, especialmente de la clase “Normal”, podría mejorar la capacidad  de predicción y permitir desarrollar un modelo predictivo de mayor calidad. 
Este enfoque combina conocimiento clínico y técnicas de Machine Learning,  proporcionando una herramienta potencial para la identificación temprana de pacientes con riesgo de dolor lumbar y apoyando la toma de decisiones del  fisioterapeuta. 

---

**Autor:** David Prados Medina 
**Curso:** Certificado de Big Data & IA - UAX 2026  
