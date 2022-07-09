## ¿Que es una Función?

 

Una función es un bloque de código que realiza alguna operación. Esta nos permiten dividir el trabajo que hace un programa, en tareas más pequeñas separadas de la parte principal.

 Una función puede definir opcionalmente parámetros de entrada que permiten a los llamadores pasar argumentos a la función. Una función también puede devolver un valor como salida. 
 
 #### *¿Para que son Útiles las Funciones?*
 
 Las funciones son útiles para encapsular las operaciones comunes en un solo bloque reutilizable, idealmente con un nombre que describa claramente lo que hace la función. 

 #### *¿Como se Crea una Función?*

 Para crear una función se debe tener en cuenta 5 partes:

* **Modificadores de una función:**
    Los modificadores son varias palabras clave , o palabras reservadas de un lenguaje de programación, que puede modificar la forma en que los métodos son usados.

*  **Ejemplos de modificadores:**
   * public
   * private
   * protected
   * virtual
   * static
            
---
* **Tipo de retorno de un método:** 
    El tipo retorno es el tipo de valor devuelto por la función, las funciones sólo pueden devolver un valor, ya sea un tipo de datos básico, como puede ser un número entero o un string.
---

* **Nombre de la función:**
El nombre o identificador de las funciones es como se llama la función. Se debe tener en cuenta que al momento de ponerle nombre no puede tener espacios.
  * **Ejemplos:**
    
 |Correcto   | Incorrecto |
 |----------|--------|
 |Funcion_1 |Funcion 1  |
 |Resta_Nomina|Resta Nomina|
 |Suma_Resta_Nomina|Suma Resta Nomina
 ---

* **Argumentos de una función:**

    Los argumentos de una función, también llamados parámetros, representa una lista de variables opcionales cuyos valores son pasados al método para ser usados por éste.

    Son opcionales ya que algunos métodos no aceptan argumentos
---
* **Bloque de código:**
El código de la función es la secuencia de instrucciones o sentencias que la función realiza.Estas instrucciones son las tareas que hacen que la función tengan sentido.
---
A continuación se muestra un ejemplo de como se vería en código:
**Ejemplo:**

```
[Modificadores] tipo_retorno nombre_funcion ([argumentos])
{
    bloque_código;
}

```
 Este es un ejemplo de una función que tiene dos argumentos y devuelve un resultado de una resta:

```Java
public int Resta(int numero1, int numero2)
{
    return num1 - num2;
}
```
