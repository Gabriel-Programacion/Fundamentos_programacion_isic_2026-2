# Reporte de Reflexión y Autoevaluación

## 1. Retos y Dificultades Encontradas
El principal reto fue entender en qué se diferencia el ciclo `Repetir - Hasta Que` de la estructura `Mientras`[cite: 16, 18, 23]. Me costaba trabajo plantear la condición de salida al final, ya que no sabía si debía evaluar cuándo continuar dentro del menú o cuándo salirme por completo de la ejecución[cite: 18, 23].

## 2. Errores Cometidos durante la Depuración
El menú solo se mostraba una vez y se cerraba sin importar qué opción pusiera[cite: 18, 23]. El error estuvo en que escribí la condición al revés: puse `Hasta Que opcion != 0` cuando lo correcto para detener esta estructura en PSeInt/DFD es evaluar `Hasta Que opcion == 0`[cite: 18, 23].

## 3. Conclusión Técnica
Con esta práctica entendí la utilidad de las estructuras repetitivas post-prueba para crear menús interactivos[cite: 18, 23]. Su gran ventaja es que aseguran al menos una ejecución inicial del código antes de verificar si el usuario desea repetir la acción o salir del programa[cite: 18, 23].