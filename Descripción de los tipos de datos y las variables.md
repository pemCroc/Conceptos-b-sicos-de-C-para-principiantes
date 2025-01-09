# Video 5 

### Descripción breve
En este video se explican los conceptos fundamentales de las variables en C#, cómo declarar y asignar valores, los diferentes tipos de datos y buenas prácticas para trabajar con ellas en programas simples.

Las variables en C# son como "buckets" en la memoria del computador. Estos "buckets" pueden almacenar diferentes tipos de datos según nuestras necesidades, como números, cadenas de texto, fechas y más. Para usarlas correctamente, debemos declarar el tipo de dato que contendrán y asignarles un nombre descriptivo.

#### Declaración y Asignación de Variables
- Para declarar una variable, indicamos el tipo de dato y le damos un nombre:
  ```csharp
  int x; // Declara una variable llamada x que contiene un número entero.
  ```
- La asignación de valores usa el operador `=`:
  ```csharp
  x = 7; // Asigna el valor 7 a x.
  ```
- También podemos declarar y asignar en una sola línea (inicialización):
  ```csharp
  int y = x + 3; // Declara y asigna a y el valor de x + 3.
  ```

#### Ejemplo Básico
Este programa suma dos números y muestra el resultado:
```csharp
using System;

namespace VariablesDemo
{
    class Program
    {
        static void Main(string[] args)
        {
            int x = 7;
            int y = x + 3;
            Console.WriteLine(y); // Muestra "10" en la consola
            Console.ReadLine();   // Pausa la ejecución hasta que el usuario presione Enter
        }
    }
}
```

#### Tipos de Datos Comunes en C#
- **int:** Almacena números enteros (sin decimales), por ejemplo, 7.
- **string:** Almacena cadenas de texto, como "Hola, mundo".
- **double:** Almacena números con decimales, como 3.14.
- **bool:** Almacena valores lógicos (true o false).

#### Operadores Importantes
- **Operador de asignación (`=`):** Asigna un valor a una variable.
- **Operador aritmético (`+`):** Suma valores o concatena cadenas:
  ```csharp
  string saludo = "Hola, " + "mundo"; // Resultado: "Hola, mundo"
  ```

#### Buenas Prácticas
1. Usa nombres descriptivos para las variables. Ejemplo:
   ```csharp
   string primerNombre; // Mejor que "x" o "var1".
   ```
2. Sigue la convención "camel case" para los nombres (primer palabra en minúsculas, las siguientes con mayúscula inicial).
3. Declara y asigna valores lo antes posible para mantener las variables en un "estado válido".

#### Ejemplo Interactivo: Preguntar Nombre
Un programa que solicita al usuario su nombre y lo saluda:
```csharp
using System;

namespace NombreDemo
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("¿Cuál es tu nombre?");
            Console.Write("Escribe tu primer nombre: ");
            string primerNombre = Console.ReadLine();

            Console.Write("Escribe tu apellido: ");
            string apellido = Console.ReadLine();

            Console.WriteLine("Hola, " + primerNombre + " " + apellido + "!");
            Console.ReadLine();
        }
    }
}
```

Este ejemplo introduce el tipo `string` y cómo usar `Console.ReadLine()` para capturar entradas del usuario.

### Notas Importantes
- **Camel Case:** Usa mayúscula para la primera letra de cada palabra, excepto la primera. Ejemplo: `miPrimerNombre`.
- **Precisión:** C# es sensible a mayúsculas y minúsculas (`nombre` es diferente de `Nombre`).
- **Evitar Nombres Duplicados:** Cada variable debe tener un nombre único dentro del mismo bloque de código.

