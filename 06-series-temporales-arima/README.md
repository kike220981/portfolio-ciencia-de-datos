# ⏳ Probabilidad y Estadística: Modelado y Predicción de Series Temporales (ARIMA)

Este proyecto, desarrollado en **R Markdown (.Rmd)**, implementa técnicas avanzadas de **análisis de series temporales** para identificar, modelar y predecir el comportamiento futuro de datos dependientes del tiempo.

## 🎯 Objetivo Principal

El objetivo es aplicar la metodología **ARIMA (Auto-Regressive Integrated Moving Average)** para modelar una serie temporal específica (probablemente económica o financiera) y realizar predicciones a corto plazo.

## 🧠 Metodología y Técnicas Aplicadas

El proyecto sigue la metodología estándar para el modelado de series temporales:

### 1. Preparación de la Serie Temporal
* **Transformación:** Conversión del conjunto de datos en un objeto de serie temporal (`ts`) en R.
* **Análisis Descriptivo:** Visualización y descomposición inicial para identificar tendencias, estacionalidad (si aplica) y residuos.

### 2. Identificación del Modelo ARIMA
* **Función de Autocorrelación (ACF) y Parcial (PACF):** Análisis de los correlogramas para identificar los órdenes iniciales $p$ (AR) y $q$ (MA).
* **Automatización:** Uso de la función `auto.arima` para la identificación automática del mejor modelo ARIMA no estacional y estacional, basado en criterios de información como **AIC** o **BIC**.

### 3. Estimación y Diagnóstico
* **Estimación de Parámetros:** Ajuste de varios modelos ARIMA (ej. `ARIMA(2,0,0)`) con componentes estacionales para encontrar el mejor ajuste.
* **Diagnóstico de Residuos:** Uso de la función `checkresiduals()` para verificar que los residuos del modelo sean ruido blanco (independientes, con media cero y varianza constante), una condición necesaria para la validez del modelo. 

### 4. Predicción (Forecasting)
* Se realiza una **predicción** a futuro (`forecast`) comparando los resultados de varios modelos (`M1`, `M3`, `Ma`, `E.Ma`) para determinar cuál ofrece la mejor proyección basada en métricas como el **LL (Log Likelihood)** o el **AIC**.

## 🛠️ Tecnologías y Librerías

* **R Language:** Lenguaje principal para el análisis estadístico.
* **R Markdown (.Rmd):** Para generar un informe reproducible que integra código, resultados y gráficos.
* **Librería `forecast`:** Esencial para las funciones de `auto.arima`, `checkresiduals`, `forecast` y `autolayer`.
* **Librería `tseries` o `xts`:** (Probablemente usada) Para la manipulación general de series temporales.

## 🚀 Instrucciones de Ejecución

1.  **Software:** Se requiere **R** y **RStudio**.
2.  **Librerías:** Instalar las librerías necesarias (principalmente `forecast`).
    ```R
    install.packages("forecast")
    ```
3.  **Ejecutar:** Abrir el archivo `ACT1_EV3_ENRIQUE_SANCHEZ_53529839F.Rmd` en RStudio y usar la función **Knit** (Generar) para compilar el código R y obtener el informe final.
