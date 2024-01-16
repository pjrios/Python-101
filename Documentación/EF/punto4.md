# Estructuras de Control

### Declaraciones Condicionales (if, else, elif)
1. **Declaraciones Condicionales (if, else, elif)**
   - **Propósito:** Estas declaraciones te permiten ejecutar ciertas partes del código dependiendo de las condiciones.
   - **Declaración if:** Prueba una condición y ejecuta código si la condición es Verdadera.
     - Ejemplo: 
       ```python
       if x > 0:
           print("x es positivo")
       ```
   - **Declaración else:** Usada con if, ejecuta código cuando la condición if es Falsa.
     - Ejemplo:
       ```python
       if x > 0:
           print("x es positivo")
       else:
           print("x no es positivo")
       ```
   - **Declaración elif:** Abreviatura de 'else if'. Permite comprobar múltiples condiciones, una tras otra.
     - Ejemplo:
       ```python
       if x > 0:
           print("x es positivo")
       elif x < 0:
           print("x es negativo")
       else:
           print("x es cero")
       ```

### Bucles
2. **Bucles**
   - **Bucle For:** Itera sobre una secuencia (como una lista, tupla, cadena o rango).
     - Ejemplo:
       ```python
       for i in range(5):
           print(i)
       ```
       Este bucle imprime números del 0 al 4.
   - **Bucle While:** Ejecuta repetidamente una declaración objetivo mientras una condición dada sea verdadera.
     - Ejemplo:
       ```python
       count = 0
       while count < 5:
           print(count)
           count += 1
       ```
       Este bucle imprime números del 0 al 4.

### Declaraciones Break y Continue
3. **Declaraciones Break y Continue**
   - **break:** Se utiliza para salir de un bucle for o while.
     - Ejemplo:
       ```python
       for i in range(10):
           if i == 5:
               break
           print(i)
       ```
       Este bucle se detiene cuando `i` se convierte en 5.
   - **continue:** Omite el resto del cuerpo del bucle y vuelve a probar su condición antes de reiterar.
     - Ejemplo:
       ```python
       for i in range(10):
           if i == 5:
               continue
           print(i)
       ```
       Este bucle omite imprimir el número 5 y continúa con el resto.

Entender las estructuras de control es vital para dirigir el flujo de un programa en Python. Te permiten tomar decisiones y repetir acciones basadas en condiciones. Experimenta con estas estructuras usando diferentes condiciones y bucles para entender cómo influyen en el flujo y la lógica de tu código.
