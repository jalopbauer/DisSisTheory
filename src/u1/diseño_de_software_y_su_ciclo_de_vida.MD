# Diseño de software y su ciclo de vida
## Temas
- Diseño de software

## Diseño de software
Diseñar software es el proceso de definir la arquitectura, componentes y otras características del sistema para su realización. El resultado de ese proceso es el Diseño de software. 
### Decisiones de diseño
Al diseñar lo que hacemos es tomar decisiones, estas deben cumplir con los requerimienos, deben ser justificadas y comparardas entre si ya que toda decision genera trade-offs. Una decision puede ser recomendable para un contexto pero no para otro. Se tiene que empezar con las que generen una alta calidad con poco costo. Se debe tomar deciciones sin complejizar innecesariamente el propósito pautado (KISS). Hay que concentrarse en el núcleo de lo que se necesita, y postergar las ideas que requieran pensar y las implementaciones futuras lo más posible, para no encasillarse en la idea de desarrollar. Pensar en conceptos amplios.
### Restricciones a la hora de diseñar software
- Dinero
- Tiempo
- Know how del equipo de desarrollo
- Arquitectura y entorno del proyecto
- Software pre-existente
- Limitaciones de hardware
### Aspectos del diseño
- Datos: Las estructura de datos son escenciales para el software. Cualquiera puede escribir código pero se necesita experiencia y un grado de conocimiento para definir una buena estructura de datos.
- Funciones/Algoritmos
- Arquitectura
- Interfaces (integración)
- Experiencia de Usuario (UI/UX)
- Procesos: Diseñar el ciclo de vida y el flujo de alguna acción que se quiera modelar

## Ciclo de vida del software
Es el proceso que incluye el planeamiento, creación, validación y puesta en marcha de sistemas de software

### Fases
```scala
while (vos.sueldoRecibido() == True)
 analisisDeRequerimientos()
 diseño()
 codificacion()
 pruebas()
 desplegarMantener()
```
### Modelos de ciclo de vida del software
#### Cascada/Waterfall

![Diagrama modelo en cascada](/resources/img/u1/diagrama_software_cascada.png)

El costo de un error en todo el flujo, aumenta en forma exponencial conforme avanzamos en las etapas del ciclo.

#### Iterativo

![Diagrama modelo iterativo](/resources/img/u1/diagrama_software_iterativo.png)

Se llevan múltiples iteraciones en cascada a partir de un primer MVP para largar un prototipo que puedan probar los clientes. Se busca tener un feedback constante y rapido. Un error comun al seuir este modelo es que al hacer nuevas feaures no se tienen encuenta patrones o soluciones reutilizables.

#### Espiral (Boehm, 1988)

![Diagrama modelo Boehm](/resources/img/u1/diagrama_software_boehm.png)

Es igual a simple iterativo

#### Unified Process

![Diagrama modelo unified process](/resources/img/u1/diagrama_software_unified_process.webp)

Este modelo lo que denota es que a medida que avanza el proyecto, el esfuerzo relativo de cada disciplina va variando. Se puede hacer tanto en cascada o iterativo.

#### Otros
- Evolutivo
- Basado en prototipos
- Modelo en “V”
- “Ágiles”

