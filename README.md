## APIs de Chrome utilizadas

### Interacción con el Navegador
- [chrome.tabs](https://developer.chrome.com/docs/extensions/reference/tabs/): Sistema completo para gestionar pestañas del navegador. Permite crear, modificar, mover y cerrar pestañas, además de acceder a su contenido y estado. Incluye funciones para capturar visualizaciones y manipular grupos de pestañas.
- [chrome.windows](https://developer.chrome.com/docs/extensions/reference/windows/): Control total sobre las ventanas del navegador. Permite crear ventanas con configuraciones específicas, gestionar su estado (maximizado, minimizado, pantalla completa), posición y tamaño. Soporta eventos para detectar cambios en las ventanas.
- [chrome.history](https://developer.chrome.com/docs/extensions/reference/history/): Acceso completo al historial de navegación. Permite buscar, añadir, eliminar y modificar entradas del historial. Incluye funciones para obtener las URLs más visitadas y gestionar las visitas por fecha y hora.
- [chrome.bookmarks](https://developer.chrome.com/docs/extensions/reference/bookmarks/): Gestión avanzada de marcadores. Permite crear, modificar y organizar marcadores y carpetas, realizar búsquedas, importar/exportar y sincronizar marcadores entre dispositivos.

### Comunicación y Runtime
- [chrome.runtime](https://developer.chrome.com/docs/extensions/reference/runtime/): Centro neurálgico de la extensión. Gestiona el ciclo de vida, la comunicación entre componentes, y proporciona información sobre el entorno de ejecución. Incluye:
  - Gestión de actualizaciones y eventos del navegador
  - Comunicación entre background scripts, content scripts y popups
  - Manejo de mensajes externos y conexiones nativas
  - Control de permisos y manifestación de la extensión
- [chrome.messaging](https://developer.chrome.com/docs/extensions/reference/messaging/): Sistema robusto de comunicación entre componentes. Soporta:
  - Mensajes síncronos y asíncronos
  - Comunicación entre extensiones diferentes
  - Canales de comunicación persistentes
  - Mensajería con aplicaciones nativas
- [chrome.webRequest](https://developer.chrome.com/docs/extensions/reference/webRequest/): Control granular sobre solicitudes de red. Permite:
  - Interceptar y modificar solicitudes y respuestas HTTP/HTTPS
  - Bloquear o redirigir solicitudes
  - Modificar encabezados y datos de la solicitud
  - Implementar reglas de seguridad y privacidad personalizadas

### Almacenamiento y Datos
- [chrome.storage](https://developer.chrome.com/docs/extensions/reference/storage/): Almacena y gestiona datos de la extensión.
- [chrome.cookies](https://developer.chrome.com/docs/extensions/reference/cookies/): Gestiona cookies del navegador.
- [chrome.downloads](https://developer.chrome.com/docs/extensions/reference/downloads/): Gestiona descargas de archivos.

### Manipulación de Contenido
- [chrome.scripting](https://developer.chrome.com/docs/extensions/reference/scripting/): Inyecta y ejecuta scripts en páginas web.
- [chrome.contentSettings](https://developer.chrome.com/docs/extensions/reference/contentSettings/): Control detallado sobre el comportamiento del contenido web:
  - Gestión de cookies y almacenamiento local
  - Control de JavaScript, plugins y popups
  - Configuración de cámaras y micrófonos
  - Gestión de notificaciones y ubicación
- [chrome.declarativeContent](https://developer.chrome.com/docs/extensions/reference/declarativeContent/): Define reglas para activar acciones en páginas web.

### Interfaz de Usuario
- [chrome.action](https://developer.chrome.com/docs/extensions/reference/action/): Gestiona el ícono y popup de la extensión.
- [chrome.contextMenus](https://developer.chrome.com/docs/extensions/reference/contextMenus/): Crea y gestiona menús contextuales.
- [chrome.notifications](https://developer.chrome.com/docs/extensions/reference/notifications/): Muestra notificaciones del sistema.

### Seguridad y Permisos
- [chrome.permissions](https://developer.chrome.com/docs/extensions/reference/permissions/): Sistema completo de gestión de permisos. Permite:
  - Solicitar y revocar permisos dinámicamente
  - Verificar permisos actuales
  - Implementar permisos opcionales para funcionalidades específicas
  - Gestionar permisos por host y API
- [chrome.privacy](https://developer.chrome.com/docs/extensions/reference/privacy/): Control avanzado de configuraciones de privacidad:
  - Gestión de servicios de red (predicción de red, protección contra phishing)
  - Control de características de privacidad del navegador
  - Configuración de políticas de seguridad
  - Gestión de certificados y autenticación

### Sistema y Dispositivo
- [chrome.system.cpu](https://developer.chrome.com/docs/extensions/reference/system_cpu/): Accede a información del CPU.
- [chrome.system.memory](https://developer.chrome.com/docs/extensions/reference/system_memory/): Accede a información de la memoria.
- [chrome.system.storage](https://developer.chrome.com/docs/extensions/reference/system_storage/): Accede a información del almacenamiento.

### Audio y Voz
- [chrome.audio](https://developer.chrome.com/docs/extensions/reference/audio/): Control completo sobre dispositivos y streams de audio, incluyendo entrada/salida y configuración.
- [chrome.tts](https://developer.chrome.com/docs/extensions/reference/tts/): Convierte texto a voz con amplio control sobre voces, idiomas y parámetros de síntesis.
- [chrome.ttsEngine](https://developer.chrome.com/docs/extensions/reference/ttsEngine/): Permite crear motores personalizados de texto a voz para extender las capacidades nativas.
- [Speech Recognition API](https://developer.mozilla.org/es/docs/Web/API/SpeechRecognition): Proporciona reconocimiento de voz en tiempo real con soporte para múltiples idiomas y gramáticas.
- [Speech Synthesis API](https://developer.mozilla.org/es/docs/Web/API/SpeechSynthesis): Genera voz sintética de alta calidad con control sobre propiedades como tono, velocidad y volumen.
- [Web Audio API](https://developer.mozilla.org/es/docs/Web/API/Web_Audio_API): Framework completo para procesamiento y síntesis de audio, incluyendo efectos, análisis y visualización.

### Multimedia y Dispositivos
- [chrome.desktopCapture](https://developer.chrome.com/docs/extensions/reference/desktopCapture/): Captura contenido de la pantalla.
- [chrome.mediaGalleries](https://developer.chrome.com/docs/extensions/reference/mediaGalleries/): Accede a galerías multimedia.
- [chrome.serial](https://developer.chrome.com/docs/extensions/reference/serial/): Comunica con dispositivos seriales.
- [chrome.usb](https://developer.chrome.com/docs/extensions/reference/usb/): Interactúa con dispositivos USB.
- [MediaDevices API](https://developer.mozilla.org/es/docs/Web/API/MediaDevices): Accede a micrófono, cámara y pantalla.
- [Media Capture and Streams API](https://developer.mozilla.org/es/docs/Web/API/Media_Streams_API): Graba y transmite audio/video.
- [Screen Capture API](https://developer.mozilla.org/es/docs/Web/API/Screen_Capture_API): Captura la pantalla del usuario.
- [Media Session API](https://developer.mozilla.org/es/docs/Web/API/Media_Session_API): Personaliza controles de reproducción.

### Interacción y Entrada
- [chrome.input.ime](https://developer.chrome.com/docs/extensions/reference/input_ime/): Implementa métodos de entrada personalizados.
- [chrome.commands](https://developer.chrome.com/docs/extensions/reference/commands/): Define y maneja atajos de teclado.
- [chrome.omnibox](https://developer.chrome.com/docs/extensions/reference/omnibox/): Integra funciones en la barra de direcciones.
- [Gamepad API](https://developer.mozilla.org/es/docs/Web/API/Gamepad_API): Permite usar controles de videojuegos.
- [Pointer Lock API](https://developer.mozilla.org/es/docs/Web/API/Pointer_Lock_API): Control absoluto del cursor.
- [Touch Events API](https://developer.mozilla.org/es/docs/Web/API/Touch_events): Maneja eventos táctiles.
- [Keyboard API](https://developer.mozilla.org/es/docs/Web/API/Keyboard_API): Detecta el estado de teclas físicas.

### Rendimiento y Optimizaciones
- [chrome.debugger](https://developer.chrome.com/docs/extensions/reference/debugger/): API de depuración de bajo nivel:
  - Control total sobre el depurador de Chrome
  - Inspección de estado de ejecución
  - Manipulación de puntos de interrupción
  - Acceso a la consola de depuración
- [chrome.processes](https://developer.chrome.com/docs/extensions/reference/processes/): Monitorea procesos del navegador.
- [chrome.performance](https://developer.chrome.com/docs/extensions/reference/performance/): Accede a métricas de rendimiento.
- [Performance API](https://developer.mozilla.org/es/docs/Web/API/Performance): Mide tiempos de carga y rendimiento.
- [WebAssembly](https://developer.mozilla.org/es/docs/WebAssembly): Ejecuta código C/C++ en el navegador.
- [Battery Status API](https://developer.mozilla.org/es/docs/Web/API/Battery_Status_API): Muestra nivel de batería.

### Red y Comunicación
- [chrome.proxy](https://developer.chrome.com/docs/extensions/reference/proxy/): Configura ajustes del proxy.
- [chrome.socket](https://developer.chrome.com/docs/extensions/reference/socket/): Implementa comunicaciones TCP/UDP.
- [chrome.webRTC](https://developer.chrome.com/docs/extensions/reference/webrtc/): Gestiona conexiones WebRTC.
- [chrome.networkingPrivate](https://developer.chrome.com/docs/extensions/reference/networkingPrivate/): Gestiona conexiones de red.
- [WebSockets API](https://developer.mozilla.org/es/docs/Web/API/WebSockets_API): Comunicación en tiempo real.
- [Fetch API](https://developer.mozilla.org/es/docs/Web/API/Fetch_API): Realiza peticiones HTTP modernas.
- [Broadcast Channel API](https://developer.mozilla.org/es/docs/Web/API/Broadcast_Channel_API): Comunicación entre pestañas.
- [Network Information API](https://developer.mozilla.org/es/docs/Web/API/Network_Information_API): Estado de la conexión.

### Almacenamiento y Archivos
- [chrome.fileSystem](https://developer.chrome.com/docs/extensions/reference/fileSystem/): Sistema completo para acceder y manipular archivos locales. Permite leer, escribir y gestionar archivos del sistema operativo de forma segura.
- [chrome.fileBrowserHandler](https://developer.chrome.com/docs/extensions/reference/fileBrowserHandler/): Extiende las capacidades del explorador de archivos nativo, permitiendo manejar tipos de archivos específicos y acciones personalizadas.
- [chrome.syncFileSystem](https://developer.chrome.com/docs/extensions/reference/syncFileSystem/): Proporciona sincronización automática de archivos con Google Drive, manteniendo los datos actualizados entre dispositivos.
- [File System Access API](https://developer.mozilla.org/es/docs/Web/API/File_System_Access_API): API moderna para interactuar directamente con el sistema de archivos local, permitiendo crear, modificar y eliminar archivos y directorios.
- [IndexedDB API](https://developer.mozilla.org/es/docs/Web/API/IndexedDB_API): Base de datos NoSQL de alto rendimiento para almacenar grandes cantidades de datos estructurados, incluyendo archivos y blobs.
- [LocalStorage & SessionStorage](https://developer.mozilla.org/es/docs/Web/API/Web_Storage_API): Mecanismos simples de almacenamiento clave-valor para datos persistentes (LocalStorage) o de sesión (SessionStorage).

### APIs Avanzadas y Experimentales
- [chrome.declarativeNetRequest](https://developer.chrome.com/docs/extensions/reference/declarativeNetRequest/): Permite bloquear o modificar solicitudes de red mediante reglas declarativas, ofreciendo mejor rendimiento que webRequest.
- [chrome.enterprise.deviceAttributes](https://developer.chrome.com/docs/extensions/reference/enterprise_deviceAttributes/): Proporciona información detallada sobre el dispositivo en entornos empresariales, incluyendo directivas y configuraciones.
- [chrome.enterprise.platformKeys](https://developer.chrome.com/docs/extensions/reference/enterprise_platformKeys/): Gestiona certificados y claves criptográficas a nivel empresarial para autenticación y firma digital.
- [chrome.gcm](https://developer.chrome.com/docs/extensions/reference/gcm/): Implementa Google Cloud Messaging para enviar y recibir mensajes push entre servidor y extensión.
- [Web Bluetooth API](https://developer.mozilla.org/es/docs/Web/API/Web_Bluetooth_API): Permite la conexión y comunicación con dispositivos Bluetooth Low Energy (BLE) desde el navegador.
- [WebGPU API](https://developer.mozilla.org/es/docs/Web/API/WebGPU_API): Nueva generación de gráficos 3D y computación en el navegador, sucesor de WebGL con mejor rendimiento.
- [WebHID API](https://developer.mozilla.org/es/docs/Web/API/WebHID_API): Proporciona acceso a dispositivos HID (Human Interface Device) como gamepads, teclados y dispositivos especializados.
- [Web Serial API](https://developer.mozilla.org/es/docs/Web/API/Serial): Establece conexiones serie bidireccionales con dispositivos hardware a través de puertos COM o USB.

### APIs de Desarrollo y Depuración
- [chrome.devtools](https://developer.chrome.com/docs/extensions/reference/devtools/): Herramientas avanzadas para desarrollo web:
  - Paneles personalizados en DevTools
  - Inspección y modificación del DOM en tiempo real
  - Análisis de red y recursos
  - Depuración de JavaScript y extensiones
