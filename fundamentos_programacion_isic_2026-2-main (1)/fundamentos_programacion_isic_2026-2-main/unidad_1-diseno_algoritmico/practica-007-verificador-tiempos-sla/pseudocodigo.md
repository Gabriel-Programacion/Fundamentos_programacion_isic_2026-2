Algoritmo Practica07_VerificadorSLA
	// Declaración de variables y constante
	Definir tiempoRespuesta Como Real
	Definir cumpleSLA Como Logico
	Definir SLA_LIMITE Como Real
	SLA_LIMITE <- 200.0
	
	// Entrada de datos
	Escribir "Ingrese el tiempo de respuesta registrado en milisegundos (ms):"
	Leer tiempoRespuesta
	
	// Proceso relacional directo
	cumpleSLA <- (tiempoRespuesta <= SLA_LIMITE)
	
	// Salida de datos
	Escribir "----------------------------------------"
	Escribir "      AUDITORÍA DE SERVICIO SLA         "
	Escribir "----------------------------------------"
	Escribir "Tiempo de Respuesta (ms): ", tiempoRespuesta
	Escribir "Cumple SLA (<= 200ms)   : ", cumpleSLA
	Escribir "----------------------------------------"
FinAlgoritmo