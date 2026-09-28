# A1.1 · Estudio comparativo de tecnologías

Para comparar distintas formas de desarrollar una aplicación móvil se analizarán tres tecnologías de familias diferentes: **Android nativo, Flutter y PWA (Progressive Web App)**.

## Tabla comparativa

| Aspecto | Android nativo | Flutter | PWA |
|---|---|---|---|
| **Lenguaje** | Principalmente Kotlin. Java también es compatible. | Dart. | HTML, CSS y JavaScript. |
| **Herramientas** | Android Studio, Android SDK y emulador o dispositivo Android. | Flutter SDK, Dart y un editor como Android Studio o VS Code. | Editor de código y navegador web. Se utilizan además tecnologías como Web App Manifest y Service Workers. |
| **Plataformas** | Principalmente Android. | Android, iOS, web, Windows, macOS y Linux utilizando gran parte del mismo código. | Cualquier sistema que disponga de un navegador compatible, incluyendo Android, iOS y ordenadores. |
| **Rendimiento** | Muy alto, ya que la aplicación utiliza directamente las herramientas y APIs de Android. | Alto. Las aplicaciones se compilan para las plataformas de destino y ofrecen un rendimiento cercano al de una aplicación nativa. | Generalmente suficiente para aplicaciones sencillas, aunque depende del navegador y tiene más limitaciones para tareas exigentes. |
| **Acceso al hardware** | Acceso muy completo a las funciones del dispositivo: GPS, cámara, Bluetooth, sensores, almacenamiento, etc. | Puede acceder al hardware mediante los paquetes de Flutter o mediante código específico de cada plataforma cuando sea necesario. | Puede utilizar algunas funciones del dispositivo mediante APIs web, pero la disponibilidad depende del navegador y del sistema operativo. |
| **Coste de desarrollo** | Bajo si solamente se desarrolla para Android. Si también se necesita iOS habría que desarrollar otra versión de la aplicación. | Puede reducir el coste cuando se quiere desarrollar para Android e iOS porque gran parte del código es compartido. | Generalmente bajo, ya que una misma aplicación web puede funcionar en muchos dispositivos. |
| **Mantenimiento** | Sencillo si solo existe la versión Android. Mantener versiones nativas independientes para Android e iOS aumenta el trabajo. | Una única base de código permite realizar muchos cambios para varias plataformas al mismo tiempo. | Normalmente sencillo, porque las actualizaciones se realizan en el servidor web y los usuarios acceden a la nueva versión sin tener que actualizar manualmente la aplicación. |

Android recomienda actualmente **Kotlin para nuevos proyectos**, y Android Studio incluye soporte completo para este lenguaje.

Flutter permite crear aplicaciones para **Android, iOS, web y sistemas de escritorio desde una misma base de código**, aunque determinadas funciones pueden necesitar configuración o integración específica para cada plataforma.

Las PWA utilizan tecnologías web, pero pueden instalarse en el dispositivo, funcionar sin conexión mediante Service Workers y acceder a algunas características del sistema. Su grado de integración depende de las APIs que soporte cada navegador y plataforma.

## Casos de uso

### Android nativo

Sería especialmente adecuado para una aplicación cuyo objetivo principal sea **Android y que necesite utilizar intensivamente el hardware del teléfono**, por ejemplo una aplicación deportiva que utilice GPS, cámara, acelerómetro u otros sensores.

Al trabajar directamente con las APIs de Android se dispone de un gran control sobre las funciones del dispositivo.

Para el proyecto de calistenia que se desarrollará durante el curso, Android nativo resulta una opción apropiada porque la aplicación está destinada a Android y más adelante utilizará funciones del dispositivo, como la ubicación o algún sensor.

### Flutter

Sería especialmente adecuado para una empresa que quiera desarrollar una aplicación para **Android e iOS al mismo tiempo**, intentando reutilizar la mayor cantidad posible de código.

Por ejemplo, una aplicación de una tienda que necesite publicar una versión para ambos sistemas podría utilizar Flutter para evitar desarrollar dos aplicaciones completamente independientes.

### PWA

Sería especialmente adecuada para una aplicación relativamente sencilla que necesite llegar rápidamente a usuarios de **móviles y ordenadores sin obligarlos a instalar una aplicación desde una tienda**.

Por ejemplo, podría utilizarse para una aplicación de un restaurante en la que los usuarios consulten el menú, promociones y horarios desde cualquier dispositivo.

## Conclusión

Las tres tecnologías permiten crear aplicaciones accesibles desde dispositivos móviles, pero están orientadas a necesidades diferentes.

**Android nativo** ofrece una integración muy completa con el sistema Android y su hardware, aunque está centrado principalmente en esta plataforma.

**Flutter** permite reutilizar gran parte del código entre diferentes sistemas y resulta interesante cuando se quiere desarrollar para Android e iOS simultáneamente.

**PWA** permite desarrollar una aplicación utilizando tecnologías web y distribuirla fácilmente a muchos tipos de dispositivos, aunque puede disponer de menos acceso a determinadas características del hardware.

Para el proyecto de este curso utilizaría **Android nativo con Kotlin**, ya que el proyecto se desarrollará específicamente para Android y será necesario trabajar posteriormente con funciones propias del dispositivo, como localización, sensores y contenido multimedia.