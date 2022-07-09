## Operaciones de Filtrado

Las operaciones de filtrado son  operaciones intermedias que se pueden realizar sobre un stream que solo contenga algunos de los elementos del stream original. Para ello, Java nos proporciona distintos métodos.


El primero de ellos es el método **distinct()**, que retorna un nuevo stream con los elementos del stream original, excepto aquellos que estuvieron repetidos. Para determinar que dos elementos son iguales se usara el método **equals()** del elemento. Esta operación de comparación requiere de la comprobación del estado de los elementos, por lo que su rendimiento no es adecuado para streams paralelos. 

**Ejemplo:**

```java
Stream.of(5,3,4,5)
    .distinc()
    .forEach(System.out::println);
```

Otra operación de filtrado es el método **limit(n)**, que retorna un nuevo stream con tan solo n elementos de stream original, atendiendo el orden intrínseco del mismo. Tiene un mal rendimiento en streams paralelos ordenados. 

**Ejemplo:**

```java
Stream.of(5,3,4,5)
    .limit(5)
    .forEach(System.out::println);
```
Mostraría los valores 3 y 4.

La operación de filtrado mas genérico es el método **filter(predicate)**, que retorna un nuevo stream que solo incorpora los elementos del stream original que cumplan el predicado recibido. 

**Ejemplo:**
```java
Stream.of(5,3,4,6,2)
    .filter(n -> n < 7)
    .forEach(System.out::println);
```

Muestra los valores 6,5,4,3,2.




