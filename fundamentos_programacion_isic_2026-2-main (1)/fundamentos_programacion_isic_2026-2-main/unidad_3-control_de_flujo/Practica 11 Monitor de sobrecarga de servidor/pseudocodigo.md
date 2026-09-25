# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 11: Monitor de Sobrecarga de Servidor

### 1. Planteamiento del Problema
Un servidor web monitorea su porcentaje de uso de CPU. Si el uso excede el 85.0%, debe emitirse un mensaje de advertencia y activar la variable de bandera de alerta. En caso contrario, el programa finaliza su reporte sin alterar la bandera.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `usoCPU` (Real) | Inicializar `alertaActivada <- FALSO`.<br>Si `usoCPU > 85.0` Entonces `alertaActivada <- VERDADERO`. | Porcentaje medido, estado de la bandera `alertaActivada` y mensaje de advertencia si aplica. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Inicializar la variable `alertaActivada` en `FALSO`.
3. Pedir al usuario que ingrese el `usoCPU`.
4. Evaluar si `usoCPU` es mayor a `85.0`.
5. Si la condición se cumple, cambiar `alertaActivada` a `VERDADERO` y mostrar el mensaje `"ALERTA: Uso crítico de CPU"`.
6. Mostrar el porcentaje medido y el estado final de la bandera `alertaActivada`.
7. Fin del algoritmo.