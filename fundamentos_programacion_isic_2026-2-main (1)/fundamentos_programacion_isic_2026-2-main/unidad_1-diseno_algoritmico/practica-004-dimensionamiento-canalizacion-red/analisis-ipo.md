## Práctica 04: Dimensionamiento de Canalización para Redes de Fibra Óptica

### 1. Planteamiento del Problema
Un equipo de ingenieros de infraestructura necesita calcular la superficie exterior y el volumen interno de un conducto cilíndrico de protección para cables de fibra óptica.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `radio` (Real)<br>`longitud` (Real) | `PI_VALOR = 3.14159265`<br>`areaBase = PI_VALOR * (radio * radio)`<br>`areaLateral = 2 * PI_VALOR * radio * longitud`<br>`volumen = PI_VALOR * (radio * radio) * longitud` | Áreas y Volumen del ducto en unidades cuadradas y cúbicas (`areaBase`, `areaLateral`, `volumen`). |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Solicitar el `radio` y la `longitud` del ducto cilíndrico.
3. Definir la constante `PI_VALOR` con el valor `3.14159265`.
4. Calcular el `areaBase` multiplicando `PI_VALOR` por el `radio` al cuadrado.
5. Calcular el `areaLateral` usando la fórmula `2 * PI_VALOR * radio * longitud`.
6. Calcular el `volumen` multiplicando `PI_VALOR` por el `radio` al cuadrado por la `longitud`.
7. Mostrar los resultados calculados de `areaBase`, `areaLateral` y `volumen`.
8. Fin del algoritmo.