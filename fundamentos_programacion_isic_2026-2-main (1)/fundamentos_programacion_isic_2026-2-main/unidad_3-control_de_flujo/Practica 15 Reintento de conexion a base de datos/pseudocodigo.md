# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 15: Reintento de Conexión a Base de Datos

### 1. Planteamiento del Problema
Un cliente de base de datos intenta establecer conexión con un servidor remoto. Si la conexión falla, se realiza un reintento hasta alcanzar un límite máximo de 3 intentos o hasta que la contraseña sea correcta.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `passwordIngresada` (Cadena) introducida en cada iteración. | Inicializar `intento <- 1` y `estadoConexion <- FALSO`.<br>Mientras `intento <= 3` Y `estadoConexion == FALSO` Hacer:<br>- Si `passwordIngresada == "dbpass123"` Entonces `estadoConexion <- VERDADERO`<br>- Sino `intento <- intento + 1`. | Estatus final de la conexión (éxito en la conexión o límite de intentos agotado). |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Inicializar la variable `intento` en 1 y `estadoConexion` en `FALSO`.
3. Mientras `intento` sea menor o igual a 3 Y `estadoConexion` sea igual a `FALSO`:
   a. Solicitar al usuario que ingrese la `passwordIngresada`.
   b. Si `passwordIngresada` es igual a `"dbpass123"`, cambiar `estadoConexion` a `VERDADERO`.
   c. De lo contrario, incrementar `intento` en 1.
4. Si `estadoConexion` es `VERDADERO`, mostrar mensaje de conexión exitosa.
5. Si no, mostrar mensaje de intentos agotados.
6. Fin del algoritmo.