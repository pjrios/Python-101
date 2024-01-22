# Estructuras de Datos
Python ofrece varias estructuras de datos integradas que son fundamentales para almacenar y organizar datos. Estas incluyen listas, tuplas, conjuntos y diccionarios.

### Listas
1. **Listas**
   - **Descripción:** Las listas son colecciones ordenadas y mutables (cambiables) de elementos. Pueden contener elementos de diferentes tipos.
   - **Creación:** Usa corchetes `[]` para crear una lista.
     - Ejemplo: `mi_lista = [1, 2, 3, "Python", 4.5]`
   - **Acceso a Elementos:** Usa el índice (comienza en 0) para acceder a los elementos. 
     - Ejemplo: `mi_lista[0]` da `1`.
   - **Modificación de Listas:** Puedes añadir, eliminar o cambiar elementos.
     - Ejemplo: `mi_lista.append("nuevo elemento")` añade un elemento al final.

### Tuplas
2. **Tuplas**
   - **Descripción:** Las tuplas son colecciones ordenadas e inmutables. Una vez creada una tupla, no puedes cambiar su contenido.
   - **Creación:** Usa paréntesis `()` para crear una tupla.
     - Ejemplo: `mi_tupla = (1, 2, 3, "Python")`
   - **Acceso a Elementos:** Similar a las listas, usa el índice.
     - Ejemplo: `mi_tupla[1]` da `2`.
   - **Inmutabilidad:** No puedes cambiar una tupla después de haberla creado.

### Conjuntos
3. **Conjuntos**
   - **Descripción:** Los conjuntos son colecciones desordenadas y mutables de elementos únicos. Son útiles para pruebas de membresía y eliminación de entradas duplicadas.
   - **Creación:** Usa llaves `{}` o la función `set()`.
     - Ejemplo: `mi_conjunto = {1, 2, 3, 4}`
   - **Acceso a Elementos:** Los conjuntos no admiten indexación ni segmentación. Puedes recorrerlos o preguntar si un valor está presente.
     - Ejemplo: `3 en mi_conjunto` da `Verdadero`.
   - **Modificación de Conjuntos:** Puedes añadir o eliminar elementos.
     - Ejemplo: `mi_conjunto.add(5)`

### Diccionarios
4. **Diccionarios**
   - **Descripción:** Los diccionarios son colecciones desordenadas de pares clave-valor. Son mutables y están indexados por claves.
   - **Creación:** Usa llaves `{}` con pares de clave-valor.
     - Ejemplo: `mi_diccionario = {"nombre": "Alice", "edad": 25}`
   - **Acceso a Elementos:** Accede a los valores usando sus claves.
     - Ejemplo: `mi_diccionario["nombre"]` da `"Alice"`.
   - **Modificación de Diccionarios:** Añade o cambia elementos usando claves.
     - Ejemplo: `mi_diccionario["edad"] = 26`

Entender estas estructuras de datos es crucial, ya que se utilizan para almacenar y organizar datos en Python. Cada una tiene sus propias características y se utiliza en diferentes escenarios. ¡Experimenta con ellas para ver cómo funcionan y cómo pueden aplicarse en diversas situaciones de programación!

# Ejemplos

## Listas

Las listas son colecciones ordenadas y modificables. Pueden contener elementos de diferentes tipos.

### Ejemplos:

```python
# Creando una lista
frutas = ["manzana", "banana", "cereza"]

# Accediendo a elementos de la lista
print(frutas[0])  # manzana

# Añadiendo elementos a la lista
frutas.append("naranja")

# Eliminando elementos de la lista
frutas.remove("banana")
```

## Tuplas

Las tuplas son colecciones ordenadas e inmutables. Una vez creadas, sus elementos no pueden ser modificados.

### Ejemplos:

```python
# Creando una tupla
dimensiones = (20, 50, 30)

# Accediendo a elementos de la tupla
print(dimensiones[1])  # 50

# Intentar cambiar un elemento de la tupla generará un error
# dimensiones[0] = 10  # Esto es un error
```

## Conjuntos

Los conjuntos son colecciones desordenadas y sin elementos duplicados. Son útiles para pruebas de pertenencia y eliminación de duplicados.

### Ejemplos:

```python
# Creando un conjunto
colores = {"rojo", "verde", "azul"}

# Añadiendo elementos al conjunto
colores.add("amarillo")

# Eliminando elementos del conjunto
colores.discard("verde")
```

## Diccionarios

Los diccionarios son colecciones desordenadas con un par clave-valor. Son optimizados para recuperar valores cuando se conoce la clave.

### Ejemplos:

```python
# Creando un diccionario
persona = {
    "nombre": "Carlos",
    "edad": 30,
    "profesion": "Ingeniero"
}

# Accediendo a elementos del diccionario
print(persona["nombre"])  # Carlos

# Añadiendo o modificando elementos
persona["edad"] = 31
persona["hobby"] = "fotografía"
```

Estos ejemplos demuestran cómo utilizar las estructuras de datos básicas en Python. Cada estructura tiene sus características y usos específicos, siendo fundamentales para el manejo efectivo de la información en la programación.
