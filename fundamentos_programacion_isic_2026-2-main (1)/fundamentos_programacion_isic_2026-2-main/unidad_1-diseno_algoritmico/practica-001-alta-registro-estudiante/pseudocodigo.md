Algoritmo Practica01_AltaEstudiante
	// Declaración de variables
	Definir numeroControl Como Entero
	Definir nombreCompleto Como Cadena
	Definir promedioPrepa Como Real
	Definir estatusDocumentos Como Logico
	
	// Entrada de datos
	Escribir "Ingrese el número de control:"
	Leer numeroControl
	
	Escribir "Ingrese el nombre completo del estudiante:"
	Leer nombreCompleto
	
	Escribir "Ingrese el promedio de preparatoria:"
	Leer promedioPrepa
	
	Escribir "Ingrese el estatus de documentos completados (Verdadero/Falso):"
	Leer estatusDocumentos
	
	// Salida de datos (Ficha escolar impresa)
	Escribir "----------------------------------------"
	Escribir "       FICHA DE REGISTRO ESCOLAR       "
	Escribir "----------------------------------------"
	Escribir "Número de Control : ", numeroControl
	Escribir "Nombre Completo   : ", nombreCompleto
	Escribir "Promedio Prepa    : ", promedioPrepa
	Escribir "Documentos OK     : ", estatusDocumentos
	Escribir "----------------------------------------"
FinAlgoritmo