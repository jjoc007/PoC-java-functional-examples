## ¿Que es una Interface Predicate?

El Predicate es una interfaz en Java que se utiliza como asignación de destino para una expresión lambda o una referencia de método. Se agregó a Java 8 y proporcionó un enfoque más funcional para escribir código en Java.

Un Predicate se usa más comúnmente para filtrar una secuencia de objetos.

La interfaz de sintaxis de Predicate tiene el siguiente aspecto.

**Ejemplo:**

```java
@FunctionalInterface
public interface Predicate<T>
```

La **T** es el tipo de entrada a la interfaz de predicado. 

Ahora un ejemplo de como se vería un objeto predicate.

**Ejemplo:**

```java
Predicate<Integer> noMenorQue5 = x -> x > 5;
```

El el ejemplo creamos un Predicate llamado noMenorque5. Este predicate toma la entrada Integer; por lo tanto, T es entero aquí. Este predicate verifica si los argumentos de entrada son mayores que cinco o no.
