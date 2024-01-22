# Módulos y Paquetes

### Entendiendo los Módulos
1. **Entendiendo los Módulos**
   - **Módulo:** Un módulo en Python es un archivo que contiene definiciones y declaraciones de Python. El nombre del archivo es el nombre del módulo con el sufijo `.py`.
   - **Propósito:** Los módulos se utilizan para organizar el código en partes manejables. Puedes definir funciones, clases y variables en un módulo.
   - **Importando un Módulo:** Usa la declaración `import`. Por ejemplo, `import math` importará el módulo de matemáticas.
   - **Accediendo al Contenido del Módulo:** Usa el nombre del módulo seguido de un punto y el nombre del atributo. Por ejemplo, `math.sqrt(4)`.

### Creando Tus Propios Módulos
2. **Creando Tus Propios Módulos**
   - **Cómo Crear:** Escribe código Python (funciones, variables, clases, etc.) en un archivo `.py`. Este archivo es tu módulo.
   - **Ejemplo:** Si creas un archivo `mimodulo.py` con una función `saludar()`, puedes importarlo usando `import mimodulo` y llamar a la función usando `mimodulo.saludar()`.

### Entendiendo los Paquetes
3. **Entendiendo los Paquetes**
   - **Paquete:** Un paquete es una forma de recopilar módulos relacionados dentro de una jerarquía similar a un árbol. Los paquetes muy complejos a veces se llaman "bibliotecas".
   - **Estructura:** Un paquete a menudo contiene múltiples módulos. Se define con un directorio y un archivo especial llamado `__init__.py`.
   - **Importando desde Paquetes:** Puedes importar módulos específicos de un paquete. Por ejemplo, si hay un módulo llamado `mimodulo` en un paquete llamado `mipaquete`, lo importas usando `from mipaquete import mimodulo`.

### Utilizando las Bibliotecas Estándar
4. **Utilizando las Bibliotecas Estándar**
   - **Biblioteca Estándar:** Python viene con un conjunto de módulos estándar que puedes usar sin instalar nada más.
   - **Ejemplos:** `os` para interactuar con el sistema operativo, `datetime` para operaciones de fecha y hora, `math` para funciones matemáticas y muchos más.
   - **Importar y Usar:** Importa estas bibliotecas usando la declaración `import` y usa sus funciones y clases en tu código.

Entender cómo usar módulos y paquetes es crucial para escribir código Python bien organizado y eficiente.
