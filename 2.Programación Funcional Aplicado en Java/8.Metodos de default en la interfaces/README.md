## ¿Que es un Método de Default en las Interfaces?

Los Default Method o Métodos default fueron incorporados en Java 8 y se encuentra en el paquete java. util. function.

Estos  son los que permiten agregar métodos implementados en las interfaces. Antes  era totalmente imposible definir el cuerpo a los métodos de las interfaces ya que nos marcaba error de compilación, pero gracias a la version de java 8 es totalmente funcional.

 Los métodos default se utilizan cuando es necesario implementar un cuerpo sin la necesidad de tener que implementar por separado una clase abstracta, además los métodos por default se pueden sobrescribir en caso de que la implementación por default no cumpla con lo que requerimos.

 **Ejemplo**
 
```java

   public default double getTotal(){
  return quantity * price;
}

```