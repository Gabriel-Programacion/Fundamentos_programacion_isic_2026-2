# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
El mayor desafío fue que eran muchas condiciones juntas para evaluar rangos (mínimos y máximos de temperatura y humedad) y generar dos salidas distintas (`operacionNormativa` y `alertaRiesgo`). Me enredaba un poco con los paréntesis. Lo resolví evaluando primero cada variable por separado y luego combinándolas con `Y` u `O`.

## 2. Errores Cometidos durante la Depuración
Durante la prueba me daba que todo estaba en riesgo aunque la temperatura fuera correcta, porque en la variable `alertaRiesgo` puse el operador `Y` en vez del operador `O`. Lo corregí cambiando a `(temperatura > 24.0) O (humedad > 60.0)` para que la alerta brinque si cualquiera de los dos parámetros se excede.

## 3. Conclusión Técnica
Esta práctica reafirma que se pueden monitorear sistemas complejos de múltiples variables mediante lógica booleana pura, manteniendo el programa limpio, rápido y estrictamente secuencial.