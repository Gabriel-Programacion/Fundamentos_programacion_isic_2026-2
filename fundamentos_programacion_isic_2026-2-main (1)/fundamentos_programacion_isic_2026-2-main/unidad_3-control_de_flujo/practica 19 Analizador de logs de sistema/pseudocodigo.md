# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 19: Analizador de Logs de Sistema

### 1. Planteamiento del Problema
Un servidor procesa un lote de N registros de log de red. Cada registro contiene un código de estado HTTP (200, 4xx, 5xx). Se requiere un reporte estadístico que contabilice cada tipo de evento procesado.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `totalRegistros` (Entero) y `codigoHTTP` (Entero) repetidamente. | Inicializar contadores: `cant200 <- 0`, `cant4xx <- 0`, `cant5xx <- 0`.<br>Ciclo de 1 hasta `totalRegistros`:<br>- Si `codigoHTTP == 200` -> `cant200 <- cant200 + 1`<br>- Si `codigoHTTP >= 400` y `< 500` -> `cant4xx <- cant4xx + 1`<br>- Si `codigoHTTP >= 500` y `< 600` -> `cant5xx <- cant5xx + 1`. | Resumen estadístico mostrando el total acumulado de respuestas exitosas (200), errores de cliente (4xx) y errores de servidor (5xx). |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Inicializar los contadores `cant200`, `cant4xx` y `cant5xx` en 0.
3. Pedir al usuario la cantidad total de registros a procesar (`totalRegistros`).
4. Para cada registro desde 1 hasta `totalRegistros`:
   a. Pedir al usuario el `codigoHTTP`.
   b. Si `codigoHTTP` es igual a 200, incrementar `cant200` en 1.
   c. Si no, si `codigoHTTP` está entre 400 y 499, incrementar `cant4xx` en 1.
   d. Si no, si `codigoHTTP` está entre 500 y 599, incrementar `cant5xx` en 1.
5. Al finalizar el ciclo, desplegar el resumen estadístico con los conteos finales.
6. Fin del algoritmo.