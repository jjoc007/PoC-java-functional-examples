## Funciones Puras

**¿Que es una función pura?**


 Una función pura son aquellas que operan utilizando solo los parámetros de entrada sin recurrir a ningún otro elemento fuera de ellas siempre regresa el mismo valor de salida y no tiene otro efecto secundario observable.

Se puede decir que las funciones puras son aquellas que cumplen con dos requisitos:

* Dado unos parámetros de entrada de idéntico valor, la función siempre devolverá el mismo resultado.
* El cómputo de la función, su lógica, no implica ningún efecto observable colateral fuera de ella.

**Ejemplo:**
```
function restaej(resta = 5) {

  return function (cantidad) {

    return resta + cantidad;
  }

}

const restA = restaej();

restA(5); //5
restA(5); //5
```

Como vemos cada vez que ejecutemos la función con el mismo parámetro obtenemos el mismo resultado.

---
## ¿Que es una función Impura?

Las funciones impuras son aquellas que no siempre retornan lo mismo o que pueden leer o escribir de un estado que puede cambiar.


Se puede decir que las funciones impuras son aquellas que cumplen con dos requisitos básicos:

* Cambia el estado interno de cualquier argumento que se haya pasado

* Puede tener efecto sin devolver nada

**Ejemplo:**

```

const time = () => Date.now();
time(); // => 17
time(); // => 30
```
Como vemos cada vez que ejecutemos la función no podremos predecir su valor de retorno, debido que no tenemos unos parámetros fijos definidos.
 