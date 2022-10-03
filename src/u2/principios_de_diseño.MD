# Principios de Diseño

## Temas
- ¿Qué hace a un buen diseño?
- Calidad de software.
- Principios de Diseño.

## ¿Qué es un buen diseño?
El principio de la sabiduría de un ingeniero de software es reconocer la diferencia
entre conseguir que un programa funciones y que funcione correctamente.

## Calidad de Software - McCall's Classic Model for Software Quality Factors (1977)
![](../../resources/img/u2/McCalls_Quality_Factors.jpg)

### Operational Factors
- Correctness: Funciona y hace lo que debe hacer.
- Reliability: Que sea confiable, que no se rompa, que no se caiga, que maneje bien 
  los errores. Hace lo que debe hacer siempre.
- Efficiency: Hace lo que debe hacer lo más rápido posible y con la menor cantidad
  de recursos.
- Integrity: Que no se caiga, que no permita invasiones de memoria. 
- Usability: Fácil de interactuar, que sea intuitivo, que las capacidades del sistema
  sean fáciles de descubrir por el usuario.

### Revision Factors
- Maintainability: Codigo fácil de entender, monitoreo de software, alertas, manejo
  de errores, logs distribuidos.
- Flexibility: Adaptable a cambios futuros.
- Testability: Self explanatory.

### Transition Factors
- Portability: Que todo o parte del codigo se pueda usar en distintos hardwares.
- Reusability: Reutilizar módulos para dar soluciones a otros problemas.
- Interoperability: Que el software pueda operar con otros softwares.

## Cualidades de un buen diseño
- Compatibility: Los componentes trabajan bien entre sí.
- Extensibility: Fácil de agregar funcionalidades.
- Fault-tolerance: Maneja errores elegantemente.
- Maintainability.
- Modularity: Soporta correctamente cambios en los componentes.
- Performance: Funciona según la necesidad.
- Portability.
- Reliability.
- Reusability.
- Robustness == Integrity (no se cae y no permite invasiones de memoria)
- Scalability: Mantiene la performance conforme sube la demanda.
- Security: Solo ocurre el comportamiento deseado.
- Usability.

## Principios de Diseño - Alan M. Davis
- Evaluar más de una alternativa.
- Cada elemento tiene que ser _traceable_ a un requerimiento.
- No debe reinventar la rueda. (KISS)
- Debe minimizar la distancia intelectual entre el software y el problema a resolver.
- Debe ser uniforme e integrado.
- Debe ser fácil de cambiar. (Modularity)
- Debe mantenerse simple y evitar la proliferación de casos especiales.
- Debe poder manejar errores y situaciones no previstas de manera elegante. (Fault-tolerance)
- La calidad del diseño debe asegurarse en el momento de la construcción y no una
  vez realizado.
- El diseño deber ser revisado para minimizar errores conceptuales.
- Registrar las suposiciones y decisiones importantes.

## DRY: Don't Repeat Yourself
> Every piece of knowledge must have a single, unambiguous, authoritative 
  representation within a system. - Andy Hunt & Dave Thomas (The Pragmatic Programmer)
- Código duplicado.
- Conocimiento duplicado.
- Representaciones duplicadas.
- Duplicados entre proyectos.

## KISS: Keep It Simple, Stupid
> Un sistema complejo que funciona invariablemente se ha desarrollado a partir de 
  un sistema simple que funciona. - John Gall (1975)

> You can't write perfect software. - Andy Hunt & Dave Thomas (The Pragmatic Programmer)

## Design by Contract (Bertrand Meyer)
- Preconditions.
- Postconditions.
- Class invariants.

## Defensive Design / Programming
- Validate all input/data.
- Expect malicious input/data.
- Validate assumptions.
- Expect and handle errors.

> Good design is easier to change than bad design. - Andy Hunt & Dave Thomas (The Pragmatic Programmer)