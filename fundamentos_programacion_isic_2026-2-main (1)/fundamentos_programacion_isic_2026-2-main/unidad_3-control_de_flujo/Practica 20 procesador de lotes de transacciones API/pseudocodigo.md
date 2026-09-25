# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 20: Proyecto Integrador: Procesador de Lotes de Transacciones API

### 1. Planteamiento del Problema
Una pasarela de pagos digitales procesa un lote indeterminado de transacciones bancarias. El sistema debe solicitar transacciones (depósitos/retiros) de manera continua hasta que el operador decida finalizar la sesión, realizando validaciones de entradas y balance general.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `opcion` (Entero), `tipo` (Entero), `monto` (Real) repetidamente. | Inicializar `saldoCuenta <- 5000.0`, `totalDepositado <- 0.0`, `totalRetirado <- 0.0`, `exitosas <- 0`, `rechazos <- 0`.<br>Bucle mientras `opcion != 0`:<br>- Validar `monto > 0.0`.<br>- Si `tipo == 1` (Depósito): Incrementar saldo y acumulador, `exitosas <- exitosas + 1`.<br>- Si `tipo == 2` (Retiro): Verificar `monto <= saldoCuenta`. Si cumple, descontar saldo y acumular retiro; si no, emitir alerta e incrementar `rechazos`. | Reporte de auditoría financiera del lote: saldo final, total depositado, total retirado, operaciones exitosas y rechazos. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Inicializar `saldoCuenta = 5000.0`, acumuladores en 0.0 y contadores de operaciones en 0.
3. Iniciar bucle repetitivo para presentar el menú de opciones (1. Procesar Transacción, 0. Finalizar Lote).
4. Si se selecciona procesar transacción:
   a. Solicitar y validar el `tipo` de transacción (1: Depósito, 2: Retiro).
   b. Solicitar el `monto` y verificar que sea mayor a 0.0.
   c. Si es Depósito (1), aumentar `saldoCuenta`, acumular en `totalDepositado` y sumar 1 a `exitosas`.
   d. Si es Retiro (2), evaluar si el `monto` es menor o igual a `saldoCuenta`.
      - Si hay fondos: restar de `saldoCuenta`, acumular en `totalRetirado` y sumar 1 a `exitosas`.
      - Si no hay fondos: mostrar alerta `"Fondos Insuficientes"` y sumar 1 a `rechazos`.
5. Repetir el bucle hasta que el usuario ingrese la opción 0 para finalizar.
6. Desplegar el reporte completo con el saldo final, totales depositados/retirados y conteo de operaciones exitosas y rechazadas.
7. Fin del algoritmo.