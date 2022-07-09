## Funciones Generadoras de Streams
Vamos a ver diferentes ejemplos de funciones generadoras de stream

* **Array:** El método estático **Arrays.stream(Array)** recibe un array, que actuara como fuente de datos origen del stream.
```java
String asistentes[] = Arrays.asList{"Martinez","Mass","Perez"};
Stream<String> stream = Arrays.stream()
```

* **Colección:** Vamos a ver un ejemplo en que se ejecuta el método stream() sobre una colección para crear un stream que tenga como fuente de datos origen dicha colección. También tenemos disponible el métodos parallelStream() para que los elementos sean procesados en modo paralelo.

Podemos crear un **List**, **Set** o **Queue** y cualquiera de las clases que implementen dichas interfaces. Por ejemplo desde una lista:

```java
List<String> apellidos = Arrays.asList("Martinez","Mass","Perez");
Stream<String> stream = apellidos.stream()
```
* **Función suministrada de objetos:** El método estático **Stream.generate()** recibe un **Supplier**, es decir, una función suministrada de elementos, que actuara como fuente de datos de origen infinita para el stream.

```java
AtomicInteger asistenteNumber = new AtomicInteger(1);
Stream<String> stream = Stream.generate(() -> "Asistente #" + 

studentNumber.getAndIncrement());
```

* **Conjunto predeterminado de elementos:** El método estático **Stream.of()** recibe un numero variable de elementos, que actuaran como fuente de datos de origen del stream.
```java
Stream<String> stream = Stream.of()("Martinez","Mass","Perez")
```







