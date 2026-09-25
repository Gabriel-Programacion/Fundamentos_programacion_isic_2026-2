## Práctica 08: Dictamen Booleano de Candidato a Beca de Investigación

### 1. Planteamiento del Problema
El departamento de investigación ofrece una beca a estudiantes que cumplan con dos criterios simultáneos: Promedio general igual o superior a 85.0 Y haber aprobado un mínimo de 45 créditos.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `promedioGeneral` (Real)<br>`creditosAprobados` (Entero) | `esElegible = (promedioGeneral >= 85.0) AND (creditosAprobados >= 45)` | Valor booleano de la variable `esElegible`. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Solicitar la entrada de `promedioGeneral` y `creditosAprobados`.
3. Evaluar la conjunción lógica `(promedioGeneral >= 85.0) AND (creditosAprobados >= 45)`.
4. Guardar la respuesta booleana resultante en la variable `esElegible`.
5. Imprimir el valor de `esElegible` en pantalla.
6. Fin del algoritmo.