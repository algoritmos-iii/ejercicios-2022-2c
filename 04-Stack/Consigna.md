# Stack

## Primera Parte 

En este ejercicio deberán implementar un stack y testearlo. Para ello, partirán del código inicial del archivo `StackPrimeraParte.st` 

Nuestros desarrolladores se fueron de vacaciones y dejaron las cosas por la mitad, tenemos un solo test... ¡Y FALLA!

Por lo menos armaron una lista de las cosas que querían probar:

- que se pueda agregar un elemento (push)
- que se pueda sacar un elemento (pop)
- que el pop devuelve el último elemento
- que el stack es LIFO. Es decir el último que se agrega (push) es el primero que sale (pop) 
- que se puede obtener el último elemento agregado sin removerlo (top)

La recomendación será hacer de a un test y hacerlo pasar de la forma más sencilla, usando ifs.


## Segunda Parte


Vamos a empezar de nuevo. Primero, hagan un file out del paquete que ya tenian (`StackPrimeraParte`) y guárdenlo, habrá que incluírlo en la entrega. Luego, borren por completo el paquete `StackPrimeraParte` (la primera de las columnas del browser).

Hacer file in del archivo Stack-Exercise.st.

Se encontrarán con algunos tests que fallan, tendrán que reimplementar el stack a partir de ellos. 

Les dejamos algunas ayudas: 

1. Primero hagan pasar todos los tests usando if y después aplique la técnica para sacar if que vimos. 
2. Si les sirve, utilicen una metáfora. Una muy útil es la de representar el juego de los bebés donde se apilan platos en una especie de torre de Hanoi.
Importante: Tampoco se puede usar handleo de excepciones para ocultar lo que sería en definitiva un if.

## Tercera Parte

El stack de la segunda parte es utilizado para almacenar oraciones de cualquier longitud. Se debe implementar el mensaje find de `SentenceFinderByPrefix` que dado un prefijo se encarga de devolver todas las oraciones almacenadas en el Stack que contengan dicho prefijo. Por ej. si el prefijo es "Wint", y las oraciones en el Stack son "winter is coming", "winning is everything", "The winds of Winter" y "Winter is here" sólo debería devolver la última. 

El prefijo es case-sensitive, no puede ser vacío, ni contener espacios vacíos y el stack al terminar la operación de búsqueda debe de mantener las mismas oraciones en idéntico orden. 

Además de implementar "find", se debe testear dicha funcionalidad. Para ello escriba todos los tests que crea necesario en SentenceFinderByPrefixTest.

Aclaración: No se pueden agregar mensajes adicionales a Stack.

## Extra

Se pide extender el modelo para que además de representar al stack ilimitado ya construido, se puedan construir instancias de un stack limitado. Es decir, uno que tenga una cantidad limitada de celdas y que no se puedan pushear más elementos que los disponibles en su capacidad.

Se pide además analizar cuál de los modelos anteriores cree que es más sencillo extender para representarla y hacerlo. 

Además se deberán agregar los casos de tests que hagan falta para probar el nuevo tipo de stack.
