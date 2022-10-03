# Singleton
Solo haya una instancia de una clase.
## Implementaciones
### Eager
Tener la instancia cuando se crea la clase. El problema es que si hay más de un hilo de ejecución puede fallar ya que si ambos llaman getInstance al mismo tiempo explota todo. Si no se usa 
### Lazy
Solo se instancia al pedirlo y solo si la instancia es null. El problema es que si hay más de un hilo de ejecución puede fallar ya que si ambos llaman getInstance al mismo tiempo explota todo.
### Lazy “synchronized”
Muy parecida a la lazy pero con el agregado de asegurarse de que cada hilo tenga una instancia asignada, el problema de esta es que genera mucho código, haciéndolo costoso e ineficiente.
### Lazy “double-check locking” 
Se hace un doble chequeo con synchronized dentro del bloque, pero no funciona en el caso de java se soluciona usando volatile.
