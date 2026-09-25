Algoritmo Practica10_CalculadoraProyecto
	// Declaración de variables
	Definir nombreProyecto Como Cadena
	Definir horasDesarrollo, plazoClienteDias Como Entero
	Definir costoHora, presupuestoCliente Como Real
	
	// Variables financieras
	Definir subtotal, imprevistos, descuento, costoTotalNeto, impuestoIVA, granTotal Como Real
	
	// Variables de tiempo
	Definir diasTotales, horasSobrantes, semanasLaborales Como Entero
	
	// Variables lógicas
	Definir presupuestoViable, plazoViable, proyectoAprobado Como Logico
	
	// Definición de Constantes
	Definir JORNADA_DIARIA, DIAS_SEMANA Como Entero
	JORNADA_DIARIA <- 8
	DIAS_SEMANA <- 5
	
	// Entrada de datos
	Escribir "Ingrese el nombre del proyecto:"
	Leer nombreProyecto
	
	Escribir "Ingrese las horas totales de desarrollo estimadas:"
	Leer horasDesarrollo
	
	Escribir "Ingrese el costo por hora:"
	Leer costoHora
	
	Escribir "Ingrese el presupuesto máximo del cliente:"
	Leer presupuestoCliente
	
	Escribir "Ingrese el plazo máximo tolerado por el cliente (días):"
	Leer plazoClienteDias
	
	// 1. Cálculos Financieros
	subtotal <- horasDesarrollo * costoHora
	imprevistos <- subtotal * 0.12
	descuento <- subtotal * 0.05
	costoTotalNeto <- subtotal + imprevistos - descuento
	impuestoIVA <- costoTotalNeto * 0.16
	granTotal <- costoTotalNeto + impuestoIVA
	
	// 2. Cálculos de Tiempo
	diasTotales <- TRUNC(horasDesarrollo / JORNADA_DIARIA)
	horasSobrantes <- horasDesarrollo Mod JORNADA_DIARIA
	semanasLaborales <- TRUNC(diasTotales / DIAS_SEMANA)
	
	// 3. Evaluaciones Booleanas
	presupuestoViable <- (granTotal <= presupuestoCliente)
	plazoViable <- (diasTotales <= plazoClienteDias)
	proyectoAprobado <- presupuestoViable Y plazoViable
	
	// Salida de resultados
	Escribir "----------------------------------------"
	Escribir "   INFORME INTEGRADOR DE PROYECTO       "
	Escribir "----------------------------------------"
	Escribir "Proyecto: ", nombreProyecto
	Escribir "Subtotal Mano de Obra : $", subtotal
	Escribir "Gastos e Imprevistos  : $", imprevistos
	Escribir "Descuento por Convenio: $", descuento
	Escribir "Costo Total Neto      : $", costoTotalNeto
	Escribir "Impuesto IVA (16%)    : $", impuestoIVA
	Escribir "Gran Total a Cobrar   : $", granTotal
	Escribir "----------------------------------------"
	Escribir "Días Totales Estimados: ", diasTotales
	Escribir "Horas Sobrantes       : ", horasSobrantes
	Escribir "Semanas Laborales     : ", semanasLaborales
	Escribir "----------------------------------------"
	Escribir "Presupuesto Viable    : ", presupuestoViable
	Escribir "Plazo Viable          : ", plazoViable
	Escribir "PROYECTO APROBADO     : ", proyectoAprobado
	Escribir "----------------------------------------"
FinAlgoritmo