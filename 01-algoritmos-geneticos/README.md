# 🧬 Optimización con Algoritmos Genéticos (GA)

Este proyecto implementa Algoritmos Genéticos (GA) utilizando la librería **PyGAD** en Python para resolver dos problemas de optimización fundamentales, demostrando la capacidad de esta técnica para encontrar soluciones aproximadas a problemas complejos.

## 📁 Estructura del Proyecto

El análisis y la implementación se encuentran en el archivo:
* `EnriqueSanchezAntuña_AlgoritmosGeneticos_A2.ipynb`

## 🚀 Problemas Resueltos

### 1. Problema de la Mezcla de Ingredientes Óptima

Este problema busca determinar las dosis óptimas de cuatro ingredientes clave en una bebida energética (Cafeína, Azúcar, Taurina y Vitaminas) para alcanzar un rendimiento energético ideal de **300**.

* **Variables (Genes):** Dosis de Cafeína, Azúcar, Taurina y Vitaminas (valores reales).
* **Fórmula del Rendimiento:** El rendimiento ($E$) se calcula mediante la función objetivo:
    $$E = 2C + 1A + 3T + 2V$$
* **Objetivo:** Minimizar la diferencia entre el rendimiento calculado y el rendimiento ideal.
* **Función de Aptitud (Fitness):** Se maximiza la inversa del error absoluto para penalizar las desviaciones del objetivo:
    $$\text{Fitness} = \frac{1}{|E - 300| + \epsilon}$$
    *Resultado Típico: Una combinación de ingredientes que logra un rendimiento muy cercano a $300.00$.*

### 2. Problema de la Mochila (Knapsack Problem)

Se aborda el problema clásico de la mochila, donde el objetivo es seleccionar un subconjunto de 10 productos (cada uno con un peso y un valor) para maximizar el valor total sin exceder la **capacidad máxima de 15 kg**.

* **Variables (Genes):** 10 genes binarios (0 o 1), donde 1 significa que el producto está incluido.
* **Restricción Clave:** El peso total de los productos seleccionados no debe exceder $15 \text{ kg}$.
* **Función de Aptitud (Fitness):**
    * Si el peso total $\leq 15 \text{ kg}$, el fitness es igual al **Valor Total** de los productos seleccionados.
    * Si el peso total $> 15 \text{ kg}$, el fitness se penaliza a **0**.
    *Resultado Típico: Se obtiene el conjunto de productos con el máximo valor posible dentro del límite de peso.*

## 🛠️ Tecnologías y Librerías

* **Python 3.x**
* **PyGAD:** Framework de código abierto para la implementación de Algoritmos Genéticos.
* **NumPy:** Utilizado para la realización de cálculos numéricos eficientes.

## ⚙️ Parámetros del Algoritmo Genético

| Parámetro | Problema 1 (Ingredientes) | Problema 2 (Mochila) |
| :--- | :--- | :--- |
| **Número de Genes** | 4 | 10 |
| **Tamaño de Población** | 100 | 100 |
| **Número de Generaciones** | 100 | 200 |
| **Porcentaje de Mutación** | 10% | 10% |

## 📦 Ejecución

Para ejecutar y replicar el proyecto, sigue estos pasos:

1.  **Instalar dependencias:**
    ```bash
    pip install pygad numpy
    ```
2.  **Abrir el Notebook:**
    Ejecuta el archivo `EnriqueSanchezAntuña_AlgoritmosGeneticos_A2.ipynb` en un entorno compatible (como Jupyter, Colab o VS Code) y ejecuta las celdas en orden.
