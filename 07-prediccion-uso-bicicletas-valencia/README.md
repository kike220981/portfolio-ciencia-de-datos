# 🚴 Proyecto Integral de Ciencia de Datos: Análisis y Predicción de Uso de Bicicletas

Este repositorio contiene la implementación completa de un proyecto de **Ciencia de Datos** y **Machine Learning** que sigue todas las etapas del ciclo de vida de un análisis de datos, desde la exploración inicial hasta el modelado supervisado y no supervisado.

El objetivo es analizar y modelar patrones en el **uso de bicicletas** (probablemente en una red de estaciones o un sistema de *bike-sharing*).

## 🚀 Flujo de Trabajo del Proyecto

El proyecto está organizado en una secuencia lógica de *notebooks* que corresponden a las fases de la metodología CRISP-DM (o similar):

| Archivo | Fase | Objetivo Principal |
| :--- | :--- | :--- |
| `2_eda.ipynb` | **Análisis Exploratorio de Datos (EDA)** | Comprender la estructura de los datos, identificar valores atípicos (*outliers*) y faltantes, y diagnosticar la calidad inicial de la información. |
| `3_visualizacion.ipynb` | **Visualización de Datos** | Generar gráficos (Histogramas, Boxplots) y matrices de correlación (Heatmaps) para descubrir relaciones y patrones subyacentes entre las variables. 

[Image of a data correlation heatmap]
 |
| `5_transformacion.ipynb` | **Preprocesamiento y Transformación** | Preparar los datos para los modelos: **Codificación de variables categóricas** (`One-Hot Encoding`) y aplicación de técnicas de **escalado** (`MinMaxScaler` y `StandardScaler`) a las variables numéricas. |
| `6_clustering.ipynb` | **Aprendizaje No Supervisado** | Aplicar técnicas de **Clustering (K-Means)** para segmentar las estaciones o los patrones de uso en grupos con características comunes, sin una variable objetivo predefinida. |
| `7_supervisado.ipynb` | **Aprendizaje Supervisado** | Implementar y evaluar modelos de **Regresión** (ej. Regresión Lineal o Árboles de Decisión) para **predecir** el número de usos de bicicletas en función de las variables ambientales y temporales. |

***

## ⚙️ Tecnologías y Librerías

El proyecto utiliza las herramientas fundamentales de Python para el análisis y modelado de datos:

* **Análisis y Manipulación:** `pandas`, `numpy`.
* **Visualización:** `matplotlib`, `seaborn`.
* **Machine Learning (Scikit-learn):** Módulos para `preprocessing`, `cluster`, `linear_model` (Ridge/Lasso), `DecisionTreeRegressor`, y métricas de evaluación.
* **Reportes de EDA:** `pandas-profiling` y `dtale` (para informes detallados).

## 💡 Habilidades Demostradas

* Dominio del flujo de trabajo completo de la Ciencia de Datos.
* Capacidad para preparar datos desestructurados para el modelado.
* Experiencia en modelado supervisado (Regresión) y no supervisado (Clustering).
* Interpretación de coeficientes de regresión y métricas de *clustering* (como el **Silhouette Score**).

***

## 📦 Instrucciones de Ejecución

1.  **Clonar el Repositorio:**
    ```bash
    git clone [TU_URL_DEL_REPOSITORIO]
    ```
2.  **Instalar Dependencias:**
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn pandas-profiling dtale
    ```
3.  **Ejecutar los Notebooks:**
    Asegúrate de que el archivo de datos (`usobici.csv` o similar) esté en la ubicación correcta y luego ejecuta los archivos `.ipynb` en orden numérico (del 2 al 7) para seguir el proceso completo.
