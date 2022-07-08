## ¿Que es una Interfaz Funcional?


Las interfaces funcionales son interfaces que tienen un método a implementar, es decir, un método abstracto, es decir puede implementar uno o más métodos default, pero deberá tener forzosamente un único método abstracto. Y, ¿que es un método abstracto? Un método abstracto en una interface, es un método sin implementar.

Las interfaces funcionales es un nuevo concepto que fue agregado a partir de la versión 8 de Java y cobran su importancia al utilizar.

### Ejemplo

```java
{
	package com.osb.functionalinterface;

public interface IStrategy {
    
    public String sayHelloTo(String name);
    
    public default String sayHelloWord(){
        return "Hola mundo";
    }
}
}
```

Como vemos esto es un interface funcional ya que tiene solo un método abstracto.
