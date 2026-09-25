# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
Lo más difícil fue acordarme de definir e identificar la constante `PIN_CORRECTO` antes de hacer la comparación[cite: 13, 23]. A veces se me olvidaba y quería comparar `pinIngresado` directo contra un número escrito a mano dentro de la condición[cite: 13, 23]. También me daba duda la diferencia de sintaxis entre guardar un valor `=` y comparar dos valores `==`[cite: 13, 23].

## 2. Errores Cometidos durante la Depuración
Durante la ejecución paso a paso el programa aceptaba cualquier PIN porque en el condicional había puesto `=` en lugar de `==` para evaluar la igualdad[cite: 13, 23]. Lo corregí cambiando la expresión dentro del rombo a `pinIngresado == PIN_CORRECTO` para que bifurcara de forma correcta entre conceder o denegar el acceso[cite: 13, 23].

## 3. Conclusión Técnica
Esta práctica me ayudó a dominar la estructura selectiva doble `Si-Entonces-Sino` para manejar alternativas mutuamente excluyentes[cite: 13, 23]. Comprendí cómo la computadora puede tomar una ruta verdadera o una falsa según las credenciales del usuario, asegurando que solo los datos válidos tengan acceso[cite: 13, 23].