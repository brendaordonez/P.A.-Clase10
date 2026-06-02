# P.A.-Clase10
# Ejercicio 1: Investigar y documentar críticas a los patrones de diseño
  
Los patrones de diseño han sido criticados por varias razones:

Rigidez: obligan a encajar problemas en moldes predefinidos, incluso cuando no son necesarios.

Complejidad innecesaria: algunos patrones generan más clases y jerarquías de las que realmente se necesitan.

Obsolescencia: ciertos patrones pierden relevancia en lenguajes modernos que ya ofrecen soluciones más simples (ej. lambdas en Python reducen la necesidad de Strategy).

Por ejemplo el uso excesivo de Singleton puede dificultar pruebas unitarias y generar dependencias ocultas.

# Ejercicio 2:
Seleccione 3 patrones de diseño e implementarlos en Python. Arme ejemplos concretos de uso. Lo ideal es
elegir un patrón de cada clasificación.

# Ejercicio 3: Piense en 3 problemas habituales de su vida diaria en los cuales podría aplicar patrones de diseño

Problemas habituales podrian ser la planificación de estudio (Command: cada tarea como leer, resolver ejercicios, repasar se modela como un comando ejecutable)

Otro ejemplo sería cocinar , podria relacionarse con Factory, ya que elegir qué receta instanciar según ingredientes disponibles.

La organización de series en Netflix se asimilaria a Composite, donde se agruparian capítulos en temporadas y temporadas en series.

# Ejercicio 4: Los patrones de diseño suelen poseer distintos nombres o denominaciones. Arme una tabla con los posibles distintos nombres usados.

| **[Patrón](ca://s?q=Lista_de_patrones_de_dise%C3%B1o)** | Alias |
| --- | --- |
| Singleton | Instancia única |
| Observer | Publicador–Suscriptor |
| Strategy | Política, algoritmo intercambiable |
| Factory Method | Constructor, Creator |
| Composite | Árbol, Contenedor jerárquico |
| Proxy | Representante, Placeholder |



# Ejercicio 5: ¿Qué son los antipatrones de diseño? Ejemplifique algunos casos.
 
Los antipatrones son soluciones aparentemente útiles pero que generan problemas a largo plazo. 
Ejemplos:

God Object: una clase que concentra demasiadas responsabilidades.

Spaghetti Code: lógica enredada sin estructura clara.

Golden Hammer: usar siempre la misma técnica o patrón para todo.

Lava Flow: código viejo que nadie elimina y se acumula.

Copy-Paste Programming: duplicar código en lugar de abstraer.


# Ejercicio 6: Investigue el uso de otras buenas prácticas, como por ejemplo SOLID.

Los principios SOLID son un conjunto de cinco buenas prácticas de programación orientada a objetos que ayudan a crear software más mantenible, escalable y fácil de entender. Aplicarlos correctamente evita problemas como el “código espagueti” y el exceso de acoplamiento

| **Principio** | **Descripción** | **Beneficio clave** |
| --- | --- | --- |
| **[Responsabilidad Única (SRP)](ca://s?q=Principio_de_Responsabilidad_%C3%9Anica)** | Cada clase debe tener un único propósito o motivo de cambio. | Código más claro y fácil de mantener. |
| **[Abierto/Cerrado (OCP)](ca://s?q=Principio_Abierto_Cerrado)** | El software debe estar abierto a extensión pero cerrado a modificación. | Permite agregar nuevas funcionalidades sin alterar código existente. |
| **[Sustitución de Liskov (LSP)](ca://s?q=Principio_de_Sustituci%C3%B3n_de_Liskov)** | Las clases hijas deben poder reemplazar a las clases padres sin alterar el comportamiento esperado. | Favorece la reutilización y evita errores en jerarquías de herencia. |
| **[Segregación de Interfaces (ISP)](ca://s?q=Principio_de_Segregaci%C3%B3n_de_Interfaces)** | Es mejor tener interfaces específicas que una interfaz general demasiado grande. | Reduce dependencias innecesarias y simplifica el diseño. |
| **[Inversión de Dependencias (DIP)](ca://s?q=Principio_de_Inversi%C3%B3n_de_Dependencias)** | Los módulos de alto nivel no deben depender de módulos de bajo nivel, ambos deben depender de abstracciones. | Disminuye el acoplamiento y facilita pruebas unitarias. |

Ejemplos prácticos de aplicación

SRP: Una clase Factura que solo maneja datos de facturación, mientras otra clase ImpresoraFactura se encarga de imprimir.

OCP: Un sistema de pagos que permite agregar nuevos métodos (PayPal, criptomonedas) sin modificar el código base.

LSP: Una clase Ave con método volar(), y subclases como Gorrión que respetan ese contrato.

ISP: En lugar de una interfaz Vehículo con demasiados métodos, dividir en VehículoConMotor y VehículoConPedales.

DIP: Un sistema de notificaciones que depende de una interfaz Notificador, no de implementaciones concretas como EmailNotificador o SMSNotificador.
