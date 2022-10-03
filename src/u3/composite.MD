# Composite
## Definicion
Componer objetos en estructuras de árbol para representar jerarquías, el cliente de nuestro modelo trate a los objetos de forma homogénea.

Leaf --> Component

Composite --> Component

## Consecuencias

- Composición recursiva
- Simplifica al Cliente
- Unificación de interfaz
- Evitamos Ifs/cases
- Fácil agregar componentes
- El diseño es muy general, no tengo muchas limitaciones. 
- Dificil restringir componentes en un contenedor y operaciones

## Formas de implementación:
- Para matener uniformidad.
    - Todos los metodos tienen implementaciones default en el Component
- Para seguridad de tipado.
    - Solo el Composite tiene los metodos para componer Componentes.
