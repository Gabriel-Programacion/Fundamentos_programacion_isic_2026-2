## Práctica 03: Punto de Venta de Equipo Tecnológico

### 1. Planteamiento del Problema
Una tienda de componentes informáticos requiere calcular el total a pagar por la compra de tres productos diferentes (ej. Procesador, RAM, SSD), incluyendo un costo fijo de envío y el desglose del Impuesto al Valor Agregado (IVA del 16%).

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `precioProd1` (Real)<br>`precioProd2` (Real)<br>`precioProd3` (Real) | `subtotal = precioProd1 + precioProd2 + precioProd3`<br>`montoIVA = subtotal * 0.16`<br>`totalFinal = subtotal + montoIVA + 150.00` | Subtotal, IVA, Costo de Envío y Total Final a pagar. |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Solicitar los precios unitarios de los tres productos (`precioProd1`, `precioProd2`, `precioProd3`).
3. Calcular el `subtotal` sumando los tres precios unitarios.
4. Calcular el `montoIVA` multiplicando el `subtotal` por 0.16.
5. Calcular el `totalFinal` sumando `subtotal` + `montoIVA` + 150.00 (costo fijo de envío).
6. Desplegar el desglose comercial completo con Subtotal, IVA, Costo de Envío y Total Final.
7. Fin del algoritmo.