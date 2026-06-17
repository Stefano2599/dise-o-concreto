# Predicción de la Resistencia a la Compresión del Concreto mediante Ciencia de Datos

## Integrantes

- Stefano Anderson Lazarte Villafan
  
Docente: Kurt Soncco

---

# 1. Descripción del Problema

## Contexto

En ingeniería estructural, la resistencia a la compresión del concreto es una de las propiedades mecánicas más importantes para el diseño y evaluación de estructuras. Esta propiedad determina la capacidad del concreto para soportar cargas sin fallar.

Tradicionalmente, la resistencia se determina mediante ensayos de laboratorio realizados sobre probetas sometidas a compresión. Sin embargo, estos ensayos requieren tiempo, materiales y recursos económicos.

El uso de técnicas de Ciencia de Datos permite desarrollar modelos predictivos capaces de estimar la resistencia del concreto a partir de las características de su composición, reduciendo tiempos de evaluación y apoyando la toma de decisiones en proyectos de ingeniería.

## Problema de Ingeniería

¿Cómo predecir la resistencia a la compresión del concreto utilizando las proporciones de sus materiales constituyentes y la edad de curado mediante técnicas de Ciencia de Datos?

---

# 2. Objetivos

## Objetivo General

Desarrollar un modelo predictivo que estime la resistencia a la compresión del concreto utilizando variables relacionadas con su composición y edad.

## Objetivos Específicos

- Analizar las características del conjunto de datos.
- Identificar las variables que influyen en la resistencia del concreto.
- Aplicar técnicas de análisis exploratorio de datos.
- Construir modelos predictivos utilizando algoritmos de Machine Learning.
- Evaluar el desempeño de los modelos mediante métricas estadísticas.
- Interpretar los resultados obtenidos para su aplicación en ingeniería estructural.

---

# 3. Dataset Seleccionado

## Nombre del Dataset

Concrete Compressive Strength Dataset

## Fuente

UCI Machine Learning Repository

https://archive.ics.uci.edu/dataset/165/concrete+compressive+strength

## Descripción

El dataset contiene información sobre diferentes mezclas de concreto y la resistencia a la compresión obtenida para cada una de ellas.

La base de datos fue desarrollada por Yeh (1998) y es ampliamente utilizada para investigaciones relacionadas con predicción de propiedades mecánicas del concreto.

## Características del Dataset

- Número de registros: 1030
- Número de variables de entrada: 8
- Número de variable objetivo: 1
- Tipo de datos: Numéricos continuos

---

# 4. Variables

| Variable | Unidad |
|-----------|---------|
| Cemento | kg/m³ |
| Escoria de alto horno | kg/m³ |
| Ceniza volante | kg/m³ |
| Agua | kg/m³ |
| Superplastificante | kg/m³ |
| Agregado grueso | kg/m³ |
| Agregado fino | kg/m³ |
| Edad del concreto | días |

## Variable Objetivo

| Variable | Unidad |
|-----------|---------|
| Resistencia a la compresión | MPa |

---

# 5. Metodología

## Etapa 1: Recolección de Datos

Obtención del dataset desde el repositorio UCI Machine Learning Repository.

## Etapa 2: Exploración de Datos

- Verificación de valores faltantes.
- Estadísticas descriptivas.
- Análisis de correlación.
- Visualización de distribuciones.

## Etapa 3: Preprocesamiento

- Limpieza de datos.
- Estandarización de variables.
- División en conjuntos de entrenamiento y prueba.

## Etapa 4: Modelado

Se evaluarán distintos algoritmos de Machine Learning:

- Regresión Lineal
- Random Forest
- Gradient Boosting
- XGBoost (opcional)

## Etapa 5: Evaluación

Métricas consideradas:

- MAE (Mean Absolute Error)
- MSE (Mean Squared Error)
- RMSE (Root Mean Squared Error)
- R² Score

---

# 6. Aplicación del Marco PCS

## Predictibilidad

La resistencia del concreto depende directamente de la cantidad y proporción de sus componentes, así como de la edad de curado.

Debido a la existencia de relaciones físicas y químicas conocidas entre estas variables, se espera que los modelos predictivos alcancen niveles aceptables de precisión.

---

## Computabilidad

El dataset contiene únicamente 1030 observaciones y 8 variables explicativas.

Esto permite procesar los datos eficientemente utilizando herramientas de análisis como:

- Python
- Pandas
- NumPy
- Scikit-Learn

Los requerimientos computacionales son bajos y pueden ejecutarse en computadoras personales.

---

## Estabilidad

La estabilidad del modelo será evaluada mediante:

- Validación cruzada.
- Comparación entre diferentes algoritmos.
- Sensibilidad ante cambios en los datos de entrenamiento.
- Evaluación de la importancia de variables.

El objetivo es garantizar que pequeñas variaciones en los datos no generen cambios significativos en las predicciones.

---

# 7. Herramientas Utilizadas

- Python 3.x
- Jupyter Notebook
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Git
- GitHub

---

# 8. Estructura del Proyecto

```
Proyecto-Concreto/
│
├── README.md
│
├── data/
│   └── Concrete_Data.csv
│
├── notebooks/
│   └── analisis_exploratorio.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── training.py
│   └── evaluation.py
│
├── informe/
│   └── Informe_Inicial.docx
│
└── results/
    ├── graficos/
    └── modelos/
```

---

# 9. Resultados Esperados

Se espera desarrollar un modelo predictivo que permita estimar la resistencia a la compresión del concreto con un nivel de precisión adecuado para apoyar procesos de análisis y toma de decisiones en proyectos de ingeniería estructural.

---

# 10. Referencias

- Yeh, I. C. (1998). Modeling of Strength of High-Performance Concrete Using Artificial Neural Networks.
- UCI Machine Learning Repository. Concrete Compressive Strength Dataset.
- Yu, B., & Barter, R. (2024). Veridical Data Science (PCS Framework).
