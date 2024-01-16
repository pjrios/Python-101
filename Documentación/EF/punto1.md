# Sintaxis y Semántica en Python

## Fundamentos de la Sintaxis de Python

### Sintaxis de Python
La sintaxis de Python se refiere al conjunto de reglas que definen cómo se escribirá e interpretará un programa en Python (tanto por el lector como por el propio Python). A diferencia de muchos otros lenguajes, Python enfatiza la legibilidad y la simplicidad.
Ejemplo: En Python, puedes imprimir una cadena en la consola con una simple instrucción: `print("Hola, Mundo!")`. Observa el uso de paréntesis y comillas, que son partes esenciales de la sintaxis de Python.

### Entendiendo la Indentación

#### Indentación
Python utiliza la indentación para definir bloques de código. A diferencia de otros lenguajes de programación que utilizan llaves `{}` o palabras clave, Python usa espacios en blanco (espacio o tabulación).
Ejemplo: En un bloque if-else de Python, la indentación aclara qué declaraciones son parte de la condición if y cuáles no:
```python
if True:
    print("Esto es verdad.")
else:
    print("Esto no es verdad.")
```
Las declaraciones bajo if y else están indentadas, mostrando que pertenecen a estas condiciones.

### Comentarios y Docstrings

#### Comentarios
En Python, puedes escribir comentarios usando el símbolo `#`. Los comentarios son ignorados por Python y están ahí para que el programador deje notas y explicaciones.
Ejemplo:
```python
# Este es un comentario que explica el código siguiente
print("Hola, Mundo!")
```
#### Docstrings
Estos son comentarios de varias líneas utilizados para explicar el propósito de una función, método, clase o módulo. Están encerrados en comillas triples (`"""` o `'''`).
Ejemplo:
```python
def saludo(nombre):
    """Esta función saluda a la persona cuyo nombre se pasa como parámetro."""
    print(f"Hola, {nombre}!")
```
Entender estos elementos básicos de la sintaxis y semántica de Python es crucial para escribir código en Python claro y correcto. Establece una base para aprender conceptos más complejos de Python. Recuerda, Python está diseñado para ser legible y sencillo, ¡así que no dudes en experimentar y practicar!

