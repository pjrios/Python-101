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
