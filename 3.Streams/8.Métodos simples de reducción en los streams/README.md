## Métodos Simples de Reducción en los Streams

La reducción consiste en obtener un único valor a partir de todos los valores manejados por el stream.

La clase **Stream** y las clases especificas **DoubleStream**, **IntStream** y **LongStream** implementan algunos métodos que son operaciones terminales de reducción especializadas.

La primera de ellas es **count()**, que retorna un **Long** con el numero de elementos de un stream.

**Ejemplo:**

```java
long cuantosSonImpares = Stream.of(5,4,3)
    .filter(n -> n % 2 == 0)
    .count();
```
 Retorna 4, ya que después de filtrar el stream para quedarnos solo con los números impares tan solo queda el cuatro.

 