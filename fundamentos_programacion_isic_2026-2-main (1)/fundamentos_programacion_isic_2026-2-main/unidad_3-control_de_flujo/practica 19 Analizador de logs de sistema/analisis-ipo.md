# Análisis Entrada-Proceso-Salida (IPO)

## Práctica 01: Alta de Registro de Estudiante en el Sistema Universitario

### 1. Planteamiento del Problema
El Departamento de Servicios Escolares de la universidad requiere un módulo algorítmico inicial para registrar a los alumnos de nuevo ingreso. Se deben almacenar datos de identificación sin procesar condicionalmente la información.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `numeroControl` (Entero)<br>`nombreCompleto` (Texto / Cadena)<br>`promedioPrepa` (Real)<br>`estatusDocumentos` (Lógico) | Lectura secuencial de datos e impresión estructurada. | Ficha escolar impresa con los valores ingresados. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Pedir al usuario que ingrese el `numeroControl`, `nombreCompleto`, `promedioPrepa` y `estatusDocumentos`.
3. Guardar los datos ingresados en sus correspondientes variables respetando la convención camelCase.
4. Generar y desplegar en pantalla la ficha digital formateada con la información del estudiante.
5. Fin del algoritmo.
