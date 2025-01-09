# Video 4

### Descripción breve
En este video se explica cómo crear y ejecutar un programa básico en C#, conocido como "Hello World". Se introduce el flujo de trabajo fundamental que se seguirá para desarrollar aplicaciones en este lenguaje.

El objetivo del ejercicio es familiarizarnos con los pasos básicos para crear, escribir y ejecutar un programa en C#. Aunque no se profundiza en los conceptos técnicos, se establecen las bases del proceso de desarrollo.

#### Pasos para Crear el Programa
1. **Crear un nuevo proyecto:**
   - Ve a **File > New > Project** en Visual Studio.
   - Selecciona **C#** y luego el tipo de proyecto **Console Application**.
   - Nombra el proyecto "HelloWorld" (sin espacios, usando mayúsculas en cada palabra).

2. **Escribir el código:**
   - Ubica las llaves internas `{ }` del método `Main` dentro del archivo `Program.cs`.
   - Escribe las siguientes líneas de código:

```csharp
Console.WriteLine("Hello, World!"); // Imprime el mensaje en la consola
Console.ReadLine(); // Espera a que el usuario presione Enter
```

3. **Guardar el proyecto:**
   - Usa **File > Save All** para guardar todos los cambios.

4. **Ejecutar el programa:**
   - Haz clic en el botón verde **Start** o ve a **Debug > Start Debugging**.
   - Deberías ver "Hello, World!" en la ventana de la consola.

#### Errores Comunes y Soluciones
- **Error: Falta un punto y coma (`;`).**
  - C#: Todas las instrucciones deben terminar con `;`.
  
- **Error: No se encuentra `Console`.**
  - Solución: Asegúrate de que las palabras están escritas correctamente, respetando las mayúsculas y minúsculas.
  - Ejemplo correcto: `Console.WriteLine` (no `console.writeline`).

- **Error: Texto sin comillas dobles.**
  - El texto literal debe estar entre comillas dobles (").
  - Ejemplo correcto: `"Hello, World!"`.

- **Error: Código fuera de lugar.**
  - Asegúrate de que las instrucciones estén dentro de las llaves `{ }` del método `Main`.

#### Buenas Prácticas
- **Ser preciso:** C# es sensible a mayúsculas y minúsculas. Un error menor en la escritura puede generar problemas.
- **Aprovechar Visual Studio:** Las herramientas como la autocorrección y los colores ayudan a identificar errores y escribir código más rápido y preciso.

#### Estructura Final del Programa
```csharp
using System; // Importa el espacio de nombres necesario

namespace HelloWorld
{
    class Program
    {
        static void Main(string[] args)
        {
            Console.WriteLine("Hello, World!");
            Console.ReadLine();
        }
    }
}
```


