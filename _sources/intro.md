# **Proyecto final: Predicción de los niveles de $NO_2$ en el aire de Seúl mediante el modelo Temporal Convolutional Network (TCN)**

<div style="text-align: justify;">

El monitoreo de la calidad del aire es fundamental para comprender los efectos de la contaminación atmosférica en la salud pública y el medio ambiente. En este estudio, se aborda la predicción de los niveles de dióxido de nitrógeno ($NO_2$) en el aire de Seúl, Corea del Sur, utilizando datos de 1988 a 2021. Diversos enfoques, como modelos ARIMA, redes neuronales recurrentes (RNN), LSTM y transformers, han sido empleados para predecir contaminantes atmosféricos, incluyendo $NO_2$. Sin embargo, hasta la fecha no se han encontrado estudios han explorado el uso de redes convolucionales temporales (Temporal Convolutional Networks - TCN) para esta tarea. En este trabajo, se implementa un modelo TCN para predecir los niveles de $NO_2$, evaluando su capacidad para capturar dependencias temporales y realizar predicciones mas precisas. Los resultados muestran que el modelo TCN es capaz de identificar patrones complejos y no lineales en los datos históricos, superando a modelos tradicionales en términos de precisión. Este estudio destaca la efectividad de las TCN en la predicción de contaminantes atmosféricos y sugiere su potencial para mejorar la gestión de la calidad del aire a nivel global.


## Sobre los Datos:

Los datos utilizados en este estudio provienen del conjunto de datos histórico sobre la calidad del aire en Seúl, Corea del Sur desde 1988 hasta 2021. Este conjunto de datos contiene más de 5 millones de observaciones en diferentes puntos de medición por cada hora relacionadas con varios contaminantes atmosféricos tales como Ozono ($O_3$), PM2.5, PM10 y $SO_2$ y los niveles de dióxido de nitrógeno ($NO_2$) [Ver dataset aqui](https://www.kaggle.com/datasets/williamhyun/seoulairqualityhistoricdata/data). La variable de interés en este análisis es la concentración de $NO_2$, que se mide en partículas por millón [$ppm$]. Este conjunto de datos está estructurado en formato de serie temporal lo que facilita su uso para modelos de predicción basados en este tipo de datos. Los autores proporcionan acceso completo al conjunto de datos, permitiendo su replicación para futuras investigaciones y puede ser consultado en la bibliografía {cite}`seoul_air_quality`.


```{note}

El dióxido de nitrógeno ($NO_2$) es un contaminante atmosférico producido principalmente por la combustión de combustibles fósiles, incluyendo emisiones de vehículos y procesos industriales. Su presencia en el aire tiene efectos adversos tanto en la salud humana como en el medio ambiente {cite}`Stieb-21`. Exposiciones prolongadas a niveles elevados de $NO_2$ pueden agravar enfermedades respiratorias, reducir la función pulmonar y aumentar la susceptibilidad a infecciones respiratorias {cite}`Kashtan-24`. Además, este gas contribuye a la formación de ozono troposférico y partículas finas, amplificando los efectos de la contaminación del aire.
```

El análisis y predicción de la concentración de $NO_2$ en entornos urbanos es esencial para implementar políticas efectivas de control de la contaminación y mitigar sus impactos {cite}`de_Vries-24`. Para ello, se han desarrollado diversos modelos de series temporales que permiten analizar la evolución de las concentraciones de este contaminante y realizar predicciones a corto y largo plazo.

</div>

