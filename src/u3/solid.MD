# SOLID
## S:SR:Single Responsability(Agrupar)
Agrupar el codigo por responsabilidades
## O:OC:Open closed(Extender/Modificar)
El codigo me permita agregar comportamiento sin modificar el codigo
## L:LS:Liskov substitution principle(Reemplazar)
Si A extiende de B debo poder reemplazar A por B en cualquier lugar. La clase hija no puede tener precondiciones más 
estrictas. Pero las postcondiciones si pueden ser más estrictas.
## I:IS:Interface segregation(Comportamiento Innesecario)
No tengo que tener un comportamiento innecesario porque dependo de una interfaz.
## D:DI:Dependency inversion(Implementacion NO/ Interfaz SI)
No debo depender de una implementación sino de una interfaz.