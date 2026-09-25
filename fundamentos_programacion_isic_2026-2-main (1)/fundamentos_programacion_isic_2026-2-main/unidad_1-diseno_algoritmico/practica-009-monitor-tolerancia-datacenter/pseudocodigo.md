Algoritmo Practica09_MonitorDatacenter
	// Declaración de variables
	Definir temperatura, humedad Como Real
	Definir tempOk, humedadOk Como Logico
	Definir operacionNormativa, alertaRiesgo Como Logico
	
	// Entrada de datos
	Escribir "Ingrese la lectura actual de temperatura (°C):"
	Leer temperatura
	
	Escribir "Ingrese la lectura actual de humedad relativa (%):"
	Leer humedad
	
	// Procesos lógicos de evaluación
	tempOk <- (temperatura >= 18.0) Y (temperatura <= 24.0)
	humedadOk <- (humedad >= 40.0) Y (humedad <= 60.0)
	
	operacionNormativa <- tempOk Y humedadOk
	alertaRiesgo <- (temperatura > 24.0) O (humedad > 60.0)
	
	// Salida de datos
	Escribir "----------------------------------------"
	Escribir "     MONITOR DE AMBIENTE DATACENTER     "
	Escribir "----------------------------------------"
	Escribir "Operación Normativa (VERDADERO/FALSO): ", operacionNormativa
	Escribir "Alerta de Riesgo    (VERDADERO/FALSO): ", alertaRiesgo
	Escribir "----------------------------------------"
FinAlgoritmo