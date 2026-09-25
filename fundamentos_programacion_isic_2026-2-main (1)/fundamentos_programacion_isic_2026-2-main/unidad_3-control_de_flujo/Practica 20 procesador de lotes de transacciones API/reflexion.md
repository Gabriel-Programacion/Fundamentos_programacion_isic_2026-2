# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
Como esta práctica junta todo lo visto (ciclos, condicionales anidados, contadores, acumuladores y validaciones), me sentí abrumado al principio[cite: 21, 23]. El mayor reto fue coordinar el orden de todo: mostrar el menú, validar el tipo de transacción, comprobar que el monto fuera positivo y revisar si había saldo suficiente antes de restar dinero[cite: 10, 11, 21, 23].

## 2. Errores Cometidos durante la Depuración
Me salía el error "La variable no existe" o "La asignación de valores solo se realiza en campos variables" porque en el diagrama intenté poner comparaciones en el bloque de lectura o no había leído el `monto` antes de evaluarlo en el rombo[cite: 10, 11, 23]. Lo corregí asegurándome de usar un trapezoide exclusivo para leer `monto` justo antes del rombo `monto > 0`[cite: 10, 11, 23].

## 3. Conclusión Técnica
Este proyecto integrador me sirvió para entender cómo interactúan los componentes de control de flujo en un programa real más complejo[cite: 21, 23]. Comprendí cómo llevar un control de estado en tiempo real (`saldoCuenta`), hacer validaciones estrictas y producir un balance financiero estructurado al terminar el lote[cite: 21, 23].