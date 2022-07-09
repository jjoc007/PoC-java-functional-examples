## Operaciones Terminales de Consulta

La clase stream proporciona una serie de métodos de consulta sobre los elementos de un stream, denominadas operaciones de cortocircuito (short-circuit terminal operations). Se llaman asi por que se deja de procesar el resto de elementos si con los elementos que ya han sido procesados  se es capaz de determinar el resultado.

Tenemos un conjunto de métodos que permiten consultar, respectivamente, si todos, ninguno o algunos de los elementos del stream cumplen con un determinado predicado, retorna un valor booleano. Son los métodos **allMatch(predicate)**, **noneMatch(predicate)** y **anyMatch(predicate)**.

**Ejemplo:**
```java
boolean todosPares = Stream.of(1,2,3,4)
    .allMatch(n -> n % 2 != 0);
```

Falta Complementar

