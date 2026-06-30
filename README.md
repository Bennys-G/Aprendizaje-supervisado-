# Aprendizaje-supervisado-
Proyecto de Machine Learning enfocado en predecir el abandono de clientes bancarios utilizando técnicas de clasificación supervisada. Se trabajó con datos de clientes, se aplicó preprocesamiento mediante pipelines, se trató el desbalance de clases. El modelo final alcanzó un F1-score de 0.616 y un AUC-ROC de 0.862 en el conjunto de prueba.
# Predicción de abandono de clientes bancarios

## Descripción del proyecto

Este proyecto de Machine Learning está enfocado en predecir el abandono de clientes bancarios utilizando técnicas de clasificación supervisada. El objetivo principal es identificar a los clientes con mayor probabilidad de dejar el banco, permitiendo que la institución pueda tomar acciones preventivas para mejorar la retención de clientes.

Durante el desarrollo del proyecto se trabajó con datos de clientes que incluyen información como edad, país, género, saldo bancario, número de productos contratados, actividad del cliente, salario estimado y si el cliente abandonó o no el servicio.

## Objetivo

Construir un modelo predictivo capaz de clasificar correctamente a los clientes que tienen riesgo de abandonar el banco, prestando especial atención al desbalance de clases presente en los datos.

## Tecnologías utilizadas

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
* Seaborn
* Jupyter Notebook

## Proceso del proyecto

El proyecto siguió un flujo completo de análisis y modelado de datos:

1. **Carga y exploración de datos**
   Se revisó la estructura del dataset, los tipos de variables, valores faltantes y la distribución de la variable objetivo.

2. **Preparación de datos**
   Se eliminaron columnas que no aportaban valor predictivo, como identificadores de cliente o datos personales. También se trataron variables categóricas y numéricas mediante pipelines de preprocesamiento.

3. **Análisis del desbalance de clases**
   Se identificó que la mayoría de los clientes permanecían activos, mientras que una menor proporción abandonaba el banco. Por esta razón, se utilizaron métricas más adecuadas que la exactitud, como F1-score y AUC-ROC.

4. **Entrenamiento de modelos**
   Se compararon diferentes modelos de clasificación, incluyendo Regresión Logística y Random Forest.

5. **Mejora del modelo**
   Se aplicaron técnicas para manejar el desbalance de clases, como el uso de pesos balanceados y ajuste del umbral de clasificación.

6. **Evaluación final**
   El modelo final fue evaluado en el conjunto de prueba para medir su capacidad de generalización.

## Modelos utilizados

* Regresión Logística
* Random Forest Classifier
* Modelo Dummy como referencia base

## Resultados

El mejor modelo fue un Random Forest ajustado para trabajar con clases desbalanceadas. En el conjunto de prueba, el modelo final obtuvo los siguientes resultados:

* **F1-score:** 0.616
* **AUC-ROC:** 0.862
* **Accuracy:** 0.854

Estos resultados muestran que el modelo tiene una buena capacidad para diferenciar entre clientes que probablemente abandonarán el banco y clientes que permanecerán activos.

## Conclusión

Este proyecto demuestra la importancia de utilizar métricas adecuadas cuando se trabaja con problemas de clasificación desbalanceada. Aunque la exactitud puede parecer alta, métricas como F1-score y AUC-ROC permiten evaluar mejor el desempeño del modelo en la clase de mayor interés: los clientes que abandonan el banco.

El modelo final logró superar la meta establecida de F1-score mayor a 0.59, por lo que puede considerarse una solución útil para apoyar estrategias de retención de clientes en el sector bancario.

## Posibles mejoras futuras

* Probar modelos adicionales como Gradient Boosting, XGBoost o CatBoost.
* Realizar una búsqueda más amplia de hiperparámetros.
* Analizar la importancia de variables para entender qué factores influyen más en el abandono.
* Implementar el modelo en una aplicación o dashboard interactivo.
* Actualizar el modelo con datos más recientes para mejorar su desempeño.
