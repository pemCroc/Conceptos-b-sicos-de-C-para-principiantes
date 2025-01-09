# Video 6

### Descripción breve
En este video aprendemos a usar la instrucción `if` para tomar decisiones en nuestro código. Se introducen las estructuras `if`, `else if`, y `else` para manejar condiciones y ejecutar bloques de código específicos según el resultado de evaluaciones lógicas.

La instrucción `if` permite que nuestro programa elija entre diferentes bloques de código basándose en una condición que puede ser verdadera o falsa. Esto es útil para realizar decisiones dinámicas en función de datos como la entrada del usuario.

#### Sintaxis Básica
```csharp
if (condicion)
{
    // Código que se ejecuta si la condición es verdadera
}
else if (otraCondicion)
{
    // Código que se ejecuta si `otraCondicion` es verdadera
}
else
{
    // Código que se ejecuta si ninguna condición anterior es verdadera
}
```

#### Ejemplo: Juego de Elección
Este programa pide al usuario elegir una puerta y muestra un premio según su elección:
```csharp
using System;

namespace DecisionDemo
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Elige una puerta: 1, 2 o 3");
            string eleccionUsuario = Console.ReadLine();
            string mensaje;

            if (eleccionUsuario == "1")
            {
                mensaje = "¡Ganaste un auto nuevo!";
            }
            else if (eleccionUsuario == "2")
            {
                mensaje = "¡Ganaste un barco!";
            }
            else if (eleccionUsuario == "3")
            {
                mensaje = "¡Ganaste un gato!";
            }
            else
            {
                mensaje = "Lo sentimos, no entendimos tu elección.";
            }

            Console.WriteLine(mensaje);
            Console.ReadLine();
        }
    }
}
```

#### Detalles Importantes
1. **Operadores de Comparación:**
   - `==`: Verifica si dos valores son iguales.
   - `!=`: Verifica si dos valores son diferentes.
2. **Bloques de Código:**
   - Las llaves `{ }` delimitan los bloques de código. Si un bloque tiene una sola línea, las llaves son opcionales.
   - Sin llaves:
     ```csharp
     if (condicion)
         Console.WriteLine("Hola");
     ```
3. **Else "catch-all":** El bloque `else` es una solución para manejar casos no contemplados en las condiciones `if` o `else if` anteriores.

#### Operador Condicional (Ternario)
El operador condicional permite evaluar condiciones en una sola línea:
```csharp
string mensaje = (eleccionUsuario == "1") ? "Ganaste un auto" : "Ganaste algo más";
Console.WriteLine(mensaje);
```
- La estructura es: `condicion ? valorSiVerdadero : valorSiFalso`.

#### Ejemplo de Formato en Salida
Para mejorar la salida del programa, podemos usar códigos de reemplazo:
```csharp
Console.WriteLine("Elegiste {0}, por lo tanto ganaste {1}", eleccionUsuario, mensaje);
```
Esto reemplaza `{0}` con `eleccionUsuario` y `{1}` con `mensaje`.

### Buenas Prácticas
- Declara variables fuera de los bloques `if` si las necesitas después.
- Usa nombres de variables descriptivos para mejorar la legibilidad del código.
- Mantén el código limpio eliminando redundancias y reutilizando variables cuando sea posible.

Con el operador condicional y técnicas de formato, podemos escribir código compacto y fácil de leer. Este video nos introduce a la importancia de manejar condiciones en el desarrollo de software.

