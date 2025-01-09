# Video 3 

### Descripción breve
En este video se analiza el primer programa escrito en C#, explicando los conceptos básicos y fundamentales para comprender cómo funciona el código. Estas notas resumen las ideas clave y los puntos importantes de la lección.

### Contenido de la Nota
Cuando escribimos aplicaciones en C#, no solo aprendemos la sintaxis (como los nombres, verbos y puntuación), sino también aprovechamos funcionalidades preexistentes del .NET Framework, que es un conjunto de herramientas y librerías creadas por Microsoft. Este Framework tiene dos partes principales:

1. **Class Library:** Una librería de código que facilita tareas comunes como trabajar con texto, fechas, cálculos matemáticos, mostrar información en pantalla o manejar datos a través de la red. Por ejemplo, cuando usamos `Console.WriteLine()` para imprimir algo en pantalla, estamos llamando a un método predefinido en esta librería.

2. **Runtime (CLR):** Un entorno donde se ejecuta nuestra aplicación. Este runtime abstrae detalles complejos como la gestión de memoria o la interacción con el hardware, y también protege el sistema del usuario de posibles acciones maliciosas.

En el programa que escribimos, usamos dos métodos clave:

```csharp
Console.WriteLine("Hola, mundo!"); // Imprime "Hola, mundo!" en la consola
Console.ReadLine(); // Pausa la ejecución del programa hasta que el usuario presione Enter
```

Si quitáramos `Console.ReadLine();`, el programa terminaría de ejecutarse inmediatamente, sin dar tiempo a ver el resultado.

### Conceptos Clave
- **Comentarios en el código:** Usamos `//` para comentar una línea. Esto permite ignorar código temporalmente o agregar notas para futuras referencias sin eliminar las instrucciones.
  ```csharp
  // Esto es un comentario
  Console.WriteLine("Este código se ejecutará");
  ```
- **Posición del código:** El código debe escribirse dentro de los bloques de llaves `{ }` correspondientes. Si colocamos código fuera de estos bloques, el programa generará un error.

- **Métodos y clases:**
  - Un método (como `Main`) es un bloque de código que realiza una tarea específica. `Main` es el primer método que se ejecuta en un programa.
  - Los métodos están contenidos en clases (como `Program`), que organizan el código.
  - Las clases están contenidas en namespaces, que también organizan el código a un nivel más amplio.

Un ejemplo completo del programa podría ser:

```csharp
using System; // Namespace necesario para usar la clase Console

namespace HolaMundo
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hola, mundo!"); // Imprime el mensaje
            Console.ReadLine(); // Pausa la ejecución
        }
    }
}
```

### Símbolos Importantes
- **Punto y coma (`;`)**: Indica el final de una instrucción en C#. Es como un punto en un idioma natural.
- **Paréntesis (`()`):** Usados para invocar métodos. Pueden contener argumentos (datos que pasamos al método).
- **Llaves (`{ }`):** Definen bloques de código.

### Otros Detalles
El editor de código (como Visual Studio) usa colores y sangrías automáticas para mejorar la legibilidad del código. Aunque estos detalles no afectan cómo se ejecuta el programa, ayudan a organizar y entender el código más fácilmente.

Este video sienta las bases para comprender cómo se estructura el código en C# y cómo interactuamos con las herramientas que el lenguaje nos proporciona. Es una buena introducción para entender la lógica detrás de lo que escribimos y ejecutamos.

