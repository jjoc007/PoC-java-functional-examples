## ¿Que es un Consumer?

La interfaz del consumidor es parte del paquete java.util.function que se introdujo desde Java 8 para implementar la programación funcional en Java. Representa una función que toma un argumento y produce un resultado. Sin embargo, este tipo de funciones no devuelven ningún valor.

La expresión lambda asignada a un objeto de tipo Consumer se usa para definir su accept() que finalmente aplica la operación dada en su argumento. Los consumidores son útiles cuando no es necesario devolver ningún valor, ya que se espera que operen a través de efectos secundarios.

La interfaz del consumidor consta de las dos funciones siguientes:

1. **Aceptar:** acepta un valor y realiza la operación en el argumento dado.
2. **Luego:** Devuelve un Comsumer compuesto en el que el Consumer parametrizado se ejecutará después del primero. Si la evaluación de cualquiera de las funciones arroja un error, se transmite al llamador de la operación compuesta.


## ¿Que es un Supplier?

La interfaz Java Supplier pertenece al paquete java.util.function y fue introducida en Java 8 para poder implementar programación funcional con Java. Representa una función a la cual no se le pasa ningún argumento y devuelve un valor genérico T.
 * T : denota el tipo del resultado

Para utilizarlo se invoca al método get para producir un valor de la expresión lambda asignada a un objeto.

**Ejemplo:**
```java
public class Main {
    public static void main(String args[])
    {
  
        // This function returns a random value.
        Supplier<Double> randomValue = () -> Math.random();
  
        // Print the random value using get()
        System.out.println(randomValue.get());
    }
}
```

