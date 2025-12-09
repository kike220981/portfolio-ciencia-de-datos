# 🏘️ Predicción de Precios de Vivienda (Regresión)

Este proyecto aborda un problema de regresión clásico: la predicción del precio final de venta de viviendas, basándose en múltiples características descriptivas.

## 🎯 Enfoque del Proyecto

El proceso sigue un ciclo completo de Machine Learning:

1.  **Exploración y Preprocesamiento de Datos:**
    * Manejo y imputación de valores faltantes (NaN).
    * Identificación y tratamiento de *outliers*.
    * Codificación de variables categóricas (One-Hot Encoding, Label Encoding).
2.  **Feature Engineering:** Transformación de variables y, potencialmente, la creación de nuevas características para optimizar la capacidad predictiva del modelo.
3.  **Modelado:** Aplicación y entrenamiento de modelos de regresión avanzados (como modelos lineales regularizados, o métodos de *ensemble* como Gradient Boosting).

## 📉 Métrica de Evaluación

La precisión del modelo se evalúa utilizando la métrica estándar para este tipo de problemas:

* **RMSE (Root Mean Square Error):** Mide la raíz cuadrada de la media de los errores al cuadrado. Un valor más bajo de RMSE indica una mejor precisión del modelo.

## 🛠️ Tecnologías

* Python
* Pandas (para manipulación de datos)
* NumPy (para cálculos numéricos)
* Scikit-learn (para preprocesamiento y modelos de regresión)
* Matplotlib / Seaborn (para visualización)
