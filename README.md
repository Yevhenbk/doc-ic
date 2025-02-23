# DOC Ingeneria de Computadores I

# Tema 1: Parte 1

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

# Tema 1: Parte 2

## 1. Estructura del Bus
Los buses en un computador se organizan en grupos funcionales:
- **Líneas de datos:** Transportan la información entre los componentes.
- **Líneas de dirección:** Indican la ubicación de la memoria o dispositivo de E/S.
- **Líneas de control:** Gestionan la operación del bus, incluyendo:
  - Escritura y lectura de memoria.
  - Escritura y lectura de E/S.
  - Petición y autorización del bus.
  - Petición y reconocimiento de interrupción.

### **Anchura del Bus**
- La cantidad de datos transferidos a la vez depende de la anchura del bus.
- Un bus de 8 bits requiere dos accesos a la memoria para instrucciones de 16 bits.

## 2. Operación del Bus
El bus opera en dos direcciones principales:

### **Envío de datos:**
1. Obtener el uso del bus.
2. Transferir datos a través del bus.

### **Recepción de datos:**
1. Obtener el uso del bus.
2. Enviar una petición al otro módulo mediante líneas de dirección y control.
3. Esperar la respuesta con los datos.

## 3. Estructura Jerárquica del Bus
Cuando se incrementa el número de dispositivos conectados, el rendimiento del bus puede verse afectado debido a:
- Aumento del retardo de propagación.
- Posible congestión del bus debido a múltiples solicitudes simultáneas.

### **Soluciones:**
- Aumentar la velocidad y la anchura del bus.
- Implementar una **jerarquía de buses**:
  - **Bus de alto rendimiento:** Conecta dispositivos rápidos como memoria caché y procesadores.
  - **Bus de expansión:** Conecta dispositivos más lentos como almacenamiento y periféricos.

### **Ejemplo de jerarquía de buses:**
#### a) **Jerarquía de bus convencional**
- Bus del sistema.
- Bus de expansión.
- Bus local.

#### b) **Jerarquía de bus de alto rendimiento**
- Bus de alta velocidad.
- Bus de expansión.
- Bus local con conexiones a vídeo, LAN, y gráficos.

## 4. Tipos de Buses
Los buses pueden clasificarse en:
- **Dedicados:** Cada bus tiene una función específica (ejemplo: líneas separadas para datos y direcciones).
- **No dedicados:** Se utilizan para múltiples funciones mediante **multiplexación en el tiempo**.
  - Dirección y datos comparten el mismo bus.
  - Se usa una línea de control para indicar cuándo la dirección es válida.
  - Una vez identificada la dirección, se usa el bus para la transferencia de datos.

### **Ventajas y Desventajas de los Buses No Dedicados:**
✅ Menos líneas, menor costo y ahorro de espacio.  
❌ Circuitería más compleja y posible reducción del rendimiento.

## Conclusión y Recomendaciones de Estudio
- **Comprender bien la estructura del bus** y su impacto en el rendimiento.
- **Analizar la jerarquía de buses** y cómo mejora la comunicación entre dispositivos.
- **Estudiar los tipos de buses** y sus ventajas/desventajas.
- **Relacionar estos conceptos con el diseño de sistemas operativos** y hardware en arquitecturas modernas.

---

