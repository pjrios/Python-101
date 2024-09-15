### 1. Entendiendo la Indentación

Python utiliza la indentación para definir bloques de código.

**Ejemplo Correcto:**

```python
def saludar(nombre):
    mensaje = "Hola, " + nombre
    print(mensaje)

saludar("Ana")
```

**Ejemplo Incorrecto (Error de Indentación):**

```python
def saludar(nombre):
mensaje = "Hola, " + nombre  # Esta línea debería estar indentada
print(mensaje)

saludar("Ana")
```

### 2. Comentarios y Cadenas de Documentación (Docstrings)

Los comentarios se utilizan para explicar el código y no se ejecutan, mientras que los docstrings documentan funciones, clases, etc.

**Ejemplo:**

```python
# Esto es un comentario
def suma(a, b):
    """
    Esta función suma dos números.
    Argumentos:
    a (int): Primer número
    b (int): Segundo número

    Retorna:
    int: La suma de a y b
    """
    return a + b

# Llamando a la función
resultado = suma(5, 3)
print(resultado)  # Imprime 8
```

### 3. Variables y Tipos de Datos

Las variables en Python se utilizan para almacenar datos de diferentes tipos.

**Ejemplo:**

```python
# Ejemplo con Números
edad = 25  # Entero (int)
altura = 1.75  # Flotante (float)

# Cadenas de texto
nombre = "Carlos"  # String (str)

# Booleanos
es_estudiante = True  # Boolean (bool)

# Imprimir variables
print("Nombre:", nombre)
print("Edad:", edad, "años")
print("Altura:", altura, "metros")
print("Estudiante:", es_estudiante)
```

### Practice
1. a
2. b
3. c
