Algoritmo Practica04_CanalizacionFibraOptica
	// Declaración de variables y constante
	Definir radio, longitud Como Real
	Definir areaBase, areaLateral, volumen Como Real
	Definir PI_VALOR Como Real
	PI_VALOR <- 3.14159265
	
	// Entrada de datos
	Escribir "Ingrese el radio del ducto cilíndrico:"
	Leer radio
	
	Escribir "Ingrese la longitud del ducto cilíndrico:"
	Leer longitud
	
	// Procesos
	areaBase <- PI_VALOR * (radio * radio)
	areaLateral <- 2 * PI_VALOR * radio * longitud
	volumen <- PI_VALOR * (radio * radio) * longitud
	
	// Salida de datos
	Escribir "----------------------------------------"
	Escribir "     DIMENSIONAMIENTO DEL DUCTO         "
	Escribir "----------------------------------------"
	Escribir "Área de la base : ", areaBase, " unidades cuadradas"
	Escribir "Área lateral    : ", areaLateral, " unidades cuadradas"
	Escribir "Volumen total   : ", volumen, " unidades cúbicas"
	Escribir "----------------------------------------"
FinAlgoritmo