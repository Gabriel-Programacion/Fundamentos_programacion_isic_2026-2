## Práctica 07: Verificador Relacional de Acuerdos de Nivel de Servicio (SLA)

### 1. Planteamiento del Problema
Un centro de datos garantiza a sus clientes que el tiempo de respuesta de su API no superará los 200 ms. Se requiere un módulo de auditoría que evalúe si una medición registrada cumple el acuerdo SLA.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `tiempoRespuesta` (Real) | `SLA_LIMITE = 200.0`<br>`cumpleSLA = (tiempoRespuesta <= SLA_LIMITE)` | Estado booleano de cumplimiento (`VERDADERO` o `FALSO`) almacenado en `cumpleSLA`. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Solicitar la entrada del `tiempoRespuesta` en milisegundos.
3. Definir la constante `SLA_LIMITE = 200.0`.
4. Evaluar la expresión relacional `tiempoRespuesta <= SLA_LIMITE` y guardar el resultado lógico en `cumpleSLA`.
5. Mostrar en pantalla el resultado booleano almacenado en `cumpleSLA`.
6. Fin del algoritmo.
