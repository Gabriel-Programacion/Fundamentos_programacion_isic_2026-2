# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
La dificultad principal estuvo en la formulación matemática de las conversiones. Me confundía al recordar si tenía que multiplicar o dividir entre 1024 según la unidad de medida (si pasaba de GB a MB o a TB). Lo resolví anotando en una libreta las equivalencias de unidades para tener claro la escala y aplicar las operaciones correctas en el código.

## 2. Errores Cometidos durante la Depuración
Al ejecutar paso a paso, en la línea de `capacidadTB` el resultado me daba un número enorme porque por error había puesto una multiplicación (`* 1024`) en lugar de una división (`/ 1024`). La corrección aplicada fue cambiar el operador aritmético a división para que el valor en Terabytes fuera menor que el de Gigabytes.

## 3. Conclusión Técnica
Respetar la secuencialidad pura me ayudó a ver cómo una variable calculada puede reutilizarse inmediatamente en la siguiente línea de código para otro cálculo (como usar `capacidadMB` para obtener `capacidadKB`), logrando un programa eficiente sin necesidad de estructuras complejas.