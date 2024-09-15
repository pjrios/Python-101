## Definiendo y Llamando a Funciones
Una función se define con la palabra clave `def` y se llama por su nombre seguido de paréntesis.

### Ejemplos:
```python
# Definiendo una función
def saludar():
    print("Hola, mundo!")

# Llamando a la función
saludar()
```

## Declaraciones de Retorno
Las funciones pueden devolver valores usando la palabra clave `return`.

### Ejemplos:
```python
# Función que retorna la suma de dos números
def sumar(a, b):
    return a + b

resultado = sumar(5, 3)
print("La suma es:", resultado)
```

## Parámetros y Argumentos
Los parámetros son variables que se definen en la función, y los argumentos son los valores pasados a la función.

### Ejemplos:
```python
# Función con parámetros
def presentarse(nombre, edad):
    print(f"Mi nombre es {nombre} y tengo {edad} años.")

# Llamando a la función con argumentos
presentarse("Ana", 25)
```

## Alcance de las Variables
El alcance de una variable determina dónde está disponible y accesible.
### Ejemplos:
```python
# Variable global
variable_global = "Global"

def demostrar_alcance():
    # Variable local
    variable_local = "Local"
    print(variable_local)
    print(variable_global)

demostrar_alcance()
print(variable_global)
# print(variable_local) - Esto generaría un error ya que variable_local es local a la función
```

Estos ejemplos muestran cómo definir, llamar y trabajar con funciones en Python. Las funciones son herramientas esenciales en la programación que permiten escribir código más limpio, modular y reutilizable.
