# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 12: Validador de Autenticación de Usuario

### 1. Planteamiento del Problema
Un módulo de login valida las credenciales de un administrador mediante un número PIN de acceso de 4 dígitos. Si el PIN ingresado coincide con la constante definida, se concede el acceso; de lo contrario, se deniega.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `pinIngresado` (Entero) | Definir constante `PIN_CORRECTO = 4321`.<br>Si `pinIngresado == PIN_CORRECTO` Entonces conceder acceso, Sino denegar acceso. | Mensaje de autorización ("Acceso Concedido") o rechazo ("Acceso Denegado: PIN Incorrecto"). |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Definir la constante `PIN_CORRECTO` con valor `4321`.
3. Pedir al usuario que ingrese su `pinIngresado`.
4. Comparar si `pinIngresado` es igual a `PIN_CORRECTO`.
5. Si coinciden, mostrar el mensaje `"Acceso Concedido"`.
6. Si no coinciden, mostrar el mensaje `"Acceso Denegado: PIN Incorrecto"`.
7. Fin del algoritmo.