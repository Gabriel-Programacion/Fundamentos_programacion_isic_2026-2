# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
Lo difícil fue cambiar mi chip mental para no usar un `Si-Entonces`. Como el problema pedía saber si cumplía o no un límite, yo quería usar un condicional, pero la restricción pedía asignación directa. Lo resolví guardando el resultado de la comparación relacional directamente en una variable de tipo Lógico.

## 2. Errores Cometidos durante la Depuración
Cometí un error de operador relacional al poner el signo de mayor que (`>`) en lugar de menor o igual que (`<=`), lo que hacía que el programa me diera `FALSO` cuando el tiempo de respuesta era rápido. La corrección fue cambiar el operador a `tiempoRespuesta <= SLA_LIMITE`.

## 3. Conclusión Técnica
Esta práctica me enseñó que las expresiones relacionales generan valores booleanos por sí solas, lo que permite evaluar el cumplimiento de una regla dentro de un flujo secuencial sin necesidad de bifurcar el código.