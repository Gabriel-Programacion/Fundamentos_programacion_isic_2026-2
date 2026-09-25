# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
El mayor reto fue entender para qué servía realmente usar una variable de bandera (boolean) como `alertaActivada` en lugar de solo mandar un mensaje en pantalla[cite: 12, 23]. Me confundía un poco si debía inicializarla en `FALSO` desde el principio o si el programa lo hacía solo[cite: 12, 23]. También se me dificultó no poner la cláusula `Sino` porque la regla decía usar solo la estructura simple `Si-Entonces`[cite: 12].

## 2. Errores Cometidos durante la Depuración
Al probar el programa en la consola, me marcaba error porque olvidé cambiar el valor de la bandera a `VERDADERO` dentro de la condición cuando el uso de la CPU superaba el 85.0%[cite: 12, 23]. La corrección aplicada fue asignarle explícitamente `alertaActivada <- VERDADERO` únicamente en la rama afirmativa de la decisión[cite: 12, 23].

## 3. Conclusión Técnica
Esta práctica me sirvió para entender cómo funcionan los condicionales simples y para qué se utilizan las banderas en programación[cite: 12, 23]. Aprendí que una bandera actúa como un interruptor en la memoria que nos permite guardar un estado importante para consultarlo o mostrarlo al final de la ejecución del programa[cite: 12, 23].