# Churn_prediction
Una compañía de telecomunicaciones busca optimizar la retención de clientes mediante la identificación de aquellos con mayor probabilidad de cancelar el servicio (Churn). El objetivo de este proyecto es depurar y preparar un conjunto de datos para entrenar un modelo de predicción de Churn.


> **Análisis del gráfico de distribución de características de los features con respecto al Churn, podemos concluir que algunas variables no aportan mucho valor al modelo, debido a que es indiferente al valor que resulte, puede salir un Churn 0 ó Churn 1. No nos da un resultado claro. Estas variables son: telefono.servicio_telefono, telefono.varias_lineas_si y telefono.varias_lineas_sin servicio de telefono.**

![](https://github.com/juanmijael-salazar/Churn_prediction/blob/main/images/Captura%20de%20pantalla%202025-01-05%20200752.png)


> **Verificando la correlación entre las variables seleccionadas. Consideramos que nuestro modelo puede mejorar solo considerando estas variables. Se debe tener en cuenta que si nuestro modelo mejora o se mantiene en accuracy, también sería positivo, ya que con menos variables, se esta consiguiendo los mismo valores, y esto es beneficioso en términos de producción.**

![](https://github.com/juanmijael-salazar/Churn_prediction/blob/main/images/Captura%20de%20pantalla%202025-01-05%20200907.png)


>**Hemos observado que hemos obtenido mejores resultados con nuestra data desbalanceada, de acuerdo a nuestro análisis desarrollado en las partes iniciales.**

>**Se han considerado tres métricas para evaluar nuestros modelos, para todas las técnicas utilizadas. Estas métricas son: Accuracy, F1-score y time de entrenamiento modelo.**

>**El tiempo de ejecución del entrenamiento es importante por si se requiere escalar el proyecto. Por ejemplo si queremos trabajar con data real, que nos ingresa continuamente, ya que cada cierto periodo de tiempo se requerirá reentrenar el modelo, y de acuerdo a la cantidad de datos, consideramos que este aspecto es muy importante.**

![](https://github.com/juanmijael-salazar/Churn_prediction/blob/main/images/Captura%20de%20pantalla%202025-01-05%20201026.png)

**CONCLUSIONES:**
>Ambos modelos, SelectKBest y PCA, presentan altos valores en las métricas de entrenamiento, mientras que en las métricas de prueba se observa una notable diferencia. Esto indica una posible tendencia al sobreajuste, donde los modelos están aprendiendo de manera más efectiva solo de los datos de entrenamiento, pero no se desempeñan bien con datos nuevos.

>Necesidad de Más Evaluación: Para incrementar aún más los valores de las métricas, sería beneficioso recopilar más información o evaluar características adicionales. Esto podría ayudar a enriquecer el modelo y mejorar su capacidad de generalización.


[Ver completo...](https://github.com/juanmijael-salazar/Churn_prediction/blob/main/Churn_Conclusiones.ipynb)
