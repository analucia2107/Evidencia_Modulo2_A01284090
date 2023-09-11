# Ana Lucía Cárdenas Pérez - A01284090

# MomentoRetro_Modulo2_A01284090
### Archivos para evaluar
* [Momento de Retroalimentación: Módulo 2 Uso de framework o biblioteca de aprendizaje máquina para la implementación de una solución. (Portafolio Implementación)](MomentoRetro_Modulo2_A01284090.ipynb) - Primeras implementaciones de los modelos vistos en clase donde se espera retroalimentación para corregir y mejorar el trabajo presentado.
* [Momento de Retroalimentación: Módulo 2 Análisis y Reporte sobre el desempeño del modelo. (Portafolio Análisis)](https://github.com/analucia2107/MomentoRetro_Modulo2_A01284090/blob/main/MometoRetro_Modulo2_AnalisisyReporte_A01284090.ipynb) - Primeras analisis de los modelos donde esperamos recibir retroalimentación para mejorar en nuestro análisis de la situación y del código implementdo.
* [Evidencia Modulo 2](Evidencia_Modulo2_A01284090.ipynb) - Implementación y análisis de un decision classification tree con los datos de iris.csv. Se encuentra el proceso, resultados y un análisis de los puntos más importantes y sus resultados.
* [README](README.md) - Este apartado incluye una descripción general del proyecto con los links para acceder a los códigos con los que fuimos trabajando durante el bloque.

# Portafolio de Implementación
## Descripción del modelo
El modelo a utilizar en este momento de retroalimentación es el "Decision Tree Classifier" es un modelo de aprendizaje automático que nos muestra en manera de un árbol con "raíz" (la parte más alta del gráfico), "ramas", y las "hojas" (la parte final o más baja del árbol). Se empieza con una sola pregunta y dependiendo de la respuesta, se va abriendo el árbol con ramas basándose en las características con las que se pueden responder las preguntas. Cada vez que se responde la pregunta, si por ejemplo la pregunta es ¿Tiene patas? y buscamos que el animal si tenga patas y el animal en la imagen no las tiene, al responder que no, el nodo va a abrirse con otra pregunta y se vuelve a dividir en grupos dependiendo la respuesta hasta llegar a las hojas, donde se van a asignar etiquetas basadas en las respuestas anteriores.

Este modelo guarda y analiza toda la información de preguntas y características para poder clasificar nuevos ejemplos en otros posibles archivos y así poder resolcer un problema de clasificación de una manera más sencilla y rápida por su habilidad de capturar patrones y relaciones de los datos.

## Descripción de dataset IRIS
[Dataset IRIS](https://www.kaggle.com/datasets/roswellwayoff/iris-data-set?select=iris.csv)
El dataset con el que se trabajó para esta actividad es el dataset de "iris". 
Este dataset trabaja con:
* 3 clases diferentes de flores, Setosa, Versicolor y Virginica.
* Las características que se utilizan para la clasificación son 4, la longitud del sépalo, el ancho del sépalo, la longitud del sépalo, y ancho de pétalo. 

## Cambios Sugeridos por Profesores (Aplica en Entrega Final)
* Corrección de Rúbrica de entregable de portafolio de análisis.
* Añadimos link donde podemos encontrar el dataset.
* Añadimos que archivos se tienen que revisar.
* Se incluye el problema a resolver 
* Añadimos una parte al código donde llevamos a cabo pruebas con distintos hiperparámetros para crear tres predicciones y posteriormente comparar las predicciones con los valores que se debieron obtener.
* Cambiamos un hiperparámetro y llevamos a cabo pruebas con ese nuevo hiperparámetro.
* Añadimos varianza
* Añadimos podado para poder regularizar y mejorar el modelo

## Descripción breve de los datos incluidos en el dataset (cantidad de registros/muestras, número de características, número de clases de salida o rango de valores de salida)
El dataset cuenta con:
* 4 atributos o columnas, sepal length cm, sepal width cm, petal length cm, petal width cm.
* 150 registros de datos todos de tipo float64.
* 3 características, Iris Sectosa, Versicolor, y Virginica.
* Este dataset no contiene ningún valor null.

## Problema a resolver
El problema a resolver con este dataset es la "clasificación" de las flores basadas en las características en la base de datos. Entrenar algoritmos que nos permitan clasificar nuevos datos basados en las características que se presentan en el dataset.

## Métricas de desempeño para los subconjuntos de prueba y entrenamiento
- Accuracy -> mide la proporción de ejemplos clasificados en relación al otro conjunto, es decir, el de prueba con entrenamiento y vice versa.
- Precisión -> Proporción de ejemplos positivos que hayan sido clasificados de manera correcta en relación al potro conjunto, es decir, el de prueba con entrenamiento y vice versa. Sirve para ver que tan confiables son las predicciones positivas.
- Recall -> mide la proporción de ejemplos positivos que hayan sido clasificados de manera correcta en relación al potro conjunto, es decir, el de prueba con entrenamiento y vice versa. Sirve para ver que tantos valores positivos se detectaron correctamente. 
- F1 Score -> combina la precisión y el recall en un solo conjunto para poder obtener la evaluación equilibrada del rendimiento de los datos que no se han visto.
- Matriz de Confusión -> nos dice los verdaderos positivos, verdaderos negativos, falsos positivos y falsos negativos tenemos. 

## Predicciones realizadas con valores de prueba y de validación
Se llevaron a cabo 3 pruebas diferentes tanto con valores de prueba como con valores de validación donde los resultados fueron los siguientes:

*Predicción con modelo de Entropy y Max Depth 3:*
- Prueba 1: ['Iris-setosa']
- Prueba 2: ['Iris-versicolor']
- Prueba 3: ['Iris-virginica']

*Predicción con modelo de Entropy y Max Depth 3:*
- Prueba 1: ['Iris-setosa']
- Prueba 2: ['Iris-versicolor']
- Prueba 3: ['Iris-virginica']

*Predicción con modelo validacion:*
- Prueba 1: ['Iris-setosa']
- Prueba 2: ['Iris-versicolor']
- Prueba 3: ['Iris-virginica']

## Comparación entre predicciones generadas y los valores que debieron obtenerse
Generamos una serie de pruebas con distintos hiperparámetros pero por motivos de espacio y orden, solo imprimimos 10 de los resultados de cada una de las pruebas.
*Comparación de predicciones con valores reales (Entropy y Max Depth 3):*
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-virginica, Valor Real: Iris-virginica
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-virginica, Valor Real: Iris-virginica
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-virginica, Valor Real: Iris-virginica


*Comparación de predicciones con valores reales (Entropy y Max Depth 4 y random state 25):*
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-virginica, Valor Real: Iris-versicolor
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-virginica, Valor Real: Iris-virginica
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-virginica, Valor Real: Iris-virginica
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor

*Comparación de predicciones con valores de Validacion:*
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-virginica, Valor Real: Iris-virginica
- Predicción: Iris-versicolor, Valor Real: Iris-versicolor
- Predicción: Iris-virginica, Valor Real: Iris-virginica
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-setosa, Valor Real: Iris-setosa
- Predicción: Iris-virginica, Valor Real: Iris-virginica

# Conclusiones sobre resultados
Primero llevamoa a cabos pruebas con arboles de decisión con distintos parámetros,
Primero:
* Criterio: entropía
* max_depth = 3
* random state = 1
En donde obtuvimos los siguientes resultados:
* Accuracy = 0.9622
* F1-Score = 0.9622
* Confusion Matrix = [[19  0  0] [ 0 18  1] [ 0  1 14]]

Segundo:
* Criterio = Entropía
* max_depth = 4
* random state = 25
En donde obtuvimos los siguientes resultados:
* Accuracy = 0.9811
* F1-Score = 0.9811
* Confusion Matrix = [[22  0  0] [ 0 16  1] [ 0  0 14]]

Tercero:
* Criterio = Gini
* random state = 42
En donde obtuvimos los siguientes resultados:
* Accuracy = 1
* F1-Score = 1
* Confusion Matrix = [[ 6  0  0] [ 0 10  0] [ 0  0  7]]


Como el mejor valor que se obtuvo de accuracy y de F1-Score es de 1, el sesgo del conjunto de validación es de Bajo Sesgo, el cual se define como que tiene un alto rendimiento o un buen ajuste a los datos y que el modelo está capturando las relaciones de los datos de manera correcta.

Por lo mismo que los valores que obtuvimos fueron de 1, la varianza es baja y no hay overfitting ni underfitting. Aunque en el caso de los datos de prueba, es posible mejorar el modelo si modificamos los parámetros. Ya vimos que al modificar los parámetros en la segunda prueba, obtuvimos una mejora de 2%, y con el conjunto de validación, pudimos obtener resultados de 100%.

Para la varianza de las 3 pruebas que llevamos a cabo obtuvimos los siguientes resultados.

* Entropy y Max Depth 3 = 0.657173
* Entropy y Max Depth 4 (Random State 25) = 0.726949
* Validación = 0.635813
