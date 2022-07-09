## Operaciones de Ordenamiento

Algunos streams son ordenados, es decir que sus elementos poseen un determinado orden, conocido como encounter order. Por ejemplo, un stream cuya fuente de datos corresponda a una lista creara un stream ordenado, cuyo encounter order sera el orden en el que los elementos están situados en la lista. 

El hecho de que un stream sea ordenado o no dependerá del tipo de fuente de datos asociada y de las operaciones intermedias anteriores que hayamos realizado mediante las que se ha obtenido el stream.

Algunas operaciones trabajan por defecto en base de encounter order, imponiendo una restriccion acerca del orden en el que los elementos deben ser procesados, como por ejemplo las operaciones intermedias **limit**() o **skip**(). 

**Ejemplo:**

```java
Stream.of("Martinez","Mass","Perez","Piñeros")
    .limit(3)
    .forEach(System.out::println);
```

Muestra los valores Martinez, Mass, Perez, en este orden.