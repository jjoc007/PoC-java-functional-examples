## ¿Que es un Stream Especifico?


## ¿Que es un Stream Paralelo?
 
 Es una característica de Java 8 y superior, diseñada para utilizar múltiples núcleos del procesador. Normalmente, cualquier código Java tiene una secuencia de procesamiento, donde se ejecuta secuencialmente. Mientras que al usar flujos paralelos, podemos dividir el código en múltiples flujos que se ejecutan en paralelo en núcleos separados y el resultado final es la combinación de los resultados individuales. Sin embargo, el orden de ejecución no está bajo nuestro control.

 **¿Como se usa el stream paralelo?**

 Hay dos maneras de usar el stream paralelo:

 * Transmisión
 * Colección

 *Ejemplo:*

 ```java
public class ParallelStreamTest {
  
    public static void main(String[] args) throws IOException {
        File fileName = new File("M:\\Documents\\Textfile.txt");
    
        Stream<String> text = Files.lines(fileName.toPath());
        
        text.parallel().forEach(System.out::println);
          
        text.close();
    }
}
```
En el ejemplo se crea un objeto de archivo que apunta a un archivo txt preexistente en el sistema. Luego creamos una secuencia que lee del archivo de texto una línea a la vez. Luego usamos el método paralelo() para imprimir el archivo leído en la consola.

