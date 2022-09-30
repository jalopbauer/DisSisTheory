# Principios de Diseño

## Modularización

### Keywords
- Functional decomposition vs. design decision decomposition
- Module (abstraction): Comprensión, coordinación, flexibilidad.
- David parnas: Information hiding and encapsulation.
- Coupling & cohesion.
- Ortogonalidad.

### Formas de modularización
- Dividir la función en sus pasos (Functional Decomposition)
- Dividir la función en decisiones de diseño: Cada sub-función oculta alguna decision 
  importante

### Definición
Dividir un programa en módulos individuales, creando barreras de abstracción bien 
definidas entre ellos.

### Beneficios
- __Comprensión__: Nos permite estudiar un módulo a la vez.
- __Coordinación__: Distintos módulos pueden ser desarrollados y mantenidos en forma 
  independiente por diferentes equipos.
- __Flexibilidad__: Debería ser posible hacer cambios a un módulo sin necesidad de cambiar
  otros.

#### ¿Qué tipos de cambios?
- Cambio de requerimientos a través del tiempo.
- Distintos usuarios que al mismo tiempo requieren diferente funcionalidad.

### Modularización segun David Parnas, 1972
- NO es simplemente dividir una función en múltiples pasos.
- __Information Hiding__: Cada módulo oculta decisiones de diseño.
- __Encapsulation__: Cada módulo expone una interfaz sin revelar detalles de implementación.
- Empezar la descomposición de un sistema por sus decisiones de diseño difíciles o que
  pueden cambiar. Luego se diseñan módulos para ocultar esas decisiones asi se separan
  del tiempo de ejecución.

### Acoplamiento
El grado en el cual los módulos se __interconectan__ o se relacionan entre ellos.

### Cohesión
El grado en el cual las componentes de un módulo son necesarios y suficientes para llevar
a cabo __una sola función__ bien definida.

### Criterio
- Alta __cohesión__ dentro de cada módulo.
- Bajo __acoplamiento__ entre módulos.

Alto acoplamiento. Baja cohesión
![](../../resources/img/u2/AltoAcop_BajaCohe.jpg)

Bajo acoplamiento. Alta cohesión
![](../../resources/img/u2/BajoAcop_AltaCohe.jpg)

### Ortogonalidad
Dos o más elementos son ortogonales si cambios en un elemento no afectan al resto.

#### Ejemplo
```scala
class Split1 {
    constructor(filename)
    def readNextLine()
    def getField(n)
}

class Split2 {
    constructor(line)
    def getField(n)
}
```

## Principios de Diseño
