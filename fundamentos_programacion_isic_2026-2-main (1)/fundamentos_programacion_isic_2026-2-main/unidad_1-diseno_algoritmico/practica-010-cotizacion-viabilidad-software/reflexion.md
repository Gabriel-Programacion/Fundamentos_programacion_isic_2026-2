# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
Fue la práctica más compleja porque integraba todo lo visto: declaración de muchas variables, constantes, operaciones financieras, desglose de tiempo con `TRUNC`/`mod` y comparaciones lógicas complejas. El reto fue no perder el orden. Lo resolví separando el código por bloques comentados (Entrada, Finanzas, Tiempo, Lógica y Salidas).

## 2. Errores Cometidos durante la Depuración
Tuve un error de depuración al calcular los `diasTotales` porque usé el costo por hora en lugar de la constante `JORNADA_DIARIA`, dando un número gigante de días. Lo corregí revisando la fórmula en la tabla de procesos y cambiando la variable por la constante adecuada (`TRUNC(horasDesarrollo / JORNADA_DIARIA)`).

## 3. Conclusión Técnica
Integrar todo en un solo algoritmo secuencial demuestra que problemas grandes de estimación de proyectos se pueden resolver sin condicionales, ejecutando cálculos financieros, de tiempo y aprobaciones lógicas de forma totalmente lineal y estructurada.