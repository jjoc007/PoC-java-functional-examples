## ¿Que es Inmutabilidad?

Una explicación muy sencilla de esto es que algo es inmutable cuando no se puede modificar.


## ¿Que es la Inmutabilidad en Programación?

Hay que tener en cuenta que en la programación la inmutabilidad aplican para variables y objetos.

Una variable es inmutable cuando su valor no se puede modificar. Y un objeto lo es cuando su estado no puede ser modificado una vez creado. 

En algunos casos un objeto puede ser considerado como inmutable aunque algunos de sus atributos internos cambie, siempre y cuando el estado del objeto parezca no cambiar desde un punto de vista externo al mismo. 

En conclusión es una forma de asegurarnos que nuestro objeto no se modifica en lugares inesperados, afectando con ello la ejecución de nuestro programa.

**Ejemplos**

```scala
val p = new Person("name", "surname")
```

Este es un ejemplo sencillo en el cual se vuelve inmutable al cambiar la variable  'var' a 'val' para declararla.

---

```java

public final class Person {
    public final String name;
    public final String surname;

    public Person(String name, String surname) {
        this.name = name;
        this.surname = surname;
    }    
}
```

Este es un ejemplo un poco mas complejo en java, en el cual hacemos inmutable la variable Person.