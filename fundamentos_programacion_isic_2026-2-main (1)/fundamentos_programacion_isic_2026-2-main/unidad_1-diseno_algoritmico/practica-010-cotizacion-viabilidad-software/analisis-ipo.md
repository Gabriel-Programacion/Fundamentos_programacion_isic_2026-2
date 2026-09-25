## Práctica 10: Integrador: Calculadora Presupuestal y Aprobación de Proyecto de Software

### 1. Planteamiento del Problema
Una consultora de software necesita estimar el presupuesto de un proyecto basándose en las horas de desarrollo necesarias. Además, se deben calcular impuestos, un descuento por convenio, desglosar el tiempo en semanas y días de trabajo, y evaluar mediante lógica booleana la viabilidad presupuestal e imprevistos del cliente.

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `nombreProyecto` (Texto)<br>`horasDesarrollo` (Entero)<br>`costoHora` (Real)<br>`presupuestoCliente` (Real)<br>`plazoClienteDias` (Entero) | **Constantes:**<br>`JORNADA_DIARIA = 8`<br>`DIAS_SEMANA = 5`<br><br>**Cálculos Financieros:**<br>`subtotal = horasDesarrollo * costoHora`<br>`imprevistos = subtotal * 0.12`<br>`descuento = subtotal * 0.05`<br>`costoTotalNeto = subtotal + imprevistos - descuento`<br>`impuestoIVA = costoTotalNeto * 0.16`<br>`granTotal = costoTotalNeto + impuestoIVA`<br><br>**Cálculos de Tiempo:**<br>`diasTotales = TRUNC(horasDesarrollo / JORNADA_DIARIA)`<br>`horasSobrantes = horasDesarrollo mod JORNADA_DIARIA`<br>`semanasLaborales = TRUNC(diasTotales / DIAS_SEMANA)`<br><br>**Evaluaciones Booleanas:**<br>`presupuestoViable = (granTotal <= presupuestoCliente)`<br>`plazoViable = (diasTotales <= plazoClienteDias)`<br>`proyectoAprobado = presupuestoViable AND plazoViable` | `nombreProyecto` (Texto)<br>`subtotal` (Real)<br>`imprevistos` (Real)<br>`descuento` (Real)<br>`costoTotalNeto` (Real)<br>`impuestoIVA` (Real)<br>`granTotal` (Real)<br>`diasTotales` (Entero)<br>`horasSobrantes` (Entero)<br>`semanasLaborales` (Entero)<br>`presupuestoViable` (Booleano)<br>`plazoViable` (Booleano)<br>`proyectoAprobado` (Booleano) |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Solicitar `nombreProyecto`, `horasDesarrollo`, `costoHora`, `presupuestoCliente` y `plazoClienteDias`.
3. Inicializar las constantes `JORNADA_DIARIA = 8` y `DIAS_SEMANA = 5`.
4. Calcular `subtotal = horasDesarrollo * costoHora`.
5. Calcular `imprevistos` (12% del subtotal) y `descuento` (5% del subtotal).
6. Calcular `costoTotalNeto = subtotal + imprevistos - descuento`.
7. Calcular `impuestoIVA = costoTotalNeto * 0.16`.
8. Calcular `granTotal = costoTotalNeto + impuestoIVA`.
9. Calcular `diasTotales = TRUNC(horasDesarrollo / JORNADA_DIARIA)` y `horasSobrantes = horasDesarrollo mod JORNADA_DIARIA`.
10. Calcular `semanasLaborales = TRUNC(diasTotales / DIAS_SEMANA)`.
11. Evaluar si `granTotal <= presupuestoCliente` y guardar en `presupuestoViable`.
12. Evaluar si `diasTotales <= plazoClienteDias` y guardar en `plazoViable`.
13. Evaluar `proyectoAprobado = presupuestoViable AND plazoViable`.
14. Desplegar los montos monetarios, el desglose de tiempo y los resultados booleanos de aprobación del proyecto.
15. Fin del algoritmo.