# A1.3 · Análisis de limitaciones de un dispositivo

## Dispositivo analizado

**Modelo:** HONOR Magic7 Lite

## 1. Especificaciones

| Característica | Especificación                                                                                   |
|---|--------------------------------------------------------------------------------------------------|
| **Procesador** | Qualcomm Snapdragon 6 Gen 1, CPU de 8 núcleos: 4× Cortex-A78 a 2,2 GHz + 4× Cortex-A55 a 1,8 GHz |
| **GPU** | Adreno A710                                                                                      |
| **Memoria RAM** | 8 GB                                                                                             |
| **Almacenamiento interno** | 256 GB, dependiendo de la versión del dispositivo                                                |
| **Almacenamiento libre actual** | **187,34 GB**                                                                                    |
| **Pantalla** | AMOLED de 6,78 pulgadas                                                                          |
| **Resolución** | 2700 × 1224 píxeles                                                                              |
| **Densidad aproximada** | 437 píxeles por pulgada (ppi)                                                                    |
| **Frecuencia de actualización** | Hasta 120 Hz                                                                                     |
| **Sistema de fábrica** | MagicOS 8.0 basado en Android 14                                                                 |
| **Versión de Android instalada actualmente** | **16 GB**                                                                                        |
| **Nivel de API** | **36**                                                                                           |

## 2. Sensores disponibles

HONOR Magic7 Lite dispone de los siguientes sensores y sistemas relacionados:

- Sensor de gravedad.
- Giroscopio.
- Brújula.
- Sensor de luz ambiental.
- Sensor de proximidad.
- Sensor de huellas dactilares.
- NFC.
- GPS y otros sistemas de posicionamiento: A-GPS, GLONASS, BeiDou y Galileo.

## 3. Batería y consumo

El HONOR Magic7 Lite cuenta con una batería de **6600 mAh de capacidad típica** y admite carga rápida HONOR SuperCharge de 66 W.

### Estado actual de la batería

**Nivel de batería en el momento del análisis:** 49 %

**Estado de la batería:** En buen estado

### Consumo por aplicaciones

| Aplicación       | Consumo |
|------------------|--------:|
| **WhatsApp**     |    46 % |
| **Chrome**       |    17 % |
| **Inicio Honor** |    12 % |

## 4. Conclusiones de diseño para la futura aplicación

### Conclusión 1 · Evitar procesos multimedia demasiado pesados

El HONOR Magic7 Lite dispone de un **Snapdragon 6 Gen 1 y 8 GB de RAM**. Es un hardware suficiente para una aplicación de calistenia con imágenes, animaciones y vídeos, pero no es necesario realizar procesamiento multimedia pesado en el propio dispositivo.

Por ello, la aplicación debería utilizar contenido multimedia optimizado, evitando vídeos de resolución excesivamente alta o tareas como edición y procesamiento de vídeo en tiempo real.

Esto permitiría que la aplicación funcionase de forma fluida no solamente en este teléfono, sino también en dispositivos Android menos potentes.

### Conclusión 2 · La localización debe utilizarse solamente cuando sea necesaria

El teléfono dispone de **GPS, A-GPS, GLONASS, BeiDou y Galileo**, por lo que puede obtener su ubicación para la futura funcionalidad de encontrar parques de calistenia cercanos.

Sin embargo, mantener la localización activa continuamente aumentaría innecesariamente el consumo de batería.

Por ello, la aplicación solicitará la ubicación principalmente cuando el usuario acceda a la sección de **parques cercanos**, en lugar de mantener el GPS funcionando permanentemente en segundo plano.

### Conclusión 3 · La interfaz debe adaptarse a diferentes pantallas

El dispositivo analizado tiene una pantalla relativamente grande, de **6,78 pulgadas, resolución 2700 × 1224 y aproximadamente 437 ppi**.

La aplicación podría aprovechar esta pantalla para mostrar imágenes de los ejercicios, explicaciones y progresiones de forma cómoda. Sin embargo, no se deben diseñar los elementos utilizando tamaños o posiciones fijas pensando únicamente en esta pantalla.

La interfaz se desarrollará de manera adaptable para que botones, textos, imágenes y listas continúen siendo utilizables en teléfonos Android con pantallas más pequeñas o con resoluciones y densidades diferentes.

## Conclusión

El HONOR Magic7 Lite dispone de potencia, memoria, pantalla y sensores suficientes para desarrollar y probar la aplicación de calistenia planteada para el proyecto.

Sus sistemas de localización permiten implementar la búsqueda de parques cercanos, mientras que el giroscopio y el sensor de gravedad podrían permitir estudiar en el futuro otras funcionalidades relacionadas con el movimiento.

Aun así, el diseño de la aplicación no debe depender únicamente de las características de este dispositivo. Se deberá controlar el consumo de recursos, utilizar la localización solamente cuando sea necesaria y crear una interfaz adaptable a dispositivos Android con características diferentes.