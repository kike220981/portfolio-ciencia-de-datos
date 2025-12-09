# 🧠 Inteligencia Artificial: Lógica Difusa y Clasificación Bayesiana

Este proyecto se centra en dos áreas clave de la Inteligencia Artificial: la creación de un sistema de **Lógica Difusa** para la toma de decisiones basada en imprecisión y la implementación de modelos de **Clasificación (Naive Bayes)** para el análisis de sentimientos.

## 1. ☁️ Sistema de Lógica Difusa: Satisfacción del Cliente

Se diseña un **Sistema de Inferencia Difusa** para estimar la **Satisfacción del Cliente** a partir de variables de entrada inciertas.

### 🎯 Objetivo

Estimar la satisfacción final de un cliente (salida) basándose en la **Calidad del Servicio** y el **Tiempo de Espera**.

### ⚙️ Componentes del Sistema

* **Variables de Entrada (Antecedentes):**
    * `Calidad del servicio` (rango 0-10)
    * `Tiempo de espera` (rango 0-30 minutos)
* **Variable de Salida (Consecuente):**
    * `Satisfacción del cliente` (Probablemente definida con términos como 'Baja', 'Media', 'Alta').
* **Fases Implementadas:**
    1.  **Fuzzificación:** Definición de los términos lingüísticos y sus **Funciones de Pertenencia** (triangulares, gaussianas, etc.) para cada variable.
    2.  **Inferencia:** Aplicación de un conjunto de reglas difusas (`IF (Calidad es Baja) AND (Espera es Larga) THEN (Satisfacción es Baja)`).
    3.  **Defuzzificación:** Conversión del conjunto difuso de salida en un valor numérico crisp (p. ej., un puntaje final de satisfacción).

## 2. 🗣️ Clasificación de Sentimiento con Naive Bayes

La segunda parte del *notebook* se enfoca en el procesamiento del lenguaje natural (NLP) para clasificar comentarios (análisis de sentimiento) utilizando modelos probabilísticos.

* **Objetivo:** Clasificar comentarios de texto como 'Positivos' o 'Negativos'.
* **Modelos Probados:** Se comparan diferentes variantes del algoritmo Naive Bayes:
    * **MultinomialNB**
    * **ComplementNB**
    * **GaussianNB**
    * **BernoulliNB**
* **Desafío Principal:** El análisis incluye una discusión sobre cómo el **desbalanceo del *dataset*** afecta negativamente el rendimiento de modelos como **GaussianNB** y **BernoulliNB**, haciéndolos predecir la clase mayoritaria.

## 🛠️ Tecnologías Utilizadas

* **Python 3.x**
* **Scikit-learn (sklearn):** Para la implementación de los clasificadores Naive Bayes y métricas.
* **Librería de Lógica Difusa:** Probablemente `scikit-fuzzy` o similar (aunque esto puede variar, la base es la lógica).
* **Pandas y NumPy:** Para la manipulación y el preprocesamiento de datos de texto.

## 🚀 Ejecución del Código

Para ejecutar y explorar los resultados:

1.  **Instalar dependencias:** Se requiere `scikit-learn`, `numpy`, `pandas` y posiblemente una librería de lógica difusa (como `scikit-fuzzy`).
    ```bash
    pip install numpy pandas scikit-learn [scikit-fuzzy si aplica]
    ```
2.  **Ejecutar el Notebook:** Abrir y ejecutar el archivo `Tema4_EnriqueSanchezAntuña.ipynb` en un entorno como Jupyter o VS Code.
