# Cab_demand_forecasting_at_airports

La compañía Sweet Lift Taxi ha recopilado datos históricos sobre pedidos de taxis en los aeropuertos. Para atraer a más conductores durante las horas pico, necesitamos predecir la cantidad de pedidos de taxis para la próxima hora.

## Observaciones

Los datos históricos de pedidos de taxis en los aeropuertos fueron remuestreados por hora para estandarizar la resolución temporal, facilitando así el análisis de series temporales y la construcción de modelos predictivos. Este proceso aseguró una uniformidad en la granularidad de los datos, simplificando significativamente tanto el análisis como la predicción de la demanda de taxis.

El análisis inicial reveló una estructura temporal en los datos, con registros desde marzo hasta agosto de 2018. Se efectuó un remuestreo por hora para homogeneizar la resolución temporal, facilitando así el análisis y la predicción de la demanda de taxis. Se extrajeron estadísticas clave, como promedios y desviaciones estándar por hora y día de la semana, ofreciendo insights sobre los patrones de demanda. Las visualizaciones mostraron claramente las tendencias temporales y las variaciones en la demanda de taxis a lo largo del día y la semana.

En esta sección, se entrenó un modelo de regresión utilizando el algoritmo Random Forest. Se ajustaron algunos hiperparámetros, como el número de estimadores (100), la profundidad máxima del árbol (10) y la semilla aleatoria (12345). Estos ajustes pueden influir en la capacidad del modelo para capturar patrones complejos en los datos y generalizar bien a nuevos datos. El modelo entrenado se muestra con los hiperparámetros utilizados para su configuración.

En esta sección, se realizaron predicciones utilizando el modelo entrenado en el conjunto de prueba. Luego, se calculó el error cuadrático medio (MSE) entre las predicciones y las etiquetas reales del conjunto de prueba. Un error cuadrático medio (MSE) de 0.033 indica que, en promedio, las predicciones del modelo difieren en 0.033 unidades al cuadrado de las etiquetas reales en el conjunto de prueba. Dado que el MSE es una medida de la calidad de la predicción, un valor bajo indica que el modelo se ajusta bien a los datos de prueba y tiene una buena capacidad para generalizar a datos no vistos.

## Conclusión

Se realizó un análisis exploratorio de los datos para comprender mejor la distribución y las tendencias de la demanda de taxis a lo largo del tiempo. Los datos históricos de pedidos de taxis en los aeropuertos fueron remuestreados por hora para estandarizar la resolución temporal, facilitando así el análisis de series temporales y la construcción de modelos predictivos. Este proceso aseguró una uniformidad en la granularidad de los datos, simplificando significativamente tanto el análisis como la predicción de la demanda de taxis. Además, se entrenó un modelo de regresión utilizando el algoritmo Random Forest, ajustando algunos hiperparámetros para mejorar su desempeño. Las predicciones del modelo en el conjunto de prueba mostraron un error cuadrático medio (MSE) de 0.033, lo que indica un buen ajuste del modelo a los datos de prueba y una capacidad razonable para generalizar a datos no vistos.
