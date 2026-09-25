# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
El mayor desafío fue armar la expresión matemática única respetando la jerarquía de operadores y la parentización correcta para los cuatro rubros evaluados. Al principio no sabía bien dónde poner los paréntesis para que la máquina no sumara antes de multiplicar. Lo resolví agrupando cada multiplicación de nota por su porcentaje dentro de su propio par de paréntesis.

## 2. Errores Cometidos durante la Depuración
Al probar el algoritmo, la calificación me salía muy alta porque ingresé los porcentajes como números enteros (`40`, `30`, etc.) en lugar de sus equivalentes en decimales (`0.40`, `0.30`). Corregí los valores en la fórmula dividiéndolos entre 100 para trabajar con ponderaciones reales.

## 3. Conclusión Técnica
Trabajar este problema de forma estrictamente secuencial me enseñó la importancia de dominar la prioridad de operadores en programación, asegurando que una única fórmula parentizada calcule el resultado exacto sin depender de decisiones condicionales.