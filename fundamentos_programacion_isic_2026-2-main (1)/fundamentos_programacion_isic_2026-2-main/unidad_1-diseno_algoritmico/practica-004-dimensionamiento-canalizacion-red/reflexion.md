# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
Lo más difícil fue adaptar la fórmula matemática de la geometría de un cilindro a la sintaxis de PSeInt, especialmente el manejo del valor de $\pi$ y el radio al cuadrado. No sabía si PSeInt tenía la constante integrada, así que tuve que declararla manualmente. Lo resolví definiendo `PI_VALOR` como una variable con el valor `3.14159265` y multiplicando el radio por sí mismo.

## 2. Errores Cometidos durante la Depuración
Durante la ejecución paso a paso me daba un resultado equivocado en el área lateral porque me faltaba multiplicar por 2 en la fórmula. La corrección fue revisar la fórmula del libro y ajustar la línea a `2 * PI_VALOR * radio * longitud`.

## 3. Conclusión Técnica
Entender la secuencia lineal en cálculos geométricos es fundamental porque el orden en que se definen las constantes y se capturan las entradas afecta directamente los cálculos posteriores del área y el volumen.