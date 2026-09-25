# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
El reto más grande fue aprender a meter decisiones `Si-Entonces-Sino` adentro de un ciclo que se repite un número exacto $N$ de veces[cite: 20, 23]. Me enredaba bastante pensando cómo llevar la cuenta de tres contadores distintos (`cant200`, `cant4xx`, `cant5xx`) de manera independiente mientras el bucle avanzaba[cite: 20, 23].

## 2. Errores Cometidos durante la Depuración
Al final del ciclo, los contadores de errores `4xx` y `5xx` siempre me marcaban cero aunque metiera códigos como 404 o 500[cite: 20, 23]. Descubrí que había puesto los incrementos fuera del bloque condicional correspondiente[cite: 20, 23]. Lo corregí colocando cada `cant <- cant + 1` dentro de su respectiva rama de clasificación[cite: 20, 23].

## 3. Conclusión Técnica
Esta práctica me ayudó a combinar estructuras selectivas anidadas con estructuras repetitivas[cite: 20, 23]. Aprendí a construir algoritmos capaces de procesar colecciones de datos o lotes de registros para generar reportes estadísticos organizados[cite: 20, 23].