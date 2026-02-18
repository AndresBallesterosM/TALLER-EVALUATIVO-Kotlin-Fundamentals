# Taller Evaluativo — Kotlin Fundamentals

# Nombre: Carlos Andrés
# Fecha: 17/02/2026

1. ¿Cuál es la diferencia entre val y var?

val es inmutable (no se puede reasignar).
var es mutable (sí se puede cambiar su valor).

val nombre = "Andrés"
var edad = 20
edad = 21

2. ¿Qué es la interpolación de strings?

Es insertar variables dentro de un texto usando $.

val nombre = "Ana"
println("Hola soy $nombre")

3. ¿Qué es una función?

Es un bloque de código reutilizable que realiza una tarea específica y ayuda a organizar el programa.

4. Diferencia entre función que retorna valor y Unit

Una retorna un resultado; la otra solo ejecuta una acción.

fun sumar(a: Int, b: Int): Int = a + b
fun saludar() { println("Hola") }

5. Menciona 4 tipos de datos en Kotlin

Int

Double

String

Boolean

6. Ejemplo de if/else que clasifique una nota
fun clasificar(nota: Int): String {
    return if (nota >= 90) "A"
    else if (nota >= 80) "B"
    else if (nota >= 70) "C"
    else "D"
}

7. ¿Cuándo usar when?

Cuando hay múltiples condiciones o rangos, porque es más limpio y legible que muchos if.

8. Diferencia entre String y String?

String no permite null.
String? sí permite null.

9. ¿Qué es el safe call (?.)?

Permite acceder a algo solo si no es null.

val texto: String? = null
println(texto?.length)

10. ¿Qué es el operador Elvis (?:)?

Da un valor por defecto si la variable es null.

val nombre: String? = null
val resultado = nombre ?: "Invitado"

11. ¿Qué es una clase y un objeto?

Una clase es una plantilla.
Un objeto es una instancia de esa clase.

class Persona(val nombre: String)
val p1 = Persona("Ana")

12. ¿Qué son propiedades y métodos?

Propiedades: características del objeto.
Métodos: acciones del objeto.

13. ¿Qué es una lambda?

Es una función sin nombre que puede guardarse en una variable.

val doble: (Int) -> Int = { x -> x * 2 }

14. ¿Qué es una función de orden superior?

Es una función que recibe otra función como parámetro.

fun operar(a: Int, b: Int, op: (Int, Int) -> Int): Int {
    return op(a, b)
}

15. ¿Qué ventaja tiene Kotlin al manejar nullabilidad desde el tipo?

Reduce errores como NullPointerException y hace el código más seguro.





