# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
El reto aquí fue organizar la secuencia del cálculo financiero para que no se me revolvieran los precios con el IVA y el costo de envío. Me costaba un poco visualizar cómo acumular el subtotal de tres productos distintos y luego aplicarle el porcentaje correspondiente. Lo resolví desglosando las operaciones paso a paso en lugar de querer calcular todo en una sola línea.

## 2. Errores Cometidos durante la Depuración
Cometí un error de parentización y de sintaxis al calcular el total final porque escribí la fórmula multiplicando por `16` en lugar de `0.16` para el IVA, lo que hizo que el total me saliera gigante. Lo corregí cambiando la tasa decimal a `0.16` para sacar el porcentaje correcto antes de sumarle el costo de envío de $150.

## 3. Conclusión Técnica
Esta práctica demuestra que muchos problemas del mundo real, como una caja de cobro, son completamente secuenciales. Resolverlo sin condicionales me obligó a asegurarme de que el orden aritmético fuera el correcto para que cada resultado intermedio fuera exacto.