# Manejo de Errores y Excepciones

### Entendiendo Errores y Excepciones
1. **Entendiendo Errores y Excepciones**
   - **Errores:** Problemas en un programa que causan que se detenga. Ejemplos incluyen errores de sintaxis y errores de tiempo de ejecución.
   - **Excepciones:** Errores detectados durante la ejecución. No son fatalmente incondicionales (es decir, puedes manejarlos y mantener tu programa en funcionamiento).

### Bloques Try y Except
2. **Bloques Try y Except**
   - **Propósito:** Manejar excepciones. El código que podría generar una excepción se coloca dentro del bloque `try`. Si ocurre un error, se ejecuta el código en el bloque `except`.
   - **Ejemplo:**
     ```python
     try:
         resultado = 10 / 0
     except ZeroDivisionError:
         print("¡No puedes dividir por cero!")
     ```
     Si el bloque `try` causa un `ZeroDivisionError`, se ejecuta el bloque `except`.

### Manejo de Múltiples Excepciones
3. **Manejo de Múltiples Excepciones**
   - Puedes definir múltiples bloques `except` para manejar diferentes excepciones.
   - Ejemplo:
     ```python
     try:
         # algún código que puede generar diferentes excepciones
     except ZeroDivisionError:
         # manejar excepción de división por cero
     except ValueError:
         # manejar excepción de error de valor
     ```

### Cláusula Finally
4. **Cláusula Finally**
   - **Propósito:** El bloque `finally` te permite ejecutar código, independientemente del resultado de los bloques `try` y `except`.
   - **Ejemplo:**
     ```python
     try:
         resultado = 10 / 0
     except ZeroDivisionError:
         print("¡División por cero!")
     finally:
         print("Esto se ejecuta pase lo que pase")
     ```
     El bloque `finally` es un buen lugar para poner código que debe ejecutarse independientemente de si ocurrió una excepción o no, como cerrar un archivo o liberar recursos.

Entender cómo manejar errores y excepciones es esencial en Python, ya que ayuda a escribir programas robustos que pueden anticipar y tratar con situaciones inesperadas durante la ejecución. Este enfoque permite que el programa responda a los errores de manera elegante en lugar de colapsar inesperadamente.
