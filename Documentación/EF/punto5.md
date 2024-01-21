
# Funciones
Las funciones son bloques de código que se pueden llamar y ejecutar en cualquier momento. Son fundamentales para la reutilización de código y la organización en Python.

### Definiendo y Llamando Funciones
1. **Definición y Llamada de Funciones**
   - **Función:** Un bloque de código que solo se ejecuta cuando se llama. Las funciones pueden recibir datos (parámetros) y devolver datos como resultado.
   - **Definir una Función:** Usa la palabra clave `def`, seguida del nombre de la función y paréntesis `()`.
     - Ejemplo:
       ```python
       def saludo():
           print("¡Hola, Mundo!")
       ```
   - **Llamando a una Función:** Para ejecutar una función, llámala por su nombre seguido de paréntesis.
     - Ejemplo:
       ```python
       saludo()  # Esto mostrará: ¡Hola, Mundo!
       ```

### Declaraciones de Retorno
2. **Declaraciones de Retorno**
   - **Propósito:** Una declaración de retorno finaliza la ejecución de la función y "devuelve" el resultado al llamador.
   - **Ejemplo:**
     ```python
     def sumar(x, y):
         return x + y

     resultado = sumar(5, 3)
     print(resultado)  # Muestra: 8
     ```

### Parámetros y Argumentos
3. **Parámetros y Argumentos**
   - **Parámetros:** Variables enumeradas dentro de los paréntesis en la definición de la función. Son marcadores de posición para los valores que la función necesita para trabajar.
   - **Argumentos:** Valores reales pasados a la función cuando se llama.
   - **Ejemplo:**
     ```python
     def multiplicar(a, b):
         return a * b

     resultado = multiplicar(4, 5)  # 4 y 5 son argumentos
     print(resultado)  # Muestra: 20
     ```
   - **Nota:** Los parámetros son los nombres especificados en la definición de la función, mientras que los argumentos son los valores reales que pasas a la función.

### Alcance de las Variables
4. **Alcance de las Variables**
   - **Alcance Local:** Las variables creadas dentro de una función están en el alcance local de esa función. Solo se pueden usar dentro de esa función.
   - **Alcance Global:** Las variables creadas en el cuerpo principal del script de Python están en el alcance global y pueden ser utilizadas por cualquier parte del programa.
   - **Ejemplo:**
     ```python
     def miFuncion():
         var_local = "Soy local"
         print(var_local)  # Esto es válido

     miFuncion()
     print(var_local)  # Esto generará un error, ya que var_local no es accesible fuera de miFuncion
     ```
   - **Nota:** Una variable en el alcance local no se puede acceder desde fuera de su función, pero una variable global se puede acceder desde cualquier parte del código.

Entender las funciones en Python es clave para escribir código reutilizable y organizado. Las funciones te permiten encapsular la lógica del código y ejecutarla múltiples veces, potencialmente con diferentes argumentos, haciendo tu código más modular y eficiente. Practicar con diferentes tipos de funciones y parámetros ayudará a solidificar tu comprensión de este concepto.

# Ejemplos

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
