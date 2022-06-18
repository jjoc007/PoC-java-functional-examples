## ¿Que es una Clase Optional?

Un Optional es una clase que puede o no contener un valor, es decir, que se comporta como un wrapper para cualquier tipo de objeto que pueda o no ser nulo.

 Su principal ventaja es que nos permite manejar los NullPointer, o sea que no tendremos que ir preguntando si un objeto es nulo antes de hacer algo. Otra ventaja importante es que ayudan a la legibilidad del código, por lo que será más fácil leerlo y a su vez mantenerlo.

 
### Ejemplo:
```java

    Optional<Consola de videojuego> xboxone = obtenerConsola("XboxOne");

	xboxone.ifPresent(consola -> 
    consola.precio.ifPresent(precio -> 
        imprimirEuros(precio.euros);
    );
);

```
