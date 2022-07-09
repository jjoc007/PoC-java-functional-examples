## Método Reduce Stream


El método reduce() , es usado para realizar la suma de todos los elementos de un stream. Cada elemento de la lista de números se combina iterativamente empleando el operador de suma para generar un resultado. También se encuentra en las Clases Stream se utiliza para recorrer un stream y retornar un solo valor , si tienes un stream que almacena Strings lo puedes reducir a la concatenación de todos los objetos en el , asi mismo si guardas solo datos numéricos.

**Ejemplo:**
```java
int suma = numeros.stream().reduce(0, (5,4) -> 
5+4);
```

Retorna 9, ya que hace la operación de suma de los dos valores.