Algoritmo Practica02_ConversorAlmacenamiento
	// Declaración de variables
	Definir capacidadGB Como Real
	Definir capacidadMB Como Real
	Definir capacidadKB Como Real
	Definir capacidadTB Como Real
	
	// Entrada de datos
	Escribir "Ingrese la capacidad en Gigabytes (GB):"
	Leer capacidadGB
	
	// Procesos
	capacidadMB <- capacidadGB * 1024
	capacidadKB <- capacidadMB * 1024
	capacidadTB <- capacidadGB / 1024
	
	// Salida de datos
	Escribir "----------------------------------------"
	Escribir "     CONVERSIÓN DE ALMACENAMIENTO       "
	Escribir "----------------------------------------"
	Escribir "Capacidad en Kilobytes (KB): ", capacidadKB
	Escribir "Capacidad en Megabytes (MB): ", capacidadMB
	Escribir "Capacidad en Terabytes (TB): ", capacidadTB
	Escribir "----------------------------------------"
FinAlgoritmo