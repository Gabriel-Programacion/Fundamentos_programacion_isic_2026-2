# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 16: Acumulador de Transferencia de Archivos

### 1. Planteamiento del Problema
Un gestor de descargas tiene un límite de cuota de datos de 100.0 MB. El usuario ingresa el tamaño de varios archivos a descargar uno por uno. El proceso se detiene cuando la suma acumulada alcanza o supera la cuota.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `tamanoArchivo` (Real) en cada iteración. | Inicializar `totalDescargado <- 0.0` y `numArchivos <- 0`.<br>Mientras `totalDescargado < 100.0` Hacer:<br>- `totalDescargado <- totalDescargado + tamanoArchivo`<br>- `numArchivos <- numArchivos + 1`. | Avance actual tras cada archivo, total final acumulado en MB y cantidad de archivos procesados. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Inicializar `totalDescargado` en 0.0 y `numArchivos` en 0.
3. Mientras `totalDescargado` sea menor a 100.0:
   a. Solicitar el `tamanoArchivo` en MB.
   b. Sumar `tamanoArchivo` a `totalDescargado`.
   c. Incrementar en 1 el contador `numArchivos`.
   d. Mostrar el avance acumulado actual.
4. Al superar o alcanzar el límite, mostrar el total final descargado y la cantidad de archivos procesados.
5. Fin del algoritmo.