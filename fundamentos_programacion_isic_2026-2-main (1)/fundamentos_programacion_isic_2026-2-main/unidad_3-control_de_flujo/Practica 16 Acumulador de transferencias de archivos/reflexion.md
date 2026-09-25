# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
Mi mayor confusión fue entender la diferencia práctica entre un contador y un acumulador[cite: 17, 23]. No me quedaba claro por qué a uno se le sumaba `1` (`numArchivos <- numArchivos + 1`) mientras que al otro se le sumaba el valor variable ingresado por el usuario (`totalDescargado <- totalDescargado + tamanoArchivo`)[cite: 17, 23].

## 2. Errores Cometidos durante la Depuración
En las pruebas, el acumulador me sumaba cosas raras o daba números gigantes desde la primera vuelta[cite: 17, 23]. Descubrí que el error fue no inicializar `totalDescargado <- 0.0` antes de entrar al ciclo[cite: 17, 23]. La corrección fue asegurar que ambas variables tuvieran valor `0` al inicio para que sumaran de forma limpia[cite: 17, 23].

## 3. Conclusión Técnica
Esta práctica me ayudó a entender cómo procesar límites de cuota mediante sumas acumulativas en un bucle[cite: 17, 23]. Aprendí a diferenciar el rol de un contador (que registra cuántas veces pasa algo) de un acumulador (que va guardando totales sumados)[cite: 17, 23].