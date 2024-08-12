## Lists

Las listas guadan items en orden en el que fueron agregados y permite duplicados.

Para crear una lista(**List**) se usa **listOf()** esto crea una lista de solo lectura.

Para crear una lista(**List**) mutable se usa **MutableListOf()** esto permite modificar la lista.


```kotlin
// lista de solo lectura
val readOnlyShapes = listOf("triangle", "square", "circle")
println(readOnlyShapes)
// [triangle, square, circle]

// Lista mutable con declaracion explisita
val shapes: MutableList<String> = mutableListOf("triangle", "square", "circle")
println(shapes)
// [triangle, square, circle]
```

para evitar modificaciones inesperadas se puede crea una lista de solo lectura y asignala a una lista mutable.


```kotlin
val shapes: MutableList<String> = mutableListOf("triangle", "square", "circle")
val shapesLocked: List<String> = shapes
```

 a esto se le conoce como casting.

 para poder acceder a un elemento de una lista se hace atravez de su index.

```kotlin
val readOnlyShapes = listOf("triangle", "square", "circle")
println("The first item in the list is: ${readOnlyShapes[0]}")
// The first item in the list is: triangle
```

para poder obtener el primer elemento de la lista se usa **.first()** y para el ultimo se utiliza **.last()**

para contar el numero de elementos dentro de una lista se usa **.count()**

```kotlin
val readOnlyShapes = listOf("triangle", "square", "circle")
println("This list has ${readOnlyShapes.count()} items")
// This list has 3 items
```

para saber si un elemento esta dentro de una lista se usa **in**

```kotlin
val readOnlyShapes = listOf("triangle", "square", "circle")
println("circle" in readOnlyShapes)
// true
```

para agregar o remover elementos de una lista mutable se usa **.add()** y **.remove()**

```kotlin
val shapes: MutableList<String> = mutableListOf("triangle", "square", "circle")
// Add "pentagon" to the list
shapes.add("pentagon") 
println(shapes)  
// [triangle, square, circle, pentagon]

// Remove the first "pentagon" from the list
shapes.remove("pentagon") 
println(shapes)  
// [triangle, square, circle]
```