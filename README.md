# Análisis de Rendimiento Estudiantil con Machine Learning

Este proyecto corresponde a la **Evaluación Parcial 1** de la materia **Procesamiento de Aprendizaje Automático** (2º Año - Tecnicatura Superior en Ciencia de Datos e IA). El objetivo es predecir el desempeño académico en matemáticas de un grupo de estudiantes basándose en factores demográficos y socioeconómicos.

## Contenido del Proyecto
El análisis se divide en dos grandes bloques:
1. **Teórico-Conceptual**: Definiciones de tipos de aprendizaje, métricas de evaluación y manejo de Overfitting/Underfitting.
2. **Práctica en Python**: Implementación de un flujo completo de Ciencia de Datos (EDA, Preprocesamiento, Modelado y Evaluación).

## El Dataset
Se utilizó el **Students Performance Dataset**, que contiene información sobre:
* **Variables Categóricas**: Género, etnia, nivel educativo de los padres, tipo de almuerzo y curso de preparación.
* **Variables Numéricas**: Puntajes en Lectura, Escritura y **Matemáticas (Variable Objetivo)**.

## Tecnologías Utilizadas
* **Lenguaje**: Python 3.x
* **Librerías**: 
    * `Pandas` y `Numpy` para manipulación de datos.
    * `Scikit-Learn` para el modelado y métricas.
    * `Matplotlib` y `Seaborn` para visualizaciones.

## Metodología y Modelo
Se implementó un modelo de **Regresión Lineal** mediante un `Pipeline` que incluye:
1.  **Preprocesamiento**: Transformación de variables categóricas mediante `OneHotEncoder`.
2.  **División de datos**: 80% entrenamiento y 20% prueba.
3.  **Entrenamiento**: Ajuste del regresor para predecir el `math score`.

## Resultados y Métricas
El modelo demostró un desempeño sólido con los siguientes resultados:

* **MAE (Error Absoluto Medio)**: 4.21 pts.
* **RMSE (Raíz del Error Cuadrático Medio)**: 5.39 pts.
* **R² Score**: **0.88** (El modelo explica el 88% de la variabilidad de las notas).

### Visualización de Predicciones
![Predicciones vs Reales](https://github.com/mnahuelanca/students-performance-PML1/blob/master/grafico.png)

*(Nota: El gráfico muestra una fuerte correlación lineal, validando la eficacia del modelo para este problema).*
