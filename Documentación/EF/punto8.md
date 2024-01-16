# Manejo de Archivos

### Lectura y Escritura de Archivos
1. **Lectura y Escritura de Archivos**
   - **Concepto Básico:** El manejo de archivos en Python te permite leer datos de archivos y escribir datos en archivos. Esto es crucial para el almacenamiento, recuperación y procesamiento de datos.
   - **Abrir un Archivo:** Usa la función `open()` con el nombre del archivo y el modo ('r' para leer, 'w' para escribir, 'a' para añadir, 'r+' para leer y escribir).
     - Ejemplo: `archivo = open('miarchivo.txt', 'r')`
   - **Leyendo un Archivo:** Puedes leer todo el archivo con `read()` o línea por línea con `readline()` o `readlines()`.
     - Ejemplo: `contenido = archivo.read()` lee el archivo entero.
   - **Escribir en un Archivo:** Abre el archivo en modo de escritura o añadido y usa `write()` o `writelines()` para escribir.
     - Ejemplo: `archivo.write("¡Hola, Python!")` escribe en el archivo.
   - **Cerrar un Archivo:** Siempre cierra el archivo usando `close()` para liberar recursos del sistema.
     - Ejemplo: `archivo.close()`

### Trabajando con Diferentes Formatos de Archivo
2. **Trabajando con Diferentes Formatos de Archivo**
   - **Archivos de Texto:** Lee y escribe directamente utilizando los métodos mencionados anteriormente.
   - **Archivos CSV:** Utiliza el módulo `csv` para manejar el formato de valores separados por comas.
     - Ejemplo:
       ```python
       import csv
       with open('ejemplo.csv', 'r') as archivo_csv:
           lector = csv.reader(archivo_csv)
           for fila in lector:
               print(fila)
       ```
   - **Archivos JSON:** El módulo `json` se utiliza para datos JSON.
     - Ejemplo:
       ```python
       import json
       with open('datos.json', 'r') as archivo_json:
           datos = json.load(archivo_json)
           print(datos)
       ```

### Gestores de Contexto (La Declaración `with`)
3. **Gestores de Contexto (La Declaración `with`)**
   - **Propósito:** Maneja automáticamente la apertura y cierre de archivos. Esto es más eficiente y reduce el riesgo de errores relacionados con archivos.
   - **Ejemplo:**
     ```python
     with open('miarchivo.txt', 'r') as archivo:
         contenido = archivo.read()
         print(contenido)
     ```
     Aquí, el archivo se cierra automáticamente después de salir del bloque `with`, incluso si ocurre un error dentro del bloque.

El manejo de archivos es un aspecto fundamental de la programación en Python, especialmente cuando se trata de datos. Entender cómo abrir, leer, escribir y cerrar archivos correctamente es esencial para cualquier tarea de manipulación de datos. Recuerda siempre manejar tus archivos con cuidado para prevenir la pérdida o corrupción de datos.
