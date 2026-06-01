# P.A.-Clase10
Ejercicio 1: Investigar y documentar críticas a los patrones de diseño
  
Los patrones de diseño han sido criticados por varias razones:

Rigidez: obligan a encajar problemas en moldes predefinidos, incluso cuando no son necesarios.

Complejidad innecesaria: algunos patrones generan más clases y jerarquías de las que realmente se necesitan.

Obsolescencia: ciertos patrones pierden relevancia en lenguajes modernos que ya ofrecen soluciones más simples (ej. lambdas en Python reducen la necesidad de Strategy).

Por ejemplo el uso excesivo de Singleton puede dificultar pruebas unitarias y generar dependencias ocultas.


Ejercicio 3: Piense en 3 problemas habituales de su vida diaria en los cuales podría aplicar patrones de diseño

Problemas habituales podrian ser la planificación de estudio (Command: cada tarea como leer, resolver ejercicios, repasar se modela como un comando ejecutable)

Otro ejemplo sería cocinar , podria relacionarse con Factory, ya que elegir qué receta instanciar según ingredientes disponibles.

La organización de series en Netflix se asimilaria a Composite, donde se agruparian capítulos en temporadas y temporadas en series.


Ejercicio 4: Los patrones de diseño suelen poseer distintos nombres o denominaciones. Arme una tabla con los posibles distintos nombres usados.

| **[Patrón](ca://s?q=Lista_de_patrones_de_dise%C3%B1o)** | Alias |
| --- | --- |
| Singleton | Instancia única |
| Observer | Publicador–Suscriptor |
| Strategy | Política, algoritmo intercambiable |
| Factory Method | Constructor, Creator |
| Composite | Árbol, Contenedor jerárquico |
| Proxy | Representante, Placeholder |



Ejercicio 5: ¿Qué son los antipatrones de diseño? Ejemplifique algunos casos.
 
Los antipatrones son soluciones aparentemente útiles pero que generan problemas a largo plazo. 
Ejemplos:

God Object: una clase que concentra demasiadas responsabilidades.

Spaghetti Code: lógica enredada sin estructura clara.

Golden Hammer: usar siempre la misma técnica o patrón para todo.

Lava Flow: código viejo que nadie elimina y se acumula.

Copy-Paste Programming: duplicar código en lugar de abstraer.
