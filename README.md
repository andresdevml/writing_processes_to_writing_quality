Proyecto de Predicción de Calidad de Escritura

Objetivo: Desarrollar un modelo predictivo para evaluar la calidad de la escritura basándonos en la mecánica de la escritura.

Descripción del Proyecto:
Exploración de Datos y Preprocesamiento

Realizamos un análisis exhaustivo de las características de los datos para identificar cómo realizar un ingeniería de características que nos permita encontrar el mejor espacio de representación para la entrada del modelo. Este proceso se documenta en data_experimentation.ipynb.
Creación de Conjuntos de Datos

Una vez definidas las transformaciones, creamos conjuntos de datos para generar datos de prueba para los modelos.
Selección del Modelo

Elegimos un modelo de regresión convolucional en una dimensión para trabajar mejor con series temporales.
Optimización de Hiperparámetros

Seleccionamos los hiperparámetros del modelo a través de pruebas 'Human in the Loop', observando el comportamiento de las gráficas para la métrica de interés (RMSE) tanto en el conjunto de entrenamiento como en el conjunto de validación.
Evaluación del Modelo

Finalmente, probamos los modelos en el conjunto de prueba. Este procedimiento se llevó a cabo para el modelo base con una segmentación de datos 60/40. Luego, entrenamos el modelo para producción con la misma configuración de hiperparámetros que el modelo base, pero con una segmentación de datos 90/10.
