# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 14: Dispatcher de Comandos de Consola CLI

### 1. Planteamiento del Problema
Un intérprete de comandos simplificado de administración de servidores ejecuta tareas específicas según una opción numérica seleccionada por el usuario en un menú mediante una estructura selectiva múltiple.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `opcionMenu` (Entero) | Según `opcionMenu` Hacer:<br>Caso 1: Ejecutar reiniciar.<br>Caso 2: Mostrar estado.<br>Caso 3: Limpiar caché.<br>Caso 4: Cerrar sesión.<br>De Otro Modo: Opción no válida. | Mensaje de confirmación de la orden ejecutada o mensaje de error. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Desplegar en pantalla el menú de opciones (1. Reiniciar Servicio, 2. Mostrar Estado, 3. Limpiar Caché, 4. Cerrar Sesión).
3. Pedir al usuario que ingrese la `opcionMenu`.
4. Evaluar la `opcionMenu` mediante la estructura `Según`:
   - Si es 1: Mostrar mensaje de reinicio de servicio.
   - Si es 2: Mostrar mensaje de estado del sistema.
   - Si es 3: Mostrar mensaje de limpieza de caché.
   - Si es 4: Mostrar mensaje de cierre de sesión.
   - De otro modo: Mostrar mensaje de opción no válida.
5. Fin del algoritmo.