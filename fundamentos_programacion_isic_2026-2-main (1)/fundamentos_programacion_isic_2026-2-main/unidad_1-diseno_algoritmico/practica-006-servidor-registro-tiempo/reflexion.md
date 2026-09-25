# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
Esta fue de las prácticas que más me costó trabajo porque no entendía bien qué hacía la función `TRUNC` ni cómo funcionaba el operador de módulo (`mod` o `%`). No comprendía cómo sacar las horas y los segundos sobrantes al mismo tiempo. Lo resolví haciendo la división a mano en una hoja para ver qué parte era el cociente entero y qué parte era el residuo.

## 2. Errores Cometidos durante la Depuración
En la ejecución paso a paso me marcaba error o me daba decimales raros en los minutos porque estaba usando una división normal (`/`) en vez de aplicar `TRUNC`. Lo corregí envolviendo la división dentro de `TRUNC(segundosRestantes / 60)` y asegurándome de declarar todas las variables como tipo Entero.

## 3. Conclusión Técnica
Fue muy útil aprender a desglosar unidades numéricas puramente con matemática entera y residuo (`mod`). Hacerlo sin condicionales demuestra que la aritmética básica bien estructurada es suficiente para resolver problemas de conversión de tiempo.