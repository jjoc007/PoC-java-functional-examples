## ¿Que es una Función Lambda?

La función Lambda es una función incorporada en Java 8 y se encuentra en el paquete java. util. function .Las funciones lambdas es un término adoptado de la programación funcional y corresponden con funciones de Java que normalmente son anónimas y se escriben en línea. Como cualquier función recibe cero o más argumentos y devuelven uno o ningún valor de retorno.

**Ejemplo**


```java

    Function<String,Integer> sizeOf = (String s) -> {
    return s.length();
};

```



