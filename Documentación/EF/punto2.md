
# Variables y Tipos de Datos
## Entendiendo los Diferentes Tipos de Datos

### Tipos de Datos
En Python, cada valor tiene un tipo de dato. Los tipos más comunes son enteros (int), números de punto flotante (float), cadenas de texto (str) y booleanos (bool).
- **Enteros (int)**: Son números completos sin punto decimal, como 3, 100 o -15.
- **Números de Punto Flotante (float)**: Son números con punto decimal, como 3.14, 2.0 o -0.001.
- **Cadenas de Texto (str)**: Datos textuales encerrados en comillas simples ('...') o dobles ("..."), como "Hola" o 'Python'.
- **Booleanos (bool)**: Representan valores Verdadero o Falso, a menudo utilizados en declaraciones condicionales.

## Declarando y Usando Variables

### Variables
Una variable en Python es un lugar nombrado utilizado para almacenar datos en la memoria. A diferencia de otros lenguajes, en Python, no necesitas declarar el tipo de dato de una variable; se infiere del valor asignado a ella.
- **Declarando Variables**: Simplemente asigna un valor a un nombre de variable:
  ```python
  x = 10         # Asignación de un entero
  y = 3.14       # Asignación de un número de punto flotante
  nombre = "Alice" # Una cadena
  es_valido = True # Un valor booleano
  ```
- **Tipado Dinámico**: Python te permite reasignar un tipo de dato diferente a una variable. Por ejemplo:
  ```python
  x = 10
  x = "Diez"
  ```
  Aquí, x primero fue un entero, luego se reasignó como una cadena.

### Usando Variables

- **Accediendo a Variables**: Puedes usar el

valor almacenado en una variable simplemente usando el nombre de la variable.
  Ejemplo:
  ```python
  saludo = "Hola, "
  nombre = "Alice"
  print(saludo + nombre) # Salida: Hola, Alice
  ```
- **Variables Sensibles a Mayúsculas y Minúsculas**: En Python, los nombres de las variables son sensibles a mayúsculas y minúsculas, lo que significa que `nombre`, `Nombre` y `NOMBRE` son variables diferentes.

Entender las variables y los tipos de datos es fundamental en Python, ya que forma la base de la manipulación de datos y el cálculo. Experimentar con diferentes tipos de datos y variables profundizará tu comprensión y competencia en la programación de Python.
