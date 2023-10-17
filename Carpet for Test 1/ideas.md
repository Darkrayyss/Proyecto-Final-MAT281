# Ideas para trabajar.

## Comentarios
- Para cada tarea, existen covariables relacionadas.
- Son 25 tareas, con 18 covariables cada una.
- Las clases están balanceadas.
- Parece ser que el problema principal será la reducción de features y de información.
- La normalidad de las variables es sumamente críticada.

## Problemas
- Tengo la hipótesis, de que en cada tarea las matrices de correlación son similares, pero no sé como probarla.

## Propuestas
- Utilizar PCA o algún método de selección de features para reducir la dimensionalidad.
- Hacer un essemble machine para modelos que se ajusten para cada tarea o utilizar algoritmos tipo adaboost. La idea es entrenar un algoritmo para cada tarea y luego de alguna forma combinar sus predicciones.
- Seguido con lo anterior, podría hacerse un análisis considerando las tareas por separado.
- Para cada tarea, el modelo debe identificar aquellos pares de alta colinearidad y botar aquel con menos información mutua con la variable objetivo, dado eso, se debe entregar un arból de clasificación. Generar un bosque para predecir.