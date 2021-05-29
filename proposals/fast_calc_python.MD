# Título: Aprovechando el caché con Python para cómputo eficiente

## Abstracto: 
Cuando entras al mundo de Python, ver lo sencillo que puede ser escribir código, enamora. 

Muy pronto escuchas de todo mundo que el código en Python es lento, así que el estatus quo es que es un lenguaje _"lento"_ que no escala bien, y es verdad. Si lo usas como es enseñado normalmente en todos los tutoriales de internet, será lento. Una de las cosas por la cuál es asi es por su implementación de listas y aunque es muy fácil de aprender, su característica heterogénea complica el procesamiento rápido.

En esta charla aprenderás sobre el caché, la localidad temporal y la localidad espacial. Conceptos fundamentalmente necesarios para optimizar el tiempo de ejecución más de un 200x.

Esto es para ti si te gusta escribir en Python y quieres dar el siguiente paso como desarrollador. Te dará una herramienta para aplicar en tus futuros proyectos y asi optimizar grandes cálculos.

## Descripción:

Esta charla estará centrada en utilizar la memoria caché del procesador junto con los conceptos de localidad temporal y espacial para hacer eficiente nuestro uso de la memoria. Esto no se puede lograr con las listas de Python puesto que por tienen elementos de tipos heterogéneos, termina siendo un arreglo de apuntadores. 

La acción de hacer desreferencia para cada elemento del arreglo no nos deja aprovechar el caché porque los elementos de la lista no están en memoria **contigua**. 
Superamos este obstáculo usando los arrays de Numpy cuyos elementos SÍ existen en memoría contigua. 

Temario
* Ejercicio de multiplicación de matrices con listas (Intro) - 2 min
* Sobre mi - 2 min
* Caché - 8 min
* Localidad Espacial - 2 min
* Localidad Temporal - 2 min
* Ver implementación de listas en Python - 2 min
* Ver implementación de array de Numpy - 2 min
* Implementar multiplicación de matrices con arrays - 3 min
* Comparación con C, Java y Go - 5 min
* QA - 7 min


## Notas:
Los asistentes deben tener un entendimiento básico sobre cómo funciona una computadora, conceptos como lo que es la CPU y la memoria.
Deben además entender conceptos básicos de estructuras de datos como arreglos, listas y las operaciones que se pueden hacer con estas.

Me considero como la mejor persona para hablar sobre esto porque estoy cursando desarrollo de sistemas distribuidos y vimos a profundidad este tema. En la materia usamos Java pero yo lo traducí a Python y así es como llegué a esta realización.
Además estoy terminando mi licenciatura en ingeniería en sistemas computacionales, lo cuál me ha permitido entender de forma integral el manejo de memoria.

