# Título: Aprovechando el caché con Python para cómputo eficiente

## Abstracto: 
Aquí aprenderás sobre el caché, la localidad temporal y la localidad espacial, necesarios para optimizar el tiempo de ejecución más de un 200x. Esto te dará una herramienta para aplicar en tus futuros proyectos optimizando grandes cálculos con Python.

## Descripción:

Usar listas es muy sencillo y normalmente son usadas para todo. Hay situaciones en donde necesitamos hacer cálculos con matrices y quizá con 50 elementos no se haga ninguna diferencia pero cuando lleguemos a los miles de elementos, hacer estas operaciones con listas, termina siendo una eternidad que jamás será apta para producción. La introducción será explicando un simple programa de multiplicación de matrices N*N usando listas añidadas. Se enseñará un diagrama con la tendencia de tiempo de ejecución con respecto a N, así la audencia podrá ver lo ridiculamente lento que son las listas.

Esta charla estará centrada en utilizar la memoria caché del procesador junto con los conceptos de localidad temporal y espacial para hacer eficiente nuestro uso de la memoria. Esto no se puede lograr con las listas de Python puesto que tienen elementos heterogéneos, termina siendo un arreglo de apuntadores. La acción de hacer desreferencia para cada elemento del arreglo no nos deja aprovechar el caché porque los elementos de la lista no están en memoria **contigua**. 
Se usará el diagrama de jerarquía de memoria para dar a entender la importancia de cada uno de sus niveles. Después se explicará cómo es el intercambio de datos entre el caché y la RAM. Teniendo esto claro será fácil describir cómo conviene acceder a datos cercanos en la memoria y con alta frecuencia de uso.

Más adelante veremos un diagrama de la implementación de listas comparado con los arreglos de Numpy. Veremos que los arreglos sí tienen memoria contigua y pueden hacer uso del caché a diferencia de las listas.

Volveremos a implementar el programa de multiplicación de matrices pero con arreglos de numpy. Podremos ver una mejora inmediata en el tiempo de ejecución pero esto no acaba aquí; se hará una pequeña modificación al programa para tener en mente la localidad espacial y temporal, veremos como se vuelve más eficiente nuestro cálculo.

Al final veremos el mismo programa implementado en otros tres lenguajes populares para tener contexto de qué tan rápido puede ser Python en comparación con lenguajes *rápidos*.


Temario
* Ejercicio de multiplicación de matrices con listas (Intro) - 2 min
* Sobre mi - 2 min
* Caché - 8 min
* Localidad Espacial - 2 min
* Localidad Temporal - 2 min
* Ver implementación de listas en Python - 2 min
* Ver implementación de array de Numpy - 2 min
* Implementar multiplicación de matrices con arrays - 5 min
* Comparación con C, Java y Go - 5 min
* QA - 5 min


## Notas:
Los asistentes deben tener un entendimiento básico sobre cómo funciona una computadora, conceptos como lo que es la CPU y la memoria.
Deben además entender conceptos básicos de estructuras de datos como arreglos, listas y las operaciones que se pueden hacer con estas.

Me considero como la mejor persona para hablar sobre esto porque estoy cursando desarrollo de sistemas distribuidos y vimos a profundidad este tema. En la materia usamos Java pero yo lo traducí a Python y así es como llegué a esta realización.
Además estoy terminando mi licenciatura en ingeniería en sistemas computacionales, lo cuál me ha permitido entender de forma integral el manejo de memoria.

