## Variables

**val** variables de solo lectura

**var** variables mutables

```kotlin
val age = 36

var customers = 10

customers = 8

println(customers)

// 8
```

Las variables pueden declararse fuera de `main()` en la parte superior.

Es recomendable declarar variables de solo lectura con `val` y declarar variables mutables con `var` solo si es necesario.

## String templates

Se utliza para imprimir en pantalla. Se puede acceder a datos guardados en variables o otros objetos y convertilas a string. El string tiene que estar enbuelto en `""`.El template siempre comiensa con `$`.

```kotlin
val customers = 10

println("There are $customers customers")
// There are 10 customers

println("There are ${customers + 1} customers")
// There are 11 customers
```