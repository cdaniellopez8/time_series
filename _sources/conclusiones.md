# **Conclusiones**

<div style="text-align: justify;">

## Utilidad en la toma de decisiones

Las TCN (Temporal Convolutional Networks) son especializadas en series temporales, capturando eficientemente patrones recurrentes y estacionalidades en datos de $NO_2$ superan a métodos tradicionales como RNN o LSTM, evitando problemas de pérdida de información en largos periodos. Manejan de manera efectiva no linealidades, lo que las hace ideales para relaciones complejas entre $NO_2$, tráfico y clima. Además, integran fácilmente variables externas, como meteorología o eventos especiales, mejorando la precisión de las predicciones. Estas características las hacen muy útiles para predecir contaminación, facilitando decisiones ambientales rápidas y precisas.


## Conclusión y trabajos futuros

Los residuales del modelo son aproximadamente normales, aunque se observa la presencia de valores atípicos según el QQ-Plot. Se detecta una falta de independencia en los residuales, evidenciada por una autocorrelación significativa en los gráficos ACF/PACF. A pesar de esto, el modelo presenta un buen desempeño general, con un RMSE bajo de 0.005 y un MAPE de 14.33%. Para mejorar la independencia de los residuales, es necesario ajustar la estructura del TCN, considerando cambios en el tamaño del kernel o la adición de capas adicionales. También se recomienda incluir variables adicionales, como tráfico, clima o eventos, o explorar modelos híbridos para resolver la autocorrelación. Una opción prometedora es combinar TCN con modelos como ARIMA o GARCH, lo que podría mejorar la independencia de los residuales y el rendimiento general del modelo

</div>

```{tableofcontents}
```
