## Basic types

Toda variable y estructura tiene un tipo. El tipo es importante en kotlin por que le dice al compilador que funcion y propocito tiene.

Kotlin es capas de poder inferir el tipo de data que se asigna a una variable.

```kotlin
var customers = 10

customer = 8
customers = customers + 3 // 11
customers += 7 // 18
customers -= 3 // 15
customers *= 2 // 30
customers /= 3 // 10

println(customers) // 10
```

Kotlin tiene diferentes tipos basicos

| Category               | Basic types                      | Example                                             |
|------------------------|----------------------------------|-----------------------------------------------------|
| Integers               | `Byte`, `Short`, `Int`, `Long`    | `val year: Int = 2020`                             |
| Unsigned integers      | `UByte`, `UShort`, `UInt`, `ULong`| `val score: UInt = 100u`                           |
| Floating-point numbers | `Float`, `Double`                | `val currentTemp: Float = 24.5f`, `val price: Double = 19.99` |
| Booleans               | `Boolean`                         | `val isEnabled: Boolean = true`                    |
| Characters             | `Char`                            | `val separator: Char = ','`                        |
| Strings                | `String`                          | `val message: String = "Hello, world!"`            |


Declara una variable sin inicializar. Especifica el tipo. `:`

```kotlin
// Variable declarada sin inicializar
val d: Int
// Variable inicializada
d = 3

// Variable explicita y inicializada
val e: String = "Hello"
```

si no se inicializa la variable antes de ser leida se mostrara un error.

```kotlin
val d: Int

println(d)

// output Variable 'd' must be initialized.
```

```kotlin
// Examples
fun main() {
    val a: Int = 1000 
    val b: String = "log message"
    val c : Double = 3.14
    val d : Long = 100_000_000_000_000
    val e : Boolean = false
    val f : Char = '\n'
}
```