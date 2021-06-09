# JAVA SE
Concepto y ejemplos de JAVA SE

## Clases Abstractas
Todo tiempo una clase abstracta debe de ser una clase padre ya que es muy generico que puede heredar métodos,
**abstract** es la palabra reservada que defina una clase abstracta.

```JAVA
public abstract class Figura {
}
```

- **No** implementaremos todos los métodos
- **No** crearemos instancias. 

#### Métodos abstractos

* Un método que sea obligatorio implementar debe de tener la palabra reservada **abstract**
* Un método abstracto no tendra  implementación igual que las interfaces y debe de tener un manejador de acceso que puedan 
  ser accedido desde clases hijas

```JAVA
public abstract class Figura {
  abstract void dibujate();

}
```

La clase abstracta solucionan las siguentes restricciones de las interfaces y Herencias
### Interfaces
   - Aveces **No** necesitamos **implementar todos los métodos**
 
### Herencia
  - Las clases podrían **No** necesitar heredar la implementación de un método.
  - A veces no necesitamos crear instancias de una clase padre, por que es muy genérica.

## Interfaces 

- Métodos Abstractos sin implementación.
- Campos constantes.
- Tipo de referencia Polimorfimos similar a **Clases Abstactas**

### Interfaces apartir de Java 8 y 9
Se agregar los modificadores de acceso default en java 8 y private en java 8 con estos modificadores los metodos y apuede tener implemetación.

```JAVA
   public interfaces MyInterface {
     default void defaultMethod() {
       privateMethod("Hello from the default method!")
     }
     
     private void privateMethod(final String string) {
      System.out.println(string);
     }
     
     void normalMethod();   
 }

```

