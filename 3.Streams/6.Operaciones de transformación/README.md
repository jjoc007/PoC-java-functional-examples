## Operaciones de Transformación

La operación principal de transformación  es el método **map(mapFunction)**, que retorna un nuevo stream obtenido a partir de aplicar la función de transformación mapFunction indicada a cada uno de los elementos del stream original. El tipo del stream resultante corresponderá al tipo de retorno de la función de transformación, que puede ser distinto al tipo de stream original. El stream resultante contendrá tantos elementos como el stream original.
 **Ejemplo:**
 ```java
Stream.of(3,4,5)
    .map(n -> "Valor" + n)
    .forEach(System.out::println);
```

Muestra el valor 3, 4 y 5

También tenemos una serie de métodos que permiten obedecer un stream de un tipo primitivo a partir de uno que lo sea. Entre ellos tenemos **mapToDouble**, que retorna un DoubleStream correspondiente de aplicar a cada elemento del stream original la función de conversion a double recibida. También tenemos métodos similares para otros tipos, como **mapToInt**() o **mapToLong**().

Y si lo que queremos es realizar la conversion inversa, es decir, pasar por ejemplo in **IntStream** a un **Stream<Integer>** podemos aplicar sobre el **IntStream** el método **boxed**() que retorna un stream similar al anterior pero en el que el tipo de los elementos correspondiente al tipo boxed del tipo primitivo correspondiente del stream original.