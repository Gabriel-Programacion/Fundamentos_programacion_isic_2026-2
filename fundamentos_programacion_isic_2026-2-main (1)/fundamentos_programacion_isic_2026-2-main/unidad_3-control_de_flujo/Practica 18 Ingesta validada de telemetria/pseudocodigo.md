# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 18: Ingesta Validada de Telemetría

### 1. Planteamiento del Problema
Un sensor de temperatura transmite mediciones, pero debido a fallas a veces reporta valores fuera del rango operacional de -50.0°C a 100.0°C. Se debe validar la entrada mediante un bucle para filtrar y rechazar datos inválidos.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `temperatura` (Real). | Ciclo de lectura validada:<br>Repetir<br>- Leer `temperatura`<br>- Si está fuera de rango, mostrar error<br>Hasta Que `temperatura >= -50.0` Y `temperatura <= 100.0`. | Mensajes de error por lecturas fuera de rango y confirmación final de lectura aceptada. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Repetir las siguientes instrucciones:
   a. Pedir la lectura de `temperatura`.
   b. Verificar si `temperatura < -50.0` O `temperatura > 100.0`.
   c. Si está fuera de rango, mostrar mensaje de error notificando el dato inválido.
3. Evaluar condición: Repetir hasta que `temperatura >= -50.0` Y `temperatura <= 100.0`.
4. Mostrar mensaje de confirmación notificando que el dato ingresado fue aceptado por el sistema.
5. Fin del algoritmo.