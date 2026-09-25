# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
Se me hizo difícil pensar la lógica para "atrapar" al usuario en un bucle hasta que ponga un dato válido[cite: 19, 23]. Me confundí al armar la proposición booleana de la condición, dudando si debía usar `O` o `Y` para validar que la temperatura estuviera en el rango de -50.0 a 100.0[cite: 19, 23].

## 2. Errores Cometidos durante la Depuración
Al probar valores fuera de rango como `150`, el programa los aceptaba y finalizaba en lugar de pedir la lectura otra vez[cite: 19, 23]. Lo solucioné ajustando la expresión lógica del ciclo a `Hasta Que temperatura >= -50.0 Y temperatura <= 100.0` para que no lo deje salir hasta cumplir ambas premisas[cite: 19, 23].

## 3. Conclusión Técnica
La práctica me sirvió para dominar los patrones de validación de entradas de datos con ciclos post-prueba[cite: 19, 23]. Entendí que filtrar los datos erróneos antes de procesarlos es fundamental para mantener la integridad de la información en cualquier sistema[cite: 19, 23].