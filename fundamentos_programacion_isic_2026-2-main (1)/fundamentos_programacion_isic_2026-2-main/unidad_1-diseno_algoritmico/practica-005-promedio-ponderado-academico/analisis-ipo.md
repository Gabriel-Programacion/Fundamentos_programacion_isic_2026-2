## Práctica 05: Calculadora de Promedio Ponderado de Asignaturas de Sistemas

### 1. Planteamiento del Problema
En la materia de Fundamentos de Programación, la calificación final no es un promedio aritmético simple, sino una evaluación ponderada de cuatro rubros: Exámenes (40%), Prácticas de Laboratorio (30%), Proyecto Integrador (20%) y Autoevaluación/Tareas (10%).

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `notaExamenes` (Real)<br>`notaPracticas` (Real)<br>`notaProyecto` (Real)<br>`notaTareas` (Real) | `promedioPonderado = (notaExamenes * 0.40) + (notaPracticas * 0.30) + (notaProyecto * 0.20) + (notaTareas * 0.10)` | Promedio ponderado final obtenido (`promedioPonderado`). |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Solicitar las calificaciones individuales: `notaExamenes`, `notaPracticas`, `notaProyecto` y `notaTareas`.
3. Aplicar los porcentajes correspondientes mediante la fórmula parentizada para obtener `promedioPonderado`.
4. Mostrar en pantalla el resultado del `promedioPonderado` final.
5. Fin del algoritmo.