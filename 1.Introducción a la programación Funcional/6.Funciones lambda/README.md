##  ¿Que son Funciones Lambda?

Las funciones Lambda son funciones anónimas que solo pueden contener una expresión, ademas es una subrutina definida que no está enlazada a un identificador. 

Las expresiones lambda a menudo son argumentos que se pasan a funciones de orden superior, o se usan para construir el resultado de una función de orden superior que necesita devolver una función.

 Si la función solo se usa una vez o un número limitado de veces, una expresión lambda puede ser sintácticamente más simple que usar una función con nombre. 

 Se puede decir que las funciones lambda son aquellas que cumplen con dos requisitos basicos:
  * Son funciones anidadas que permiten el acceso a variables no locales dentro de la función contenedora
  * No pueden ser recursivas sin la asistencia de un operador de punto fijo o enlazarlas a un nombre.

  **Ejemplo:**

  ```Java
  Function<String,Integer> sizeOf = (String s) -> {
    return s.length();
};
  ```


