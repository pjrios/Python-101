## Declaraciones Condicionales (if, else, elif)

Las declaraciones condicionales permiten ejecutar diferentes bloques de código dependiendo de ciertas condiciones.

### Ejemplos:

```python
edad = 20

# Declaración if
if edad >= 18:
    print("Es mayor de edad.")

# Declaración if-else
if edad < 18:
    print("Es menor de edad.")
else:
    print("Es mayor de edad.")

# Declaración if-elif-else
if edad < 13:
    print("Es un niño.")
elif edad < 18:
    print("Es un adolescente.")
else:
    print("Es un adulto.")
```

## Bucles (for, while)

Los bucles permiten repetir un bloque de código múltiples veces.

### Ejemplos:

#### Bucle For

```python
# Iterando sobre una lista
nombres = ["Ana", "Bruno", "Carlos"]
for nombre in nombres:
    print(nombre)

# Utilizando range()
for i in range(5):
    print(i)
```

#### Bucle While

```python
# Ejecutando mientras se cumpla una condición
contador = 0
while contador < 5:
    print(contador)
    contador += 1
```

## Declaraciones de break y continue

`break` y `continue` son utilizadas para modificar el comportamiento de los bucles.

### Ejemplos:

```python
# Uso de break
for i in range(10):
    if i == 5:
        break
    print(i)

# Uso de continue
for i in range(10):
    if i % 2 == 0:
        continue
    print(i)
```

Estos ejemplos muestran cómo las estructuras de control, como las declaraciones condicionales y los bucles, son utilizadas en Python para controlar el flujo de un programa. Comprender y utilizar estas estructuras es fundamental para escribir programas eficientes y efectivos.
