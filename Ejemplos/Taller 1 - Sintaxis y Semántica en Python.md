# Sintaxis y Semántica en Python - Ejemplos
Archivo de google colab para referencia: https://colab.research.google.com/drive/1dTiH-c1MMhPcTnCg0lHDX6BA2A3Oy4cJ?usp=sharing
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

---

# Taller Práctico: Sintaxis y Semántica en Python usando Google Colab

## Objetivo del Taller

- **Comprender** y **aplicar** los conceptos básicos de sintaxis y semántica en Python.
- **Practicar** la escritura de código Python correcto y legible.
- **Familiarizarse** con el uso de **Google Colab** como herramienta de desarrollo.

---

## Preparación

1. **Acceder a Google Colab**

   - Inicia sesión en tu cuenta de Google.
   - Accede a [Google Colab](https://colab.research.google.com/).
   - Crea un **Nuevo Cuaderno** haciendo clic en **"Archivo" > "Nuevo cuaderno"**.

2. **Configuración Inicial**

   - Renombra el cuaderno a **"Taller_Sintaxis_Python"**.
   - Familiarízate con la interfaz de Google Colab:
     - Celdas de código y texto.
     - Cómo ejecutar celdas (botón de "Play" o `Shift + Enter`).

---

## Actividades del Taller

### **Actividad 1: Explorando la Sintaxis Básica**

#### **Ejercicio 1: Imprimir Mensajes**

- Escribe un programa que imprima **"¡Hola, mundo!"** en la consola.

  ```python
  print("¡Hola, mundo!")
  ```

- **Desafío Adicional**: Imprime tu nombre y tu lenguaje de programación favorito.

  ```python
  print("Mi nombre es Ana y mi lenguaje favorito es Python.")
  ```

#### **Ejercicio 2: Variables y Tipos de Datos**

- Declara las siguientes variables:

  - `nombre` (cadena de texto)
  - `edad` (entero)
  - `altura` (flotante)

  ```python
  nombre = "Ana"
  edad = 25
  altura = 1.68

  print("Nombre:", nombre)
  print("Edad:", edad)
  print("Altura:", altura)
  ```

---

### **Actividad 2: Entendiendo la Indentación**

#### **Ejercicio 3: Condicionales Simples**

- Escribe un programa que determine si un número es **par** o **impar**.

  ```python
  numero = int(input("Ingresa un número: "))

  if numero % 2 == 0:
      print("El número es par.")
  else:
      print("El número es impar.")
  ```

- **Discusión**: Analiza cómo la indentación afecta la estructura del código.

#### **Ejercicio 4: Bucles y Estructuras de Control**

- Crea un bucle que imprima los números del 1 al 5.

  ```python
  for i in range(1, 6):
      print("Número:", i)
  ```

---

### **Actividad 3: Comentarios y Docstrings**

#### **Ejercicio 5: Añadiendo Comentarios**

- Añade comentarios al siguiente código para explicar qué hace:

  ```python
  # Función que calcula el cuadrado de un número
  def cuadrado(n):
      """Calcula el cuadrado de n."""
      resultado = n ** 2
      return resultado

  numero = 4
  print("El cuadrado de", numero, "es", cuadrado(numero))
  ```

#### **Ejercicio 6: Documentación de Funciones**

- Escribe una función que convierta grados Celsius a Fahrenheit y añade un docstring descriptivo.

  ```python
  def celsius_a_fahrenheit(celsius):
      """
      Convierte una temperatura de grados Celsius a Fahrenheit.

      Parámetros:
      celsius (float): Temperatura en grados Celsius.

      Retorna:
      float: Temperatura en grados Fahrenheit.
      """
      return celsius * 9/5 + 32

  temperatura_c = 25
  temperatura_f = celsius_a_fahrenheit(temperatura_c)
  print(f"{temperatura_c}°C son {temperatura_f}°F")
  ```

---

### **Actividad 4: Práctica Integrada**

#### **Ejercicio 7: Calculadora Simple**

- Crea un programa que solicite dos números al usuario y realice las cuatro operaciones básicas.

  ```python
  numero1 = float(input("Ingresa el primer número: "))
  numero2 = float(input("Ingresa el segundo número: "))

  suma = numero1 + numero2
  resta = numero1 - numero2
  multiplicacion = numero1 * numero2
  division = numero1 / numero2

  print("Suma:", suma)
  print("Resta:", resta)
  print("Multiplicación:", multiplicacion)
  print("División:", division)
  ```

- **Desafío Adicional**: Añade manejo de errores para evitar división por cero.

  ```python
  if numero2 != 0:
      division = numero1 / numero2
      print("División:", division)
  else:
      print("Error: No se puede dividir entre cero.")
  ```

#### **Ejercicio 8: Juego de Adivinanza**

- Escribe un programa donde la computadora genera un número aleatorio entre 1 y 10, y el usuario debe adivinarlo.

  ```python
  import random

  numero_secreto = random.randint(1, 10)
  intento = int(input("Adivina el número (entre 1 y 10): "))

  if intento == numero_secreto:
      print("¡Felicidades! Adivinaste el número.")
  else:
      print("Lo siento, el número era:", numero_secreto)
  ```

---

### **Actividad 5: Profundizando en la Sintaxis y Semántica**

#### **Ejercicio 9: Listas y Bucles**

- Crea una lista con los nombres de tus tres películas favoritas y muestra cada una en pantalla.

  ```python
  peliculas = ["Inception", "Matrix", "Interstellar"]

  for pelicula in peliculas:
      print("Película:", pelicula)
  ```

#### **Ejercicio 10: Diccionarios y Funciones**

- Define un diccionario que contenga información sobre una persona (nombre, edad, ciudad) y una función que imprima esta información.

  ```python
  persona = {
      "nombre": "Carlos",
      "edad": 30,
      "ciudad": "Madrid"
  }

  def mostrar_informacion(persona):
      """
      Imprime la información de una persona.
      """
      print("Nombre:", persona["nombre"])
      print("Edad:", persona["edad"])
      print("Ciudad:", persona["ciudad"])

  mostrar_informacion(persona)
  ```

---

## Cierre del Taller

### **Repaso de Conceptos**

- **Sintaxis básica**: Uso correcto de estructuras y palabras clave.
- **Indentación**: Importancia en la estructura y ejecución del código.
- **Comentarios y Docstrings**: Mejora de la legibilidad y documentación.
- **Variables y Tipos de Datos**: Declaración y manipulación efectiva.

### **Discusión en Grupo**

- **Desafíos encontrados**: ¿Qué ejercicios fueron más complicados y por qué?
- **Aprendizajes clave**: ¿Qué conceptos nuevos aprendieron hoy?

---

## Recursos Adicionales

- **Documentación Oficial de Python**: [docs.python.org/es/3/](https://docs.python.org/es/3/)
- **Tutoriales Interactivos**: [W3Schools Python Tutorial](https://www.w3schools.com/python/)
- **Comunidades en Línea**: [Foro de Python en Español](https://foro.elhacker.net/programacion_general/python_b173.0/)

---

## Actividad Opcional

### **Proyecto Mini-Calculadora**

- **Descripción**: Crear una calculadora que permita al usuario seleccionar la operación a realizar (suma, resta, multiplicación, división) y que maneje posibles errores de entrada.

  ```python
  def calculadora():
      """
      Calculadora básica que realiza operaciones aritméticas.
      """
      print("Seleccione la operación.")
      print("1. Sumar")
      print("2. Restar")
      print("3. Multiplicar")
      print("4. Dividir")

      eleccion = input("Ingrese la opción (1/2/3/4): ")

      numero1 = float(input("Ingresa el primer número: "))
      numero2 = float(input("Ingresa el segundo número: "))

      if eleccion == '1':
          resultado = numero1 + numero2
          print("Resultado:", resultado)
      elif eleccion == '2':
          resultado = numero1 - numero2
          print("Resultado:", resultado)
      elif eleccion == '3':
          resultado = numero1 * numero2
          print("Resultado:", resultado)
      elif eleccion == '4':
          if numero2 != 0:
              resultado = numero1 / numero2
              print("Resultado:", resultado)
          else:
              print("Error: División por cero.")
      else:
          print("Opción inválida.")

  calculadora()
  ```

---

# Taller en Casa: Sintaxis y Semántica en Python

## Objetivo del Taller

- **Reforzar** los conceptos de sintaxis y semántica en Python aprendidos en clase.
- **Practicar** de forma autónoma la escritura y ejecución de código Python.
- **Desarrollar** habilidades de resolución de problemas mediante ejercicios prácticos.

---

## Actividades del Taller

### **Actividad 1: Sintaxis Básica y Operaciones Simples**

#### **Ejercicio 1: Calculadora de Propinas**

Crea un programa que calcule la propina a dejar en un restaurante. El programa debe:

- Solicitar al usuario el **monto total de la cuenta**.
- Solicitar el **porcentaje de propina** que desea dejar (por ejemplo, 10, 15, 20).
- Calcular y mostrar en pantalla:
  - El **monto de la propina**.
  - El **monto total a pagar** (cuenta + propina).

**Pista**: Asegúrate de manejar los tipos de datos correctamente (números decimales).

**Ejemplo de ejecución:**

```
Ingrese el monto total de la cuenta: 50
Ingrese el porcentaje de propina que desea dejar: 15
La propina es: 7.5
El total a pagar es: 57.5
```

---

#### **Ejercicio 2: Conversor de Unidades**

Escribe un programa que convierta una cantidad dada en **metros** a sus equivalentes en:

- **Centímetros**
- **Pulgadas**
- **Pies**

El programa debe:

- Solicitar al usuario la cantidad en metros.
- Realizar las conversiones y mostrar los resultados.

**Factores de conversión:**

- 1 metro = 100 centímetros
- 1 metro = 39.37 pulgadas
- 1 metro = 3.281 pies

**Ejemplo de ejecución:**

```
Ingrese la cantidad en metros: 2
Equivalente en centímetros: 200 cm
Equivalente en pulgadas: 78.74 in
Equivalente en pies: 6.562 ft
```

---

### **Actividad 2: Indentación y Estructuras de Control**

#### **Ejercicio 3: Clasificación de Edad**

Crea un programa que:

- Solicite al usuario su **edad**.
- Determine y muestre en pantalla si es un **niño** (0-12 años), **adolescente** (13-17 años), **adulto** (18-64 años) o **adulto mayor** (65 años en adelante).

**Ejemplo de ejecución:**

```
Ingrese su edad: 30
Eres un adulto.
```

---

#### **Ejercicio 4: Número Mayor**

Escribe un programa que:

- Solicite al usuario **tres números enteros**.
- Determine cuál es el **mayor** de los tres.
- Muestre el resultado en pantalla.

**Ejemplo de ejecución:**

```
Ingrese el primer número: 12
Ingrese el segundo número: 7
Ingrese el tercer número: 20
El número mayor es: 20
```

---

## Consejos para el Éxito

- **Planificación**: Lee todos los ejercicios antes de comenzar y planifica tu tiempo.
- **Práctica**: No te limites a los ejemplos dados; experimenta y prueba diferentes casos.
- **Preguntas**: Si tienes dudas, anótalas y consúltalas en la próxima clase o investiga en los recursos de apoyo.
- **Calidad del Código**: Escribe código limpio y legible. Usa nombres de variables descriptivos y comentarios cuando sea útil.


---

**Respuestas del Taller en Casa: Sintaxis y Semántica en Python**

---

### **Actividad 1: Sintaxis Básica y Operaciones Simples**

#### **Ejercicio 1: Calculadora de Propinas**

**Descripción:**

Crea un programa que calcule la propina a dejar en un restaurante. El programa debe:

- Solicitar al usuario el monto total de la cuenta.
- Solicitar el porcentaje de propina que desea dejar (por ejemplo, 10, 15, 20).
- Calcular y mostrar en pantalla:
  - El monto de la propina.
  - El monto total a pagar (cuenta + propina).

**Código:**

```python
# Calculadora de Propinas

# Solicitar al usuario el monto total de la cuenta y convertirlo a float
monto_cuenta = float(input("Ingrese el monto total de la cuenta: "))

# Solicitar el porcentaje de propina y convertirlo a float
porcentaje_propina = float(input("Ingrese el porcentaje de propina que desea dejar: "))

# Calcular el monto de la propina
monto_propina = monto_cuenta * (porcentaje_propina / 100)

# Calcular el monto total a pagar (cuenta + propina)
total_pagar = monto_cuenta + monto_propina

# Mostrar el monto de la propina, redondeado a dos decimales
print("La propina es:", round(monto_propina, 2))

# Mostrar el monto total a pagar, redondeado a dos decimales
print("El total a pagar es:", round(total_pagar, 2))
```

**Notas:**

- Se utiliza `float()` para manejar números decimales en caso de que el monto de la cuenta o el porcentaje de propina incluyan decimales.
- La función `round()` se utiliza para redondear los montos a dos decimales, como es común en cantidades monetarias.

---

#### **Ejercicio 2: Conversor de Unidades**

**Descripción:**

Escribe un programa que convierta una cantidad dada en metros a sus equivalentes en:

- **Centímetros**
- **Pulgadas**
- **Pies**

**Código:**

```python
# Conversor de Unidades

# Solicitar al usuario la cantidad en metros y convertirla a float
metros = float(input("Ingrese la cantidad en metros: "))

# Factores de conversión
METROS_A_CENTIMETROS = 100          # 1 metro = 100 centímetros
METROS_A_PULGADAS = 39.37           # 1 metro = 39.37 pulgadas
METROS_A_PIES = 3.281               # 1 metro = 3.281 pies

# Realizar las conversiones
centimetros = metros * METROS_A_CENTIMETROS
pulgadas = metros * METROS_A_PULGADAS
pies = metros * METROS_A_PIES

# Mostrar los resultados, redondeados según sea necesario
print("Equivalente en centímetros:", round(centimetros, 2), "cm")
print("Equivalente en pulgadas:", round(pulgadas, 2), "in")
print("Equivalente en pies:", round(pies, 3), "ft")
```

**Notas:**

- Los factores de conversión se definen como constantes para mayor claridad.
- Se utiliza `round()` para redondear los resultados:
  - Centímetros y pulgadas a dos decimales.
  - Pies a tres decimales, según el ejemplo proporcionado.

---

### **Actividad 2: Indentación y Estructuras de Control**

#### **Ejercicio 3: Clasificación de Edad**

**Descripción:**

Crea un programa que:

- Solicite al usuario su edad.
- Determine y muestre en pantalla si es un **niño** (0-12 años), **adolescente** (13-17 años), **adulto** (18-64 años) o **adulto mayor** (65 años en adelante).

**Código:**

```python
# Clasificación de Edad

# Solicitar al usuario su edad y convertirla a entero
edad = int(input("Ingrese su edad: "))

# Determinar la clasificación según la edad
if 0 <= edad <= 12:
    print("Eres un niño.")
elif 13 <= edad <= 17:
    print("Eres un adolescente.")
elif 18 <= edad <= 64:
    print("Eres un adulto.")
elif edad >= 65:
    print("Eres un adulto mayor.")
else:
    print("Edad inválida. Por favor, ingresa una edad válida.")
```

**Notas:**

- Se utilizan operadores de comparación para verificar si la edad está dentro de los rangos especificados.
- Se incluye una condición `else` para manejar edades inválidas (por ejemplo, números negativos).

---

#### **Ejercicio 4: Número Mayor**

**Descripción:**

Escribe un programa que:

- Solicite al usuario tres números enteros.
- Determine cuál es el mayor de los tres.
- Muestre el resultado en pantalla.

**Código:**

```python
# Determinar el Número Mayor

# Solicitar al usuario tres números enteros
num1 = int(input("Ingrese el primer número: "))
num2 = int(input("Ingrese el segundo número: "))
num3 = int(input("Ingrese el tercer número: "))

# Asumir inicialmente que el primer número es el mayor
mayor = num1

# Comparar con el segundo número
if num2 > mayor:
    mayor = num2

# Comparar con el tercer número
if num3 > mayor:
    mayor = num3

# Mostrar el número mayor
print("El número mayor es:", mayor)
```

**Notas:**

- Se inicia asumiendo que `num1` es el mayor y luego se compara con `num2` y `num3`.
- Se actualiza la variable `mayor` si se encuentra un número mayor.
- Este método es eficiente y fácil de entender para los estudiantes.

---
