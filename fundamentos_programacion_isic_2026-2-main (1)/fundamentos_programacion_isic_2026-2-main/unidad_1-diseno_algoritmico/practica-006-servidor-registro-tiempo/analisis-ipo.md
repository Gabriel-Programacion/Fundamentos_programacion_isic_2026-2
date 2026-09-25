## Práctica 06: Servidor de Registro de Tiempo y Desglose de Unidades

### 1. Planteamiento del Problema
Un servidor Linux registra el tiempo de actividad (uptime) en segundos acumulados. Se requiere presentar este tiempo traducido a un formato comprensible de Horas, Minutos y Segundos restantes.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `segundosTotales` (Entero) | `horas = TRUNC(segundosTotales / 3600)`<br>`segundosRestantes = segundosTotales mod 3600`<br>`minutos = TRUNC(segundosRestantes / 60)`<br>`segundosFinales = segundosRestantes mod 60` | Horas, Minutos y Segundos desglosados (`horas`, `minutos`, `segundosFinales`). |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Capturar el valor entero de `segundosTotales`.
3. Truncar la división de `segundosTotales` entre 3600 para calcular las `horas` completas.
4. Calcular `segundosRestantes` usando la operación `mod 3600`.
5. Truncar la división de `segundosRestantes` entre 60 para calcular los `minutos` completos.
6. Calcular `segundosFinales` aplicando la operación `mod 60` sobre `segundosRestantes`.
7. Desplegar los valores de `horas`, `minutos` y `segundosFinales`.
8. Fin del algoritmo.