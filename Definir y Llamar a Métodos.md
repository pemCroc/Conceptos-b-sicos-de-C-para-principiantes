# Video 9 

### Descripción breve
En este video se explica cómo definir y llamar métodos en C#. Aprendemos la importancia de los métodos para organizar el código, reducir la redundancia, mejorar la legibilidad y simplificar el mantenimiento de nuestras aplicaciones.

Los métodos son bloques de código con un nombre que encapsulan funcionalidad específica. Pueden ser reutilizados en diferentes partes de una aplicación, mejorando la eficiencia y reduciendo errores.

#### Definición Básica
Un método se define dentro de una clase y puede recibir parámetros de entrada o devolver un valor:
```csharp
private static void Saludar()
{
    Console.WriteLine("Hola, mundo!");
}
```
- **private:** Modificador de acceso. Explicado más adelante.
- **static:** Requerido para ser llamado desde `Main`.
- **void:** Indica que el método no devuelve valor.

#### Llamar un Método
Para ejecutar un método, se llama por su nombre seguido de paréntesis:
```csharp
Saludar();
```
Salida esperada:
```
Hola, mundo!
```

#### Métodos con Parámetros
Podemos pasar datos a un método usando parámetros:
```csharp
private static void Saludar(string nombre)
{
    Console.WriteLine($"Hola, {nombre}!");
}
```
Llamada del método:
```csharp
Saludar("Carlos");
```
Salida:
```
Hola, Carlos!
```

#### Métodos que Devuelven Valores
Un método puede devolver un valor usando la palabra clave `return`:
```csharp
private static int Sumar(int a, int b)
{
    return a + b;
}
```
Llamada del método:
```csharp
int resultado = Sumar(3, 4);
Console.WriteLine(resultado);
```
Salida:
```
7
```

#### Buenas Prácticas
1. **Un solo propósito:** Un método debe realizar una única tarea bien definida. Si su descripción incluye "y", considera dividirlo en dos métodos.
2. **Nombres descriptivos:** Usa nombres que expliquen claramente qué hace el método. Ejemplo: `CalcularPromedio`, `ImprimirSaludo`.
3. **Menos de seis líneas:** Mantener los métodos cortos mejora la legibilidad.
4. **Evita código duplicado:** Si necesitas repetir código, encapsúlalo en un método.

#### Sobrecarga de Métodos
Un método puede tener varias versiones con el mismo nombre pero diferentes parámetros:
```csharp
private static void MostrarMensaje(string mensaje)
{
    Console.WriteLine(mensaje);
}

private static void MostrarMensaje(string mensaje, int veces)
{
    for (int i = 0; i < veces; i++)
    {
        Console.WriteLine(mensaje);
    }
}
```
Llamadas:
```csharp
MostrarMensaje("Hola");
MostrarMensaje("Hola", 3);
```
Salida:
```
Hola
Hola
Hola
Hola
```

### Ejemplo Completo
Programa para invertir una cadena y mostrarla en pantalla:
```csharp
using System;

namespace MetodosDemo
{
    class Program
    {
        static void Main(string[] args)
        {
            string mensaje = "Hola, mundo";
            string mensajeInvertido = InvertirCadena(mensaje);
            MostrarMensaje(mensajeInvertido);
        }

        private static string InvertirCadena(string texto)
        {
            char[] caracteres = texto.ToCharArray();
            Array.Reverse(caracteres);
            return new string(caracteres);
        }

        private static void MostrarMensaje(string mensaje)
        {
            Console.WriteLine(mensaje);
        }
    }
}
```
Salida:
```
odnum ,aloH
```
