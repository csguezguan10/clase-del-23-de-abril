# clase-del-23-de-abril
Quanser matlab
# Plataforma Quanser

Quanser es una plataforma educativa y de investigación especializada en sistemas de control, robótica y mecatrónica. Se utiliza en universidades y laboratorios para simular y experimentar con sistemas reales mediante hardware y software integrados.

## Características clave
- **Laboratorios virtuales y físicos**: Permite practicar con sistemas como robots, drones o control de motores.
- **Entorno en tiempo real**: Ideal para probar algoritmos de control (PID, automatización, etc.).
- **Aplicaciones**: Desde docencia hasta prototipado industrial.

## Primeros pasos

Primero iniciamos el entorno de Quanser en MATLAB ejecutando las siguientes funciones:

- **1. QLabs.setup**
Función: Configura el entorno de trabajo en QLabs, inicializando los componentes esenciales para su operación.
Detalle:

Establece conexiones con dispositivos y servidores.

Carga bibliotecas y parámetros de configuración inicial.

Prepara el sistema para la ejecución de experimentos.

**2. QLabs.register**
Función: Registra entidades en el sistema QLabs para su identificación y gestión.
Aplicaciones típicas:

Autenticación de usuarios o dispositivos.

Configuración de perfiles de experimentos.

Asignación de recursos específicos.

**3. QLabs.launch**
Función: Inicia procesos dentro del entorno QLabs.
Operaciones posibles:

Ejecución de simulaciones o experimentos.

Lanzamiento de interfaces gráficas.

Puesta en marcha de procesos en segundo plano.

**Nota técnica:**
Esta secuencia de comandos (setup → register → launch) sigue el flujo estándar de inicialización de sistemas, donde primero se prepara el entorno, luego se autentican los componentes, y finalmente se ejecutan las operaciones principales. La implementación específica puede variar según la versión de QLabs y los módulos instalados.

## Menú principal de QLabs
Este es el menú principal de QLabs, una plataforma de laboratorios virtuales de Quanser que permite realizar experimentos de control y robótica de forma interactiva. A continuación, se detallan sus componentes:

Opciones de Experimentos Disponibles
Qube 2 - DC Motor

Enfoque: Control clásico de motores.

Aplicación: Ideal para aprender fundamentos de sistemas de control (ej. PID) usando un motor de corriente continua (DC) con retroalimentación de posición/velocidad.

Aero

Enfoque: Sistemas aerospaciales no lineales.

Aplicación: Simula el control de plataformas acopladas dinámicamente (como drones o helicópteros), donde se estudia estabilidad y control avanzado.

Ball and Beam

Enfoque: Dinámica no lineal y control en tiempo real.

Aplicación: Experimentos con una viga y bola, donde se controla la posición de la bola mediante sensores y actuadores.

Qube-Servo 2: Plataforma Principal
El Qube-Servo 2 ha sido seleccionado como plataforma principal para nuestro proyecto debido a su implementación en el laboratorio de control de la universidad y sus capacidades integrales para el estudio de sistemas dinámicos.

**Características Principales
Componentes principales:**

Motor DC con encoder de alta precisión.

Disco de inercia ajustable para modificar la dinámica del sistema.

Tarjeta de adquisición de datos integrada.

**Parámetros clave:**

Voltaje nominal: 12V.

Rango de velocidad: 0–3000 RPM.

Resolución del encoder: 2048 pulsos por revolución.

 **Software compatible:**
 

MATLAB/Simulink (via QUARC).

LabVIEW.

Python (con librerías de Quanser).

**Diferencias entre Qube-Servo 2 y Qube 3**

Aunque inicialmente planeábamos trabajar con el Qube-Servo 2 (basado en las simulaciones disponibles en QLabs), el equipo físico disponible en el laboratorio de la universidad es el Qube 3. Afortunadamente, las diferencias entre ambos modelos no son significativas, lo que permite adaptar nuestro proyecto sin mayores complicaciones.

Nota: El Qube 3 ofrece mayor precisión y opciones de conectividad, pero conserva la misma filosofía de diseño y compatibilidad con los mismos conceptos de control.

**Integración con Simulink (MATLAB)**

El Quanser Qube-Servo 2 y otros sistemas de Quanser están diseñados para funcionar de manera óptima con Simulink (MATLAB), lo que permite implementar, simular y validar algoritmos de control en un entorno académico profesional.

Ejemplo 1: Control en Cascada
El diagrama muestra un sistema de control en cascada diseñado para que la velocidad de un motor siga una referencia de 1000 unidades. El sistema compara la velocidad deseada con la real y genera un error que pasa a un controlador PI, el cual calcula la corriente necesaria para alcanzar la velocidad objetivo.

**Resultado:**La gráfica muestra que la respuesta del sistema (línea azul) sigue correctamente a la referencia (línea amarilla), confirmando que el controlador funciona adecuadamente.

**Ejemplo 2:** Control de Posición con PI Digital
El diagrama muestra un sistema de control en lazo cerrado para el QUBE-Servo 2 implementado en Simulink, donde se regula la posición del motor utilizando un controlador PI digital.

## Características:

Uso de Hardware-in-the-Loop (HIL).

Medición de corriente, velocidad y posición en tiempo real.

Visualización del comportamiento del sistema.

## Figuras de Referencia

**Fig. 10:** Datos del Qube-Servo 2.

**Fig. 11:** Tabla de datos del Qube-Servo 3.

**Fig. 7:** Montaje de comprobación.

**Fig. 8:** Curva de reacción de corriente.

**Fig. 9:** Curva de reacción de velocidad.

**Fig. 13** Configuración del QUBE-SERVO.

**Fig. 14:** Tiempo de muestreo.

**Fig. 21:** Montaje prueba relé por velocidad.
