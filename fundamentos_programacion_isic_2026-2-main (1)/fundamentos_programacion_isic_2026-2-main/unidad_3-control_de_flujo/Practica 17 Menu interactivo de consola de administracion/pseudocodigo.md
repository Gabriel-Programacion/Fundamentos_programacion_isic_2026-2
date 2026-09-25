# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 17: Menú Interactivo de Consola de Administración

### 1. Planteamiento del Problema
Una herramienta de diagnóstico de red debe desplegar repetidamente un menú de opciones hasta que el administrador seleccione explícitamente la opción de salida (0), garantizando al menos una ejecución inicial con la estructura `Repetir - Hasta Que`.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `opcion` (Entero) en cada iteración. | Bucle Post-prueba:<br>Repetir<br>- Desplegar menú (1. Ping, 2. Traceroute, 0. Salir)<br>- Leer `opcion`<br>- Ejecutar acción correspondiente<br>Hasta Que `opcion == 0`. | Ejecución reiterada de las opciones seleccionadas y mensaje final de salida. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Repetir las siguientes instrucciones:
   a. Mostrar el menú con las opciones (1. Ping a Servidor, 2. Traceroute, 0. Salir).
   b. Pedir al usuario que ingrese la `opcion`.
   c. Si `opcion` es 1, ejecutar simulación de Ping.
   d. Si `opcion` es 2, ejecutar simulación de Traceroute.
   e. Si `opcion` no es válida y no es 0, mostrar mensaje de opción incorrecta.
3. Evaluar la condición: Repetir hasta que `opcion` sea igual a 0.
4. Mostrar mensaje de finalización del programa.
5. Fin del algoritmo.