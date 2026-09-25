## Práctica 02: Conversor de Almacenamiento Digital para Centro de Cómputo

### 1. Planteamiento del Problema
Un administrador de servidores recibe solicitudes de capacidad en Gigabytes (GB) pero sus herramientas de monitoreo de disco duro reportan en Megabytes (MB), Terabytes (TB) y Kilobytes (KB).

### 2. Tabla Entrada-Proceso-Salida

| Entradas | Procesos / Fórmulas | Salidas |
| :--- | :--- | :--- |
| `capacidadGB` (Real) | `capacidadMB = capacidadGB * 1024`<br>`capacidadKB = capacidadMB * 1024`<br>`capacidadTB = capacidadGB / 1024` | Resultados en KB, MB y TB (`capacidadKB`, `capacidadMB`, `capacidadTB`). |

### 3. Algoritmo en Lenguaje Natural
1. Inicio del algoritmo.
2. Solicitar al usuario el valor de almacenamiento expresado en `capacidadGB`.
3. Multiplicar `capacidadGB` por 1024 para calcular `capacidadMB`.
4. Multiplicar `capacidadMB` por 1024 para calcular `capacidadKB`.
5. Dividir `capacidadGB` entre 1024 para calcular `capacidadTB`.
6. Mostrar los resultados de las conversiones en KB, MB y TB.
7. Fin del algoritmo.