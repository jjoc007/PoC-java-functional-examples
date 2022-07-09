## ¿Que son Funciones de Orden Superior?
Las funciones de orden superior son funciones que pueden recibir como parámetros otras funciones y/o devolverlas como resultados.


Gracias al orden superior, resulta muy sencillo utilizar esquemas generales, de modo que si tenemos que implementar una serie de funciones similares, podemos hacerlo una única vez, pero parametrizando el esquema de forma adecuada para que pueda adaptarse a cada uno de los casos concretos que necesitemos.

Se puede decir que las funciones de orden superior son aquellas que cumplen con dos requisitos básicos:

* Esperan como argumento/s una o más funciones.
* Devuelven una función como resultado.

**Ejemplo:**
```Java
const list = [2, 4, 6, 8, 9];

const squared = list.map(x => x ** 3);
```

Como vemos cada vez que ejecutemos la función se aplicara la misma función sobre cada elemento de una colección.