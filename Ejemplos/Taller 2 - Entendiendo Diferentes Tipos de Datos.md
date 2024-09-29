#  Entendiendo Diferentes Tipos de Datos
En Python, hay varios tipos de datos básicos que son fundamentales para el manejo de información en la programación. Estos incluyen enteros, flotantes, cadenas de texto, y booleanos. Además, aprenderás sobre cómo declarar y utilizar estas variables.

## Enteros, Flotantes, Cadenas, Booleanos

### Ejemplos de Tipos de Datos

```python
# Enteros (int)
numero_de_estrellas = 5

# Flotantes (float)
peso = 72.5

# Cadenas de texto (str)
nombre = "María"

# Booleanos (bool)
esta_abierto = True
```

### Declarando y Utilizando Variables

En estos ejemplos, declaramos diferentes tipos de variables y luego las utilizamos en distintas operaciones o acciones.

```python
# Declarando variables
edad = 30            # Un entero
altura = 1.82        # Un flotante
nombre = "Carlos"    # Una cadena de texto
es_mayor_de_edad = True  # Un booleano

# Utilizando variables
print("Nombre:", nombre)
print("Edad:", edad, "años")
print("Altura:", altura, "metros")
print("¿Es mayor de edad?", es_mayor_de_edad)

# Operaciones con variables
a_nacimiento = 2024 - edad
print("Año de nacimiento:", a_nacimiento)
```

En este ejemplo, utilizamos variables para almacenar información personal como la edad y el nombre, y luego realizamos una operación simple para calcular el año de nacimiento. Los tipos de datos como enteros, flotantes, cadenas de texto y booleanos son fundamentales en cualquier programa en Python y su correcta utilización es clave para el desarrollo eficiente de software.

---

# Taller Práctico en Clase: Tipos de Datos en Python usando Google Colab

## Objetivo del Taller

- **Comprender** y **aplicar** los tipos de datos básicos en Python: enteros, flotantes, cadenas de texto y booleanos.
- **Practicar** la declaración y uso de variables en Python.
- **Familiarizarse** con el uso de **Google Colab** como herramienta de desarrollo.

---

## Preparación

1. **Acceso a Google Colab**

   - Inicia sesión en tu cuenta de Google.
   - Accede a [Google Colab](https://colab.research.google.com/).
   - Crea un **Nuevo Cuaderno** haciendo clic en **"Archivo" > "Nuevo cuaderno"**.
   - Renombra el cuaderno a **"Taller_Tipos_Datos_Python"**.

2. **Organización del Cuaderno**

   - Añade una **portada** con el título del taller y tu nombre.
   - Crea secciones utilizando celdas de texto para organizar las actividades:
     - Actividad 1: Enteros y Flotantes
     - Actividad 2: Cadenas de Texto
     - Actividad 3: Booleanos y Condicionales
     - Actividad 4: Proyecto Integrador

---

## Actividades del Taller

### **Actividad 1: Enteros y Flotantes**

#### **Ejercicio 1: Operaciones Básicas**

- **Objetivo**: Practicar la declaración de variables enteras y flotantes, y realizar operaciones aritméticas básicas.

**Pasos:**

1. Declara dos variables enteras `a` y `b` con valores de tu elección.
2. Declara dos variables flotantes `x` y `y` con valores decimales.
3. Realiza y muestra en pantalla las siguientes operaciones:

   - Suma de `a` y `b`.
   - Resta de `x` menos `y`.
   - Producto de `a` por `x`.
   - División de `b` entre `y`.

**Código de ejemplo:**

```python
# Declaración de variables enteras
a = 10
b = 5

# Declaración de variables flotantes
x = 3.5
y = 2.0

# Operaciones aritméticas
suma = a + b
resta = x - y
producto = a * x
division = b / y

# Mostrar resultados
print("Suma de a y b:", suma)
print("Resta de x y y:", resta)
print("Producto de a y x:", producto)
print("División de b entre y:", division)
```

#### **Ejercicio 2: Cálculo del Área de un Círculo**

- **Objetivo**: Utilizar variables flotantes y la librería `math` para realizar cálculos matemáticos.

**Pasos:**

1. Importa la librería `math`.
2. Solicita al usuario que ingrese el radio de un círculo.
3. Calcula el área del círculo usando la fórmula: \( \text{Área} = \pi \times r^2 \).
4. Muestra el resultado en pantalla con dos decimales.

**Código de ejemplo:**

```python
import math

# Solicitar el radio al usuario
radio = float(input("Ingresa el radio del círculo: "))

# Calcular el área
area = math.pi * radio ** 2

# Mostrar el resultado
print(f"El área del círculo es: {area:.2f}")
```

---

### **Actividad 2: Cadenas de Texto**

#### **Ejercicio 3: Manipulación de Cadenas**

- **Objetivo**: Practicar operaciones básicas con cadenas de texto.

**Pasos:**

1. Declara una variable `nombre` con tu nombre completo.
2. Muestra en pantalla:

   - Tu nombre en **mayúsculas**.
   - Tu nombre en **minúsculas**.
   - La **cantidad de caracteres** que tiene tu nombre.

**Código de ejemplo:**

```python
# Declaración de la cadena
nombre = "María García"

# Operaciones con cadenas
nombre_mayus = nombre.upper()
nombre_minus = nombre.lower()
longitud = len(nombre)

# Mostrar resultados
print("Nombre en mayúsculas:", nombre_mayus)
print("Nombre en minúsculas:", nombre_minus)
print("Cantidad de caracteres:", longitud)
```

#### **Ejercicio 4: Formato de Cadenas**

- **Objetivo**: Utilizar el formato de cadenas para crear mensajes personalizados.

**Pasos:**

1. Solicita al usuario su nombre y edad.
2. Crea un mensaje que diga: "Hola, [nombre]. Tienes [edad] años."
3. Muestra el mensaje en pantalla.

**Código de ejemplo:**

```python
# Solicitar datos al usuario
nombre = input("Ingresa tu nombre: ")
edad = input("Ingresa tu edad: ")

# Crear mensaje personalizado
mensaje = f"Hola, {nombre}. Tienes {edad} años."

# Mostrar el mensaje
print(mensaje)
```

---

### **Actividad 3: Booleanos y Condicionales**

#### **Ejercicio 5: Verificación de Mayoría de Edad**

- **Objetivo**: Utilizar variables booleanas y estructuras condicionales.

**Pasos:**

1. Solicita al usuario su edad.
2. Determina si es mayor de edad (18 años o más).
3. Almacena el resultado en una variable booleana `es_mayor_de_edad`.
4. Muestra un mensaje que indique si el usuario es mayor de edad.

**Código de ejemplo:**

```python
# Solicitar la edad al usuario
edad = int(input("Ingresa tu edad: "))

# Verificar si es mayor de edad
es_mayor_de_edad = edad >= 18

# Mostrar mensaje según la verificación
if es_mayor_de_edad:
    print("Eres mayor de edad.")
else:
    print("Eres menor de edad.")
```

#### **Ejercicio 6: Número Par o Impar**

- **Objetivo**: Aplicar operadores lógicos y condicionales con variables enteras.

**Pasos:**

1. Solicita al usuario que ingrese un número entero.
2. Determina si el número es par o impar.
3. Muestra el resultado en pantalla.

**Código de ejemplo:**

```python
# Solicitar un número entero
numero = int(input("Ingresa un número entero: "))

# Determinar si es par o impar
es_par = numero % 2 == 0

# Mostrar el resultado
if es_par:
    print(f"El número {numero} es par.")
else:
    print(f"El número {numero} es impar.")
```

---

### **Actividad 4: Proyecto Integrador**

#### **Ejercicio 7: Calculadora de Índice de Masa Corporal (IMC)**

- **Objetivo**: Integrar los conceptos aprendidos para crear un programa útil.

**Pasos:**

1. Solicita al usuario su peso en kilogramos y su altura en metros.
2. Calcula el Índice de Masa Corporal usando la fórmula: \( \text{IMC} = \frac{\text{peso}}{\text{altura}^2} \).
3. Muestra el IMC con dos decimales.
4. Utiliza condicionales para interpretar el resultado según las categorías:

   - **Bajo peso**: IMC menor a 18.5
   - **Peso normal**: IMC entre 18.5 y 24.9
   - **Sobrepeso**: IMC entre 25 y 29.9
   - **Obesidad**: IMC de 30 o más

5. Muestra al usuario en qué categoría se encuentra.

**Código de ejemplo:**

```python
# Solicitar peso y altura al usuario
peso = float(input("Ingresa tu peso en kg: "))
altura = float(input("Ingresa tu altura en metros: "))

# Calcular el IMC
imc = peso / (altura ** 2)

# Mostrar el IMC
print(f"Tu IMC es: {imc:.2f}")

# Interpretar el resultado
if imc < 18.5:
    categoria = "Bajo peso"
elif 18.5 <= imc <= 24.9:
    categoria = "Peso normal"
elif 25 <= imc <= 29.9:
    categoria = "Sobrepeso"
else:
    categoria = "Obesidad"

# Mostrar la categoría
print("Categoría:", categoria)
```

---

## Cierre del Taller

### **Repaso de Conceptos**

- **Enteros y Flotantes**: Tipos numéricos para representar valores sin y con decimales.
- **Cadenas de Texto**: Manipulación y formato de secuencias de caracteres.
- **Booleanos**: Valores lógicos para control de flujo en programas.
- **Variables y Operaciones**: Declaración y uso efectivo en diferentes contextos.

### **Discusión en Grupo**

- **¿Qué aprendimos hoy?**
- **¿Qué ejercicios fueron más desafiantes y por qué?**
- **¿Cómo aplicaremos estos conceptos en futuros programas?**

---

## Recursos Adicionales

- **Documentación Oficial de Python**: [docs.python.org/es/3/](https://docs.python.org/es/3/)
- **Tutoriales en Línea**:
  - [W3Schools Python Tutorial](https://www.w3schools.com/python/)
  - [Programación en Python](https://aprendeconalf.es/docencia/python/)

---

## Actividad Opcional

#### **Ejercicio 8: Generador de Contraseñas Simples**

- **Objetivo**: Aplicar los conocimientos para crear una herramienta práctica.

**Pasos:**

1. Importa el módulo `random`.
2. Crea listas con caracteres posibles:

   - Letras minúsculas (`a`-`z`)
   - Letras mayúsculas (`A`-`Z`)
   - Dígitos (`0`-`9`)

3. Solicita al usuario la longitud deseada de la contraseña.
4. Genera una contraseña aleatoria combinando caracteres de las listas.
5. Muestra la contraseña generada.

**Código de ejemplo:**

```python
import random
import string

# Crear listas de caracteres
letras_minusculas = list(string.ascii_lowercase)
letras_mayusculas = list(string.ascii_uppercase)
digitos = list(string.digits)

# Combinar todas las listas
caracteres = letras_minusculas + letras_mayusculas + digitos

# Solicitar la longitud de la contraseña
longitud = int(input("Ingresa la longitud deseada para la contraseña: "))

# Generar la contraseña
contraseña = ''.join(random.choice(caracteres) for _ in range(longitud))

# Mostrar la contraseña generada
print("Contraseña generada:", contraseña)
```

---
---

# Taller en Casa: Tipos de Datos en Python

## Objetivo del Taller

- **Reforzar** los conceptos de tipos de datos básicos en Python aprendidos en clase.
- **Practicar** la declaración y uso de variables de diferentes tipos.
- **Desarrollar** habilidades de resolución de problemas mediante ejercicios prácticos.

---

## Instrucciones Generales

1. **Fecha de entrega**: [Especificar fecha límite].
2. **Formato de entrega**: Un cuaderno de **Google Colab** con las respuestas a los ejercicios.
3. **Recomendación**: Lee cuidadosamente cada ejercicio y asegúrate de comprender lo que se solicita antes de comenzar a programar.
4. **Recursos permitidos**: Apuntes de clase, documentación oficial de Python y recursos en línea confiables.

---

## Actividades del Taller

### **Ejercicio 1: Información Personal**

Crea un programa que:

- Solicite al usuario la siguiente información:
  - **Nombre completo** (cadena de texto).
  - **Edad** (entero).
  - **Estatura** en metros (flotante).
  - **¿Estás estudiando actualmente?** (responder con **Sí** o **No**).

- Muestra en pantalla un resumen de la información ingresada, siguiendo este formato:

  ```
  --- Información Personal ---
  Nombre: [Nombre]
  Edad: [Edad] años
  Estatura: [Estatura] metros
  Estudiando actualmente: [Sí/No]
  ```

**Pistas:**

- Para convertir la respuesta de **Sí** o **No** a un valor booleano, puedes usar condiciones.
- Asegúrate de manejar correctamente los tipos de datos al solicitar y mostrar la información.

---

### **Ejercicio 2: Calculadora de Tiempo**

Escribe un programa que:

- Solicite al usuario un número entero de **días**.
- Calcule y muestre:

  - El número de **semanas** completas en esos días.
  - El número de **horas**, **minutos** y **segundos** totales.

**Ejemplo de ejecución:**

```
Ingresa el número de días: 3
Equivalente en semanas: 0 semanas
Total de horas: 72 horas
Total de minutos: 4320 minutos
Total de segundos: 259200 segundos
```

**Pistas:**

- 1 semana = 7 días
- 1 día = 24 horas
- 1 hora = 60 minutos
- 1 minuto = 60 segundos

---

### **Ejercicio 3: Conversión de Temperaturas**

Escribe un programa que:

- Solicite al usuario una temperatura en grados **Celsius** (float).
- Convierta y muestre la temperatura en grados **Fahrenheit** y **Kelvin**.

**Fórmulas de conversión:**

- Fahrenheit = (Celsius × 9/5) + 32
- Kelvin = Celsius + 273.15

**Ejemplo de ejecución:**

```
Ingresa la temperatura en grados Celsius: 25
Equivalente en Fahrenheit: 77.0 °F
Equivalente en Kelvin: 298.15 K
```

---

### **Ejercicio 4: Año Bisiesto**

Crea un programa que:

- Solicite al usuario un **año** (entero).
- Determine si el año es **bisiesto** o no.
- Muestra el resultado en pantalla.

**Reglas para determinar si un año es bisiesto:**

- Un año es bisiesto si es divisible por 4.
- Pero no es bisiesto si es divisible por 100, a menos que también sea divisible por 400.

**Ejemplo de ejecución:**

```
Ingresa un año: 2020
El año 2020 es bisiesto.

Ingresa un año: 1900
El año 1900 no es bisiesto.
```

**Pistas:**

- Utiliza operadores lógicos (`and`, `or`, `not`) para combinar condiciones.

---

## Recursos de Apoyo

- **Documentación Oficial de Python**: [docs.python.org/es/3/](https://docs.python.org/es/3/)
- **Tutoriales en Línea**:
  - [Python desde cero](https://www.python.org/about/gettingstarted/)
  - [Programación en Python](https://aprendeconalf.es/docencia/python/)

- **Videos Educativos**:
  - [Curso de Python para Principiantes](https://www.youtube.com/watch?v=numQzIgpOo0&ab_channel=BitBoss)

---
