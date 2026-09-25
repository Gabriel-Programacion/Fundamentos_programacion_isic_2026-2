# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 13: Clasificador de Tráfico QoS de Red

### 1. Planteamiento del Problema
Un router con Calidad de Servicio (QoS) asigna prioridades al tráfico según el puerto de destino en rangos específicos: 1 a 1024 (Alta), 1025 a 49151 (Media), 49152 a 65535 (Baja). Cualquier otro número se considera un puerto inválido.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `numeroPuerto` (Entero) | Evaluaciones encadenadas:<br>- Si `numeroPuerto >= 1` Y `numeroPuerto <= 1024` -> Alta<br>- Si `numeroPuerto >= 1025` Y `numeroPuerto <= 49151` -> Media<br>- Si `numeroPuerto >= 49152` Y `numeroPuerto <= 65535` -> Baja<br>- Sino -> Puerto Inválido. | Categoría de prioridad asignada o mensaje de error. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Pedir al usuario que ingrese el `numeroPuerto`.
3. Si `numeroPuerto` está entre 1 y 1024, asignar y mostrar `"Prioridad Alta (Servicios del Sistema)"`.
4. Si no, si `numeroPuerto` está entre 1025 y 49151, asignar y mostrar `"Prioridad Media (Aplicaciones Registradas)"`.
5. Si no, si `numeroPuerto` está entre 49152 y 65535, asignar y mostrar `"Prioridad Baja (Puertos Dinámicos/Privados)"`.
6. Si no cumple ningún rango, mostrar `"Puerto Inválido"`.
7. Fin del algoritmo.