## ¿Que es un Stream?


Los Streams en java son un nuevo modelo de datos que nos permite tratar las colecciones como si de un proceso ETL (“Extract Transform and Load”) se tratara. Esto nos permite utilizar las funciones Map y Reduce tan comunes en esos procesos, especialmente en la etapa de transformación.

En diferentes palabras los Streams son "envoltorios" de colecciones de datos que nos permiten operar y hacer que el procesamiento masivo de datos sea rápido y fácil de leer. 


## ¿En que nos ayudan?

Generalmente cuando trabajamos con colecciones filtramos, calculamos y realizamos muchos tipos de operaciones sobre los datos. Los Streams nos permiten a través del paradigma funcional abstraernos del cómo programar esas operaciones y sólo centrarnos en que resultado se espera y escribirlo de una manera muy declarativa.


## ¿Que se Debe Tener en Cuenta al Usar un Steam?

Es importante tener en cuenta que los Streams no almacenan datos y no son una estructura de datos en sí. Tampoco modifican la fuente de datos subyacente. Solo realizan operaciones simples o concatenadas sobre ellos.

### Ejemplo:

```java
List<Long> listStream = lista.stream().filter(valor -> valor < valorMaximo)         
                                .collect(Collectors.toList());
```

En en el ejemplo nos muestra que a una lista le asignamos el return de un Stream al cual sólo le aclaramos que tiene que realizar un filtro a través de una función lambda y que lo tiene que recolectar en una lista.