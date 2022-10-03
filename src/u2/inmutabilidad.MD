# Inmutabilidad
## Transparencia Referencial
Una expresión es referencialmente transparente si se puede reemplazar con su valor 
correspondiente sin cambiar el comportamiento del programa.
```shell
int addOne(int i){
    return i + 1;
}
//...
int a = addOne(1) * 2;
int a = 2 * 2;
int a = 4;
```