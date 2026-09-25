Algoritmo Practica06_DesgloseTiempoUptime
	// Declaración de variables enteras
	Definir segundosTotales Como Entero
	Definir horas, segundosRestantes, minutos, segundosFinales Como Entero
	
	// Entrada de datos
	Escribir "Ingrese la cantidad entera de segundos totales:"
	Leer segundosTotales
	
	// Procesos
	horas <- TRUNC(segundosTotales / 3600)
	segundosRestantes <- segundosTotales Mod 3600
	minutos <- TRUNC(segundosRestantes / 60)
	segundosFinales <- segundosRestantes Mod 60
	
	// Salida de datos
	Escribir "----------------------------------------"
	Escribir "      DESGLOSE DE TIEMPO (UPTIME)       "
	Escribir "----------------------------------------"
	Escribir "Horas completas   : ", horas
	Escribir "Minutos completos : ", minutos
	Escribir "Segundos finales  : ", segundosFinales
	Escribir "----------------------------------------"
FinAlgoritmo