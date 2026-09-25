Algoritmo Practica08_DictamenBeca
	// Declaración de variables
	Definir promedioGeneral Como Real
	Definir creditosAprobados Como Entero
	Definir esElegible Como Logico
	
	// Entrada de datos
	Escribir "Ingrese el promedio general del estudiante:"
	Leer promedioGeneral
	
	Escribir "Ingrese la cantidad de créditos aprobados:"
	Leer creditosAprobados
	
	// Proceso lógico compuesto
	esElegible <- (promedioGeneral >= 85.0) Y (creditosAprobados >= 45)
	
	// Salida de datos
	Escribir "----------------------------------------"
	Escribir "       DICTAMEN DE BECA DE INVESTIGACIÓN "
	Escribir "----------------------------------------"
	Escribir "Candidato es Elegible (VERDADERO/FALSO): ", esElegible
	Escribir "----------------------------------------"
FinAlgoritmo