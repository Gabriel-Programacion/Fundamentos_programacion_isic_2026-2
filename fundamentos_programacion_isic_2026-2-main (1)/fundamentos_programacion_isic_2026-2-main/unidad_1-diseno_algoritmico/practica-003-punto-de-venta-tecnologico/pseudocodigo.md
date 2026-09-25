Algoritmo Practica03_PuntoDeVenta
	// Declaración de variables y constantes
	Definir precioProd1, precioProd2, precioProd3 Como Real
	Definir subtotal, montoIVA, totalFinal Como Real
	Definir COSTO_ENVIO Como Real
	COSTO_ENVIO <- 150.00
	
	// Entrada de datos
	Escribir "Ingrese el precio del Producto 1:"
	Leer precioProd1
	
	Escribir "Ingrese el precio del Producto 2:"
	Leer precioProd2
	
	Escribir "Ingrese el precio del Producto 3:"
	Leer precioProd3
	
	// Procesos
	subtotal <- precioProd1 + precioProd2 + precioProd3
	montoIVA <- subtotal * 0.16
	totalFinal <- subtotal + montoIVA + COSTO_ENVIO
	
	// Salida de datos
	Escribir "----------------------------------------"
	Escribir "         DESGLOSE DE COMPRA             "
	Escribir "----------------------------------------"
	Escribir "Subtotal acumulado : $", subtotal
	Escribir "Monto IVA (16%)    : $", montoIVA
	Escribir "Costo de Envío     : $", COSTO_ENVIO
	Escribir "Total Final a pagar: $", totalFinal
	Escribir "----------------------------------------"
FinAlgoritmo