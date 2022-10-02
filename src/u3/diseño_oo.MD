# Diseño OO
## Conceptos escenciales
Un conjunto de entidades (objetos) que se envían mensajes (llamados a los objetos, peticiones, llamados a los métodos) entre sí y tienen responsabilidades, y para cumplirlas utilizan métodos (interpretación del mensaje).
## Core de OO
Alan Kay: “OOP to me means only messaging, local retention and protection and hiding of state-process, and extreme late-binding of all things."

Only messaging: Message passing
local retention and protection and hiding of state-process: Encapsulation
extreme late-binding:Dynamic binding

## Beneficios
- Escalabilidad en respecto a la complejidad del problema a resolver
- Provee tecnicas de abstraccion que se usan dia a adia para resolver problemas
- Los noobs pueden agarrar los conceptos basicos de OOP facil
- La idea de componentes reutilizables es una idea comercial facil de comprar

## Los pilaresn't de OO
### Abstraccion
La abstraccion es el reconocimiento de similitudes entre ciertos objetos, situaciones o procesos y de concentrarse en estas similitudes e
ignorar por el momento las diferencias. Cuando abstraemos la forma en que la abstraccion esta implementada es irrelevante. Abstraer no genera impresicion sino un nivel semantico para ser absolutamente preciso. La abstraccion de objetos en un programa puede ser diferente a la de otro, sujeta al espectador.
### Encapsulamiento
Es una técnica para compartimentar los elementos de una abstracción que constituyen su estructura y comportamiento. Impide que clientes de una estructura de datos puedan "corromper" o "violar" su estructura interna. Desacopla el codigo externo de la implementacion interna del objeto. Facilita hacer cambios de la implementacion.
### Herencia
Mecanismo de basar un objeto o clase en otro objeto o clase.
#### Herencia basada en clases
Las clases son definidas con anterioridad, os objetos son instanciados a
partir de las clases.
#### Herencia basada en prototipos
Reutilización de objetos existentes que son usados como prototipos. Se pueden clonar y extender.
#### Tipos de herencia
- Herencia de tipos
- Herencia de comportamiento
- Herencia múltiple
### Encapsulamiento
Poder brindar una misma interfaz a entidades de distinto tipo. Hay dos tipos estatico o dinamico. Dinamico puedo llamar funcionalidad sin que el objeto este creado.
## Composición
- Asociación: colaboración general
- Agregación: “contiene a”. si mato al contenedor el a no muere.
- Composición: “es parte de”. si mato al de muere el es.
## Rcomendaciones 
- Cada objeto pocas responsabilidades
- programar contra interfaces
- Hace esto no dame esto
- Encapsular implementaciones, lo que varia
- Objetos inmutables
- Alta cohesión y bajo acoplamiento
- Refactorizar refactorizar refactorizar.
