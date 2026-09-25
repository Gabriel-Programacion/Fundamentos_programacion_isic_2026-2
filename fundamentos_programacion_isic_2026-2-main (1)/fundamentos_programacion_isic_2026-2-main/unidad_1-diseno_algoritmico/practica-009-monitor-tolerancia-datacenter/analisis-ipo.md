## Práctica 09: Monitor Booleano de Tolerancia en Datacenter

### 1. Planteamiento del Problema
Un servidor de misión crítica debe operar dentro de límites estrictos de ambiente: Temperatura entre 18.0 °C y 24.0 °C, y Humedad Relativa entre 40% y 60%.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `temperatura` (Real)<br>`humedad` (Real) | `tempOk = (temperatura >= 18.0) AND (temperatura <= 24.0)`<br>`humedadOk = (humedad >= 40.0) AND (humedad <= 60.0)`<br>`operacionNormativa = tempOk AND humedadOk`<br>`alertaRiesgo = (temperatura > 24.0) OR (humedad > 60.0)` | Valores booleanos de `operacionNormativa` y `alertaRiesgo`. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Capturar los valores actuales de `temperatura` y `humedad`.
3. Evaluar si la temperatura está en el rango normativo y guardar en `tempOk`.
4. Evaluar si la humedad está en el rango normativo y guardar en `humedadOk`.
5. Evaluar `operacionNormativa = tempOk AND humedadOk`.
6. Evaluar `alertaRiesgo = (temperatura > 24.0) OR (humedad > 60.0)`.
7. Mostrar los estados booleanos `operacionNormativa` y `alertaRiesgo`.
8. Fin del algoritmo.