* [Momento de Retroalimentación: Módulo 2 Uso de framework o biblioteca de aprendizaje máquina para la implementación de una solución. (Portafolio Implementación)](MomentoRetro_Modulo2_A01284090.ipynb)
* [Momento de Retroalimentación: Módulo 2 Análisis y Reporte sobre el desempeño del modelo. (Portafolio Análisis)](https://github.com/analucia2107/MomentoRetro_Modulo2_A01284090/blob/main/MometoRetro_Modulo2_AnalisisyReporte_A01284090.ipynb)

# MomentoRetro_Modulo2_A01284090

## Descripción del modelo
El modelo a utilizar en este momento de retroalimentación es el "Decision Tree Classifier" es un modelo de aprendizaje automático que nos muestra en manera de un árbol con "raíz" (la parte más alta del gráfico), "ramas", y las "hojas" (la parte final o más baja del árbol). Se empieza con una sola pregunta y dependiendo de la respuesta, se va abriendo el árbol con ramas basándose en las características con las que se pueden responder las preguntas. Cada vez que se responde la pregunta, si por ejemplo la pregunta es ¿Tiene patas? y buscamos que el animal si tenga patas y el animal en la imagen no las tiene, al responder que no, el nodo va a abrirse con otra pregunta y se vuelve a dividir en grupos dependiendo la respuesta hasta llegar a las hojas, donde se van a asignar etiquetas basadas en las respuestas anteriores.

Este modelo guarda y analiza toda la información de preguntas y características para poder clasificar nuevos ejemplos en otros posibles archivos y así poder resolcer un problema de clasificación de una manera más sencilla y rápida por su habilidad de capturar patrones y relaciones de los datos.

## Descripción de dataset IRIS
El dataset con el que se trabajó para esta actividad es parte de scikit-learn y se llama "iris". Este dataset trabaja con 3 clases diferentes de flores, Setosa, Versicolor y Virginica. Las características que se utilizan para la clasificación son 4, la longitud del sépalo, el ancho del sépalo, la longitud del sépalo, y ancho de pétalo. Este dataset puede cargarse utilizando "from sklearn.datasets import load_iris" y luego se puede guardar en una variable como "iris = load_iris()".

## Cambios Sugeridos por Profesores (Aplica en Entrega Final)

## Descripción breve de los datos incluidos en el dataset (cantidad de registros/muestras, número de características, número de clases de salida o rango de valores de salida)
El dataset cuenta con 4 columnas (sepal length cm, sepal width cm, petal length cm, petal width cm) y 150 registros de datos todos de tipo float64, y 3 características (Iris Sectosa, Versicolor, Virginica). No contiene ningún valor null.

## Problema a resolver
El problema a resolver con este dataset es la "clasificación" de las flores basado en las características en la base de datos.

## Métricas de desempreño para los subconjuntos de prueba y entrenamiento
- Accuracy -> mide la proporción de ejemplos clasificados en relación al otro conjunto, es decir, el de prueba con entrenamiento y vice versa.
- Precisión -> Proporción de ejemplos positivos que hayan sido clasificados de manera correcta en relación al potro conjunto, es decir, el de prueba con entrenamiento y vice versa. Sirve para ver que tan confiables son las predicciones positivas.
- Recall -> mide la proporción de ejemplos positivos que hayan sido clasificados de manera correcta en relación al potro conjunto, es decir, el de prueba con entrenamiento y vice versa. Sirve para ver que tantos valores positivos se detectaron correctamente. 
- F1 Score -> combina la precisión y el recall en un solo conjunto para poder obtener la evaluación equilibrada del rendimiento de los datos que no se han visto.
- Matriz de Confusión -> nos dice los verdaderos positivos, verdaderos negativos, falsos positivos y falsos negativos tenemos. 
