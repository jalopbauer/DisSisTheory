# Complejidad
### Definición: Condición de Complejo
1. Que está compuesto por muchos y variados elementos; que implica gran cantidad de aspectos muy 
   diversos; que involucra numerosas funciones o relaciones.
2. Que resulta difícil de entender, resolver, usar, etc., por estar constituido por muy diversos
   elementos o por implicar aspectos muy variados.
   
## “No silver Bullet” → Fred Brooks

### Complejidad de software es una propiedad Esencial
- La complejidad es el problema base del desarrollo de Software.
- De la complejidad vienen:
  - Dificultad en la comunicación entre el equipo.
  - Complejidad para entender el programa.
  - Complejidad para entender las funciones del programa.
- “Un problema que ocurra en el desarrollo conduce a más problemas luego.”

### Accidentales
Dificultades que hoy en dia se presentan en la producción de software pero que no son inherentes al mismo, es decir que 
son dificultades que no tiene que ver con el problema a resolver sino con el lenguaje elegido, el hardware.

### Propiedades esenciales
Complexity: dificultad propia del poder diseñar y entender el software, crece de manera no lineal. Ej: la cantidad de
líneas de codigo no es lineal a la complejidad. 
- Conformity: el software se tiene que adaptar a interfaces de sistemas y reglas hechas por otras personas de manera 
  arbitraria. Tiene que adaptarse también a la vida real y el ámbito del proyecto. Debe adaptarse a las realidades
  (instituciones humanas, por ej)
- Changeability: condición que hace que el software sea propenso al cambio debido a avances tecnológicos de hardware 
  o cambio de especificaciones.
- Invisibility: no se puede representar de forma visible todo el software completo.

### Mejoras encontradas
- High-Level languages: elimina una capa de complejidad que permite hacer un mejor enfoque en el diseño en sí.
- Time-Sharing: compartir recursos computacionales para aumentar la 
  productividad. Hoy en día se corren muchas aplicaciones al mismo tiempo en un mismo dispositivo.
- Unified Programming Environments: poder usar programas integrados entre sí que facilitan el uso.
 
### Silver Bullets:
- Ada´s high-level advances: su contribución fue que ayudó a entrenar a programadores con diseño
 de software moderno.
- Object-Oriented Programming: ayudó a remover todas las dificultades accidentales así no 
 interponerse con el diseño.
- Artificial Intelligence: eso podría ayudar, pero para resolver ciertos problemas se busca 
 creatividad y abstracción que la A.I. aún no alcanzó.
- Expert Systems: podrían ayudar en distintas formas de testeo o debugeo, sugiriendo o haciendo
 en el momento, pero no en la creación en sí.
- Automatic programming: la creación de un programa para realizar otros programas. Pero para 
 esto se le debe pasar la solución del programa y no la especificación.
- Graphical programming: la realización de flow-charts. Lo que ocurre es que estos van cambiando
 o se realizan a medida que se programa.
- Program Verification: programar sin bugs o errores desde el inicio. Muy difícil de alcanzar, 
 parte de la programación es resolver errores mediante el debugeo.
 
### Promesas para simplificar - Ataques prometedores
- Buy VS Build: el costo siempre es del desarrollo y no el de replicación. Tener en cuenta la compra 
 del software es una opción válida, esto representa menos costos, menos riesgo y se evita el desarrollo.
- Requirements Refining and Rapid Prototyping: obtener un prototipo que simule las interfaces importantes y 
 realice las funciones principales del sistema. Extraer y refinar los requerimientos del producto.
- Incremental Development: crear iteraciones del software e ir mejorándolas y agregando funcionalidades.
- Great Designers: se llegan a buenos diseños siguiendo las buenas prácticas. Y son los buenos diseñadores quienes 
 saben aplicarlas. Por eso se les debe proveer oportunidades para crecer y reconocer su importancia para el éxito. 
 Cuidar a los empleados, darles un buen entorno de trabajo, etc.

## “Out of the Tar Pit” → Ben Moseley & Peter Marks
- Los autores piensan que la única significante de las 4 propiedades de sistemas es la COMPLEJIDAD,
  ya que las otras pueden ser clasificadas como tipos de complejidad o pueden verse como 
  problemáticas solo por la complejidad del sistema.

### Complejidad: Raíz de todos los problemas 
Mientras más complejo más difícil de entender y más errores a la hora de editar el proyecto.
- “La simplicidad es difícil” 

### Caminos para entenderlo
Existen varios mecanismos que se usan comúnmente para entender sistemas complejos. Dos de los más
usados son “Testing” e “Informal Reasoning”.
- Testing: este mecanismo es utilizado para ver el sistema desde afuera, cómo funciona. 
 Demuestra cómo el sistema responde ante diferentes situaciones específicas. Testing puede 
 hacerse tanto por un humano (más común para probar todo el sistema) como por la máquina en sí
 (comúnmente para probar componentes individuales).
- Informal Reasoning: este mecanismo es para tratar de entender el sistema desde adentro. 
 Lo esperado es que al usar información extra se puede llegar a un entendimiento más certero. 

### Causas de la complejidad
- Complexity caused by State: La complejidad que viene a partir de la cantidad de estados que 
  tiene el programa. 
- Impact of State on Testing: La cantidad de estados en el sistema es muy grande para poder 
  testear todo.
- Impact of State on Informal Reasoning: Como pasa con Testing, el aumento de estados es muy 
  exponencial para poder comprender cada uno de ellos.
- Complexity caused by control: Control es el orden en el cual pasan las cosas. El problema es 
  que cuando el control es una parte del lenguaje (lo cual usualmente es) toda parte del 
  programa se tiene que entender en ese contexto asi que el control suma a la complejidad del 
  programa.
- Complexity caused by Code Volume: tener código muy voluminoso aumenta la dificultad de Testear 
  y utilizar el Informal Reasoning, entonces aumenta la complejidad del código en una forma no 
  lineal.
- Complexity breeds complexity: son todas las complejidades que se crean a raíz de no entender 
  la complejidad original del código. 
- Simplicity is hard: no siempre existe una forma simple de simplificar el código.
- Power corrupts: Mientras mas poderoso es el lenguaje, osea mientras mas libertades tiene el lenguaje, mas dificil es de entender los sistemas construidos con el.
 
### Formas clásicas de manejar la Complejidad
- Object Orientation Programming: Los lenguajes orientados a objetos sufren mucho de ambas, 
  complejidad derivada de estados como complejidad derivada de control. 
- Functional Programming: Los lenguajes funcionales evitan muy bien los problemas de 
  complejidad derivada por estados lo cual tiene grandes beneficios en el momento de testear 
  el sistema.
- Logic Programming: A pesar de las limitaciones que tienen algunos lenguajes lógicos de 
  programación, la programación lógica habilita al programador a escapar de las complejidades 
  causadas por el control. 
 
### Accidentes y Esencia
#### Tipos de Complejidad
- Complejidad Esencial: es la complejidad heredada de y la esencia del problema. (visto por el 
  usuario)
- Complejidad Accidental: es la complejidad de todo lo demás. Es la complejidad que en un mundo 
  ideal los desarrolladores no tendrían que arreglar.
  
Cuando se trata de ambos tipos de complejidad los autores creen que es el objetivo de todo 
ingeniero informático el de eliminar lo más posible, para llegar a un sistema final más simple.
