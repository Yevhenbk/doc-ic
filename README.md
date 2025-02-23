# DOC Ingeneria de Computadores I

# Tema 1

## 1. Arquitectura de Von Neumann
Un computador basado en esta arquitectura consta de los siguientes componentes principales:
- **Unidad de Memoria (UM):** Almacena datos e instrucciones.
- **Unidad Central de Proceso (CPU):** Contiene la **Unidad de Control (UC)** e **Unidad Aritmético-Lógica (ALU)**.
- **Periféricos de Entrada/Salida (E/S):** Comunicación con el exterior.
- **Bus:** Medio de comunicación entre los diferentes componentes.

## 2. Unidad Central de Proceso (CPU)
La CPU ejecuta instrucciones mediante las siguientes unidades:
- **Unidad de Control (UC):** Interpreta y controla la ejecución de instrucciones.
- **Unidad Aritmético-Lógica (ALU):** Realiza operaciones matemáticas y lógicas.
- **Registros internos:** Almacenan datos temporales.
- **Ciclo de instrucción:** Secuencia de pasos para ejecutar una instrucción.

## 3. Ciclo de Instrucción
El ciclo de instrucción consta de varias fases:

1. **Búsqueda de la instrucción (BI)**  
   - Se obtiene la instrucción desde la memoria principal.
   
2. **Decodificación de la instrucción (DI)**  
   - Se interpreta el tipo de operación a realizar.

3. **Cálculo de la dirección del operando (CDO)**  
   - Se determina la dirección del dato en memoria o en E/S.

4. **Búsqueda del operando (BO)**  
   - Se obtiene el operando necesario para la operación.

5. **Ejecución de la operación (OD)**  
   - Se ejecuta la operación en la ALU.

6. **Almacenamiento del resultado (AO)**  
   - Se guarda el resultado en memoria o en un registro.

**Nota:** Las CPU modernas pueden manejar instrucciones que requieren múltiples operandos o hacer más de una referencia a memoria.

## 4. Diagramas y Ejemplo del Ciclo de Instrucción
El ciclo de instrucción se puede representar mediante diagramas de flujo y diagramas de estado.

**Ejemplo de fases en ejecución:**
- **Fase de búsqueda:** El contador de programa (PC) envía la dirección a la memoria.
- **Fase de decodificación:** Se interpreta la instrucción almacenada en el registro de instrucciones (IR).
- **Fase de ejecución:** Se realizan las operaciones requeridas y se almacenan los resultados.

## Comparación con Conocimientos Previos
- Se mantiene la estructura tradicional de la arquitectura Von Neumann.
- El ciclo de instrucción es detallado con cada fase bien explicada.
- La presencia de operandos múltiples y la relación entre registros internos y memoria refuerza conceptos clave en arquitectura de computadoras y sistemas operativos.

## Conclusión y Recomendaciones de Estudio
- **Comprender bien el ciclo de instrucción** y su flujo de ejecución.
- **Revisar la arquitectura de Von Neumann**, especialmente el uso de memoria compartida entre instrucciones y datos.
- **Practicar con diagramas de estado y flujo** para visualizar la ejecución de instrucciones.
- **Relacionar estos conceptos con sistemas operativos** y cómo se gestionan los procesos en hardware real.

---
