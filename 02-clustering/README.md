# 📊 Análisis y Evaluación de Algoritmos de Clustering

Este proyecto implementa y compara tres algoritmos fundamentales de Machine Learning no supervisado para segmentar un conjunto de datos, evaluando cuál ofrece la mejor estructura de agrupamiento.

## ⚙️ Algoritmos Implementados

Se aplican y contrastan los siguientes métodos de agrupamiento:

* **K-Means:** Algoritmo de partición que divide el espacio de datos en $K$ clústeres.
* **Clustering Jerárquico (Agglomerative Clustering):** Construcción de clústeres mediante una aproximación "bottom-up" (ascendente).
* **DBSCAN:** Algoritmo basado en densidad, eficaz para descubrir clústeres de formas arbitrarias y manejar ruido (outliers).

## 📈 Evaluación del Rendimiento

Para determinar la calidad de los clústeres formados por cada algoritmo, se utilizan métricas internas de validación:

* **Silhouette Score:** Mide qué tan bien está clasificado un objeto dentro de su propio clúster en comparación con otros clústeres. Cuanto más cerca de $1$, mejor.
* **Davies-Bouldin Index:** Evalúa el promedio de la similitud entre clústeres, donde una puntuación baja indica una mejor separación y clústeres más compactos.

## 🛠️ Tecnologías

* Python
* Scikit-learn (para los algoritmos de clustering y métricas)
* NumPy
* Matplotlib
