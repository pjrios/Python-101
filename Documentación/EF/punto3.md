# Operadores

### Operadores Aritméticos
1. **Operadores Aritméticos**
   - Estos operadores se utilizan para realizar operaciones aritméticas como suma, resta, multiplicación, etc.
   - Ejemplos:
     - `+` Suma: `5 + 3` da `8`
     - `-` Resta: `5 - 3` da `2`
     - `*` Multiplicación: `5 * 3` da `15`
     - `/` División (flotante): `5 / 2` da `2.5`
     - `//` División (entera): `5 // 2` da `2` (sin decimales)
     - `%` Módulo: `5 % 2` da `1` (resto de la división)
     - `**` Exponenciación: `5 ** 2` da `25` (5 al cuadrado)

### Operadores de Comparación
2. **Operadores de Comparación**
   - Estos operadores se utilizan para comparar valores. El resultado de una comparación es un Booleano (Verdadero o Falso).
   - Ejemplos:
     - `==` Igual a: `5 == 3` es `Falso`
     - `!=` No igual a: `5 != 3` es `Verdadero`
     - `>` Mayor que: `5 > 3` es `Verdadero`
     - `<` Menor que: `5 < 3` es `Falso`
     - `>=` Mayor o igual a: `5 >= 5` es `Verdadero`
     - `<=` Menor o igual a: `5 <= 3` es `Falso`

### Operadores Lógicos
3. **Operadores Lógicos**
   - Los operadores lógicos se utilizan para combinar declaraciones condicionales.
   - Ejemplos:
     - `and` Devuelve Verdadero si ambas declaraciones son verdaderas: `5 > 3 and 5 < 10` es `Verdadero`
     - `or` Devuelve Verdadero si una de las declaraciones es verdadera: `5 > 3 or 5 > 10` es `Verdadero`
     - `not` Invierte el resultado, devuelve Falso si el resultado es verdadero: `not(5 > 3)` es `Falso`

### Operadores de Asignación
4. **Operadores de Asignación**
   - Se utilizan para asignar valores a variables.
   - Ejemplos:
     - `=` Asignación simple: `x = 5`
     - `+=` Sumar y asignar: `x += 3` (equivalente a `x = x + 3`)
     - `-=` Restar y asignar: `x -= 3` (equivalente a `x = x - 3`)
     - `*=` Multiplicar y asignar: `x *= 3` (equivalente a `x = x * 3`)
     - `/=` Dividir y asignar: `x /= 3` (equivalente a `x = x / 3`)
     - `%=` Módulo y asignar: `x %= 3` (equivalente a `x = x % 3`)
     - `**=` Exponente y asignar: `x **= 3` (equivalente a `x = x ** 3`)
     - `//=` División entera y asignar: `x //= 3` (equivalente a `x = x // 3`)

Entender estos operadores es crucial para realizar cálculos y operaciones lógicas en Python. Son bloques de construcción fundamentales en la programación de Python, que te permiten manipular datos y crear lógica compleja en tu código. ¡Pueden experimentar con estos operadores para ver cómo funcionan e interactúan con diferentes tipos de datos!


## Ejemplos

## Operadores Aritméticos

### Ejemplos:

```python
# Suma
suma = 10 + 5

# Resta
resta = 10 - 5

# Multiplicación
multiplicacion = 10 * 5

# División
division = 10 / 5

# Módulo (resto de la división)
modulo = 10 % 5

# Exponenciación
exponenciacion = 10 ** 5

# División Entera
division_entera = 10 // 5

print("Suma:", suma)
print("Resta:", resta)
print("Multiplicación:", multiplicacion)
print("División:", division)
print("Módulo:", modulo)
print("Exponenciación:", exponenciacion)
print("División Entera:", division_entera)
```

## Operadores de Comparación

### Ejemplos:

```python
# Igual a
igual = (10 == 5)

# Diferente de
diferente = (10 != 5)

# Mayor que
mayor_que = (10 > 5)

# Menor que
menor_que = (10 < 5)

# Mayor o igual que
mayor_o_igual = (10 >= 5)

# Menor o igual que
menor_o_igual = (10 <= 5)

print("Igual:", igual)
print("Diferente:", diferente)
print("Mayor que:", mayor_que)
print("Menor que:", menor_que)
print("Mayor o igual que:", mayor_o_igual)
print("Menor o igual que:", menor_o_igual)
```

## Operadores Lógicos

### Ejemplos:

```python
verdadero = True
falso = False

# Operador and
and_logico = verdadero and falso

# Operador or
or_logico = verdadero or falso

# Operador not
not_logico = not verdadero

print("AND lógico:", and_logico)
print("OR lógico:", or_logico)
print("NOT lógico:", not_logico)
```

## Operadores de Asignación


### Ejemplos:

```python
# Asignación simple
numero = 10

# Suma y asignación
numero += 5

# Resta y asignación
numero -= 5

# Multiplicación y asignación
numero *= 5

# División y asignación
numero /= 5

print("Número final:", numero)
```

Estos ejemplos demuestran el uso de operadores en Python para realizar tareas comunes en programación. Los operadores son fundamentales para la lógica de cualquier programa y entender su funcionamiento es clave para la resolución de problemas y la automatización de tareas.
