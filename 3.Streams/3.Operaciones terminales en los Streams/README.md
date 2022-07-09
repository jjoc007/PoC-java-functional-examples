## Operaciones Terminales en los Streams

Las operaciones terminales procesan todos los elementos del stream para generar un resultado o un efecto secundario. De echo, no retorna un stream. Después de su ejecución, el stream original NO puede ser  usado de nuevo, produciendo una excepción si se intenta. De ahi que se denominen operaciones terminales. Por tanto, un determinado stream puede ser utilizado solo una vez, si necesitamos procesar la misma fuente de datos, deberemos crear un nuevo stream con ella como origen.   

Otra característica importante de pipeline es que es perezoso, lo que quiere decir que las operaciones intermedias solo son ejecutadas cuando las requiere la operación terminal que se esta ejecutando.  

Las operaciones terminales más comunes son las siguientes:

|Operación   | Información                    |
|----------|----------------------------------|
|Optional<T> findFirst(Predicate) |Devuelve el primer elemento del Stream que coincida con la condición del predicado, o un Optional vacío si no se cumple la condición.  |
|Optional<T> findAny(Predicate)|Devuelve un elemento aleatorio del Stream que coincida con la condición del predicado, o un Optional vacío si no se cumple la condición. Pensado para ofrecer un mayor rendimiento en operaciones paralelas.|
|Boolean allMatch(Predicate)|Devuelve true si la condición del predicado se cumple para todos los elementos del Stream, false para el resto de casos. |
|Boolean anyMatch(Predicate)|Devuelve true si la condición del predicado se cumple para cualquier elemento del Stream, false para el resto de casos. |
|collect(Collector)|Devuelve el Stream en forma de colección del tipo que definamos. Podemos utilizar la clase de utilidad Collectors, que nos ofrece varias implementaciones de la interfaz Collector. |

*Este recuadro fue tomado de la pagina [Dovixman](https://dovixman.io/2019/04/03/java-8-streams/#:~:text=Las%20operaciones%20terminales%20son%20las,incluya%20una%20de%20estas%20operaciones.).*

