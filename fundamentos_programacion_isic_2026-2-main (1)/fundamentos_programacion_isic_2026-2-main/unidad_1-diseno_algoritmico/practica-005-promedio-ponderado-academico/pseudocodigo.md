Algoritmo Practica05_PromedioPonderado
	// Declaración de variables
	Definir notaExamenes, notaPracticas, notaProyecto, notaTareas Como Real
	Definir promedioPonderado Como Real
	
	// Entrada de datos
	Escribir "Ingrese la nota de Exámenes (0-100):"
	Leer notaExamenes
	
	Escribir "Ingrese la nota de Prácticas de Laboratorio (0-100):"
	Leer notaPracticas
	
	Escribir "Ingrese la nota del Proyecto Integrador (0-100):"
	Leer notaProyecto
	
	Escribir "Ingrese la nota de Tareas/Autoevaluación (0-100):"
	Leer notaTareas
	
	// Proceso mediante expresión única parentizada
	promedioPonderado <- (notaExamenes * 0.40) + (notaPracticas * 0.30) + (notaProyecto * 0.20) + (notaTareas * 0.10)
	
	// Salida de datos
	Escribir "----------------------------------------"
	Escribir "        EVALUACIÓN PONDERADA            "
	Escribir "----------------------------------------"
	Escribir "Promedio Ponderado Final: ", promedioPonderado
	Escribir "----------------------------------------"
FinAlgoritmo