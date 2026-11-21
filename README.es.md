<p align="center">
  <img src="docs/icon.png" width="96" alt="Icono de la app Exployer">
</p>

<h1 align="center">Exployer — gestor de archivos, descargador de videos, navegador y editor de fotos para Android</h1>

<p align="center">
  <b>Un APK gratuito en lugar de cinco aplicaciones.</b><br>
  Gestor de archivos con papelera y etiquetas · reproductor de música y video con reproducción inteligente
  de carpetas · navegador con bloqueador de anuncios · descargador de videos HLS/DASH · editor de fotos y
  videos · lector de ZIP · bóveda AES-256
</p>

<p align="center">
  <a href="https://github.com/balochscript/Exployer-App/releases/latest"><img alt="Última versión" src="https://img.shields.io/github/v/release/balochscript/Exployer-App?label=APK&color=22c55e"></a>
  <img alt="Android 8.0+" src="https://img.shields.io/badge/Android-8.0%2B-3ddc84">
  <img alt="Gratis" src="https://img.shields.io/badge/price-free-blue">
  <img alt="Tamaño" src="https://img.shields.io/badge/size-9.1%20MB-lightgrey">
</p>

<p align="center">
  <a href="https://github.com/balochscript/Exployer-App/releases/latest/download/exployer-0.9.103.apk"><b>⬇ Descargar el APK (9,1 MB)</b></a>
  ·
  <a href="docs/FEATURES.md">Todas las funciones</a>
  ·
  <a href="CHANGELOG.md">Changelog</a>
  ·
  <a href="FAQ.md">Preguntas frecuentes</a>
  ·
  <a href="#verificar">Verificar el hash</a>
</p>

<p align="center">
  <b>Leelo en:</b>
  <a href="README.md">English</a> ·
  <a href="README.fa.md">فارسی</a> ·
  <a href="README.es.md">Español</a> ·
  <a href="README.pt-BR.md">Português (BR)</a> ·
  <a href="README.id.md">Bahasa Indonesia</a> ·
  <a href="README.hi.md">हिन्दी</a> ·
  <a href="README.ar.md">العربية</a> ·
  <a href="README.ur.md">اردو</a>
</p>

---

## Dos compilaciones, las mismas funciones

| Archivo | Tamaño | Cuándo usarlo |
|---|---|---|
| `exployer-0.9.103.apk` | **9,1 MB** | Elección normal. Reducido y optimizado con R8; funciones y comportamiento idénticos. |
| `exployer-0.9.103-nor8.apk` | **18,0 MB** | Solo como respaldo. El mismo código sin minificación R8 — úsalo si la compilación pequeña fallara en un dispositivo poco común. |

Ambos archivos están firmados con la misma clave y pueden actualizarse entre sí. Ambos son versionCode **113**.

---

## Capturas de pantalla

| | | | |
|---|---|---|---|
| <img src="docs/screenshots/en/01-file-manager.jpg" width="210" alt="Inicio del gestor de archivos — tarjeta de almacenamiento, ocho categorías, tres herramientas, multiselección"> | <img src="docs/screenshots/en/02-folder-play.jpg" width="210" alt="Menú de reproducción de carpeta con nueve órdenes, filtros de tipo y continuar la reproducción anterior"> | <img src="docs/screenshots/en/03-video-player.jpg" width="210" alt="Reproductor de video con brillo, volumen, velocidad y búsqueda bajo el dedo"> | <img src="docs/screenshots/en/04-music.jpg" width="210" alt="Biblioteca de música, cola y ecualizador integrado"> |
| **Gestor de archivos** | **Reproducir una carpeta** | **Reproductor de video** | **Reproductor de música** |
| <img src="docs/screenshots/en/05-tags.jpg" width="210" alt="Etiquetas — etiquetar, colorear, reproducir; etiquetado rápido mientras navegas; reproducción multi-etiqueta"> | <img src="docs/screenshots/en/06-browser.jpg" width="210" alt="Navegador — menú de herramientas, grupos de pestañas y bóveda de contraseñas"> | <img src="docs/screenshots/en/07-downloads.jpg" width="210" alt="Descargas — lista y filtros, diálogo de programación, ajustes y errores honestos"> | |
| **Etiquetas** | **Navegador** | **Descargas** | |

Las siete son 1080 × 1920 y también existen en persa — el conjunto en persa es el que aparece en el
listado de Cafe Bazaar de la app. Cómo se construyen y qué afirman los textos se explica en
[docs/screenshots/README.md](docs/screenshots/README.md).

---

## ¿Qué es Exployer?

Exployer es una sola aplicación de Android que cubre las tareas cotidianas para las que la gente suele
instalar cinco aplicaciones. Está pensada para teléfonos sin cuenta de Google Play, sin root y sin
registro: instalas el APK, concedes una vez el permiso "Acceso a todos los archivos" y todo funciona
en el dispositivo.

No hay nube, ni subidas, ni telemetría. Los archivos, el historial de reproducción, las etiquetas y la
bóveda nunca salen del teléfono.

## Funciones

El catálogo completo, con los detalles de cada punto, está en [docs/FEATURES.md](docs/FEATURES.md).
Esta es la lista completa — las funciones grandes y las pequeñas.

### Gestor de archivos
- Almacenamiento interno y tarjeta SD, vistas de lista y cuadrícula, ruta de migas de pan tocable para
  saltar a cualquier carpeta
- Ordenar por nombre, fecha, tamaño o tipo, en ambas direcciones; búsqueda global en todo el almacenamiento
- Selección simple, múltiple y por rango ("del primero al último"); copiar, mover, eliminar, renombrar,
  compartir, propiedades
- Hoja de copiar/mover con su propia ruta, crear carpeta, archivos ocultos
- Ocho categorías — audio, video, imágenes, documentos, descargas, APKs, archivos, todos los archivos — más una tarjeta de
  almacenamiento en vivo (usado / libre / total) en la pantalla de inicio
- Archivos recientes (últimos cinco días) con filtro de tipo, abrir-carpeta-contenedora y propiedades;
  avisa honestamente cuando el almacenamiento era demasiado grande para escanearlo completo
- Comprimir a ZIP, cifrar a `.enx`, descifrar e instalar un APK desde la misma lista
- Visor integrado de PDF y de texto, para que un documento nunca tenga que salir de la app
- Papelera: los archivos eliminados se pueden recuperar hasta 30 días, con cuenta regresiva
- Análisis de almacenamiento: carpetas y archivos más grandes, divididos por tipo (incluye torrents);
  buscador de duplicados que mueve las copias sobrantes a la papelera

### Etiquetas
- Etiqueta cualquier archivo en el momento en que lo ves — desde la lista de archivos (pulsación larga →
  seleccionar → botón de etiqueta en la barra de selección), desde Now Playing o desde el visor de
  fotos/videos. No hay límite de etiquetas por archivo
- Etiquetado masivo: selecciona muchos archivos y aplica una etiqueta en una acción; el selector muestra
  "3 de 5" cuando solo parte de la selección ya la tiene, y las fichas muestran todo / algo / nada
- Diez colores, asignados automáticamente; crear (también desde el selector), renombrar, eliminar —
  eliminar una etiqueta nunca borra archivos, el diálogo lo dice
- Los nombres de etiqueta duplicados se rechazan (los caracteres árabe/persa parecidos se normalizan antes)
- Buscar dentro de la lista de etiquetas; cinco órdenes: más elementos, menos elementos, más nueva,
  más antigua, etiquetadas recientemente
- Reproducir una etiqueta entera: solo su música o todos sus medios, con los mismos nueve órdenes y la
  misma reanudación
- **MultiTagPlay**: mantén pulsadas varias etiquetas y reproduce todo su contenido como una sola cola;
  un archivo que pertenece a dos etiquetas seleccionadas se reproduce una sola vez; "continuar la
  reproducción anterior" y "seleccionar todo" respetan la búsqueda actual de etiquetas

### Música y video
- Biblioteca con actualización silenciosa, cola, "añadir a la cola", velocidad de reproducción
  (0,25×–3,0×), temporizador de sueño con tiempo restante, repetir apagado / todo / uno, aleatorio
- Ecualizador con preajustes, refuerzo de graves y virtualizador, más un reinicio; mini reproductor
  siempre visible
- Reproducción en segundo plano con controles de notificación; las notificaciones siguen el idioma de la app
- Reproducir una carpeta completa (subcarpetas incluidas, hasta 24 niveles y 20.000 archivos — y lo dice
  si un límite realmente se alcanza) en nueve órdenes: nombre A→Z, nombre Z→A, fecha más nueva, fecha más
  antigua, tamaño mayor, tamaño menor, menos reproducidos, más reproducidos, totalmente aleatorio
- Fichas de filtro por tipo (música / video / imágenes) con conteos, cambiables antes de pulsar reproducir
- "Continuar la reproducción anterior": la cola, el orden, el filtro de tipo y el elemento actual se
  guardan por carpeta, archivo, etiqueta y conjunto multi-etiqueta — el menú ofrece
  "continuar en 7 de 42 · menos reproducidos"
- Una reproducción cuenta solo tras 10 segundos o 25 % de progreso, así "menos reproducidos" significa algo real
- Reproductor de video: arrastre horizontal para buscar, arrastre vertical para volumen y brillo, rango de
  búsqueda por deslizamiento 0,5–20 %, doble toque para pausar/reproducir, mantener para 2×, bloqueo táctil,
  relación de aspecto (ajustar / recortar / estirar), selección de pista de audio y subtítulos, pantalla
  completa sin barras del sistema, rotación manual, picture-in-picture, captura de pantalla con un toque,
  comportamiento al final del video (repetir / detener / siguiente), medios acompañantes, recortar y
  recortar-longitud desde el propio reproductor

### Navegador (Baloch Core)
- El renderizado lo hace el WebView Chromium del sistema; pestañas, bloqueo, privacidad y estadísticas
  son código propio de Exployer
- Pestañas, vistas previas de pestañas, grupos de pestañas con ocho colores — arrastra la tarjeta de una
  pestaña a la ficha del grupo, con deshacer; cerrar un grupo deja sus pestañas abiertas y recuperables
  durante 24 horas
- Pestañas de incógnito (no se guarda nada), pestañas cerradas recuperables durante 24 horas,
  restauración de sesión con la posición exacta del scroll
- Barra de pestañas en cinco posiciones (arriba, abajo, izquierda, derecha, oculta); pestañas de solo
  favicon; barra inferior opcional
- Bloqueo de anuncios con una lista curada de dominios más ocultación de espacios publicitarios; el
  ahorro de datos retiene imágenes y videos pesados hasta que toques "Cargar todo" (desactivado por defecto)
- Interruptor opcional Do Not Track / Sec-GPC (desactivado por defecto); borrar historial, caché y
  cookies al salir
- Página de inicio con accesos directos editables, patrón de buscador personalizado, buscar en la página,
  zoom por sitio recordable, modo escritorio, tamaño de texto predeterminado, indicador HTTPS/HTTP
- Marcadores, historial, estadísticas del navegador (visitas y descargas totales y semanales, sitios más
  visitados)
- Permiso de cámara, micrófono y ubicación por sitio (preguntar / permitir / denegar) con pantalla de gestión
- Sniffer de medios: una burbuja flotante arrastrable o un icono en la barra de direcciones lista todos los
  videos y audios de la página actual con su tamaño exacto — por página, así que la siguiente página nunca
  mezcla streams antiguos; renombra antes de descargar, copia el enlace directo, vuelve a escanear

### Descargas
- Cola con porcentaje, velocidad, tamaño, tiempo restante y posición en la cola; de 1 a 15 archivos a la
  vez, o ilimitados
- Reanuda desde el byte exacto (petición Range, no un reinicio)
- De 3 a 30 reintentos automáticos (o ilimitados) con un retraso personalizado opcional; una política de
  parada decide si el motor sigue intentando, se detiene en el primer error o se detiene en una fecha límite
- Descargas programadas: fecha, hora, número de reintentos, retraso, política de parada y fecha límite;
  las programaciones sobreviven a que maten la app y a reinicios
- Detección de "ya descargado" y "ya en la cola"; verificación real del checksum del archivo terminado
- Mensajes de error honestos: protegido por DRM, 403/404, una página HTML en lugar de un archivo
  (anti-leech), red, almacenamiento lleno, fallo de conversión, fecha límite alcanzada — cada uno con el
  siguiente paso a dar
- Soporte de HLS (M3U8) y DASH, un respaldo de captura, carpeta de descargas personalizada
  (por defecto `Downloads/Exployer`)
- Pausar o reanudar todo a la vez, pausar/iniciar/reintentar/abrir/compartir/eliminar por elemento,
  selección por lotes, limpiar la lista de terminados, pestañas Todo / Activo / Programado,
  ordenar por progreso, velocidad o estado
- Notificaciones de descarga con progreso y controles mientras la app está cerrada

### Editor de fotos y videos
- Recorte libre con el tamaño de píxel de salida mostrado, rotar
- Ocho deslizadores de luz y color: exposición, contraste, luces, sombras, saturación, viveza,
  temperatura, tinte
- Curva tonal con puntos libres, más curvas prehechas; seis filtros
- Pincel de reparación con tamaño ajustable y deshacer del último trazo; corrección de perspectiva
  arrastrando cuatro esquinas
- Deshacer y rehacer; borrador automático para que salir del editor no pierda el trabajo
- Tres destinos de guardado: junto al original, `Download/Exployer/Edit`, o reemplazar el original (la
  copia anterior va a la papelera)
- Editor de video: recortar, recortar-bordes, rotar, unir clips con normalización de dimensiones,
  exportación en segundo plano con notificación de progreso — cierra el editor y el archivo se sigue creando

### ZIP, cifrado, privacidad
- Navegar un archivo ZIP como una carpeta sin extraer; extraer la carpeta actual o un solo archivo con
  progreso por bytes; pegar archivos dentro del ZIP; protección Zip-Slip; apertura rápida de ZIP muy
  grandes; reproducir los medios dentro del ZIP con los mismos nueve órdenes (pregunta antes de extraer)
- Cifrado `.enx`: AES-256-GCM por bloques con clave derivada por PBKDF2, más un contenedor de carpeta
  cifrada que se abre y navega como una carpeta normal tras una contraseña; los archivos antiguos `.enc`
  siguen abriéndose
- Bóveda de contraseñas: una contraseña maestra que estableces una vez, entradas con sitio / usuario /
  contraseña / nota, bloqueo instantáneo, cambio de contraseña maestra; la contraseña maestra nunca se almacena

### Apariencia, idioma y anuncios
- Tema del sistema / claro / oscuro, cinco paletas de color de acento
- Ocho idiomas: persa, inglés, español, portugués de Brasil, indonesio, hindi, árabe, urdu — independientes
  del idioma del teléfono, aplicados también a las notificaciones; diseño completo de derecha a izquierda
- Gratis y sostenido con anuncios (Tapsell): un video con recompensa completo apaga los anuncios 24 horas,
  cinco videos dentro de esas 24 horas los apagan una semana; el contador avisa antes de reiniciarse

## Instalación

1. Descarga `exployer-0.9.103.apk` (9,1 MB) desde el panel de [Releases](https://github.com/balochscript/Exployer-App/releases/latest).
2. Ábrelo en el teléfono. Si Android lo pide, permite instalar desde esta fuente (tu navegador o gestor de archivos).
3. Abre Exployer y concede **Acceso a todos los archivos** — es el permiso que necesita un gestor de archivos.
4. Opcional: permite "instalar apps desconocidas" solo si quieres instalar APKs desde dentro de la app.

Exployer 0.9.103 · versionCode 113 · paquete `com.balochscript.exployer` · Android 8.0 (API 26)+ ·
targetSdk 36 · 9,1 MB (compilación R8) o 18,0 MB (sin R8)

## Verificar

Compara el SHA-256 del archivo descargado con el valor de abajo. Cada versión está firmada con la misma
clave, así que un archivo alterado también sería rechazado por Android al actualizar.

```
SHA-256 (exployer-0.9.103.apk)       6bd897b87cb9cabc527c4fe6d5295fe086303bfd5d2d684d1d4e334f1779e7ca
SHA-256 (exployer-0.9.103-nor8.apk)  d53f6480bc5516123b94c595f80244a0eece17fb84816edc35c15e80ed38436d
```

```bash
# Windows
certutil -hashfile exployer-0.9.103.apk SHA256
# Linux / macOS
shasum -a 256 exployer-0.9.103.apk
# Android (Termux)
sha256sum exployer-0.9.103.apk
```

## Lo que no hace

Dicho claramente, para que nadie descargue por la razón equivocada:

- No puede descargar streams protegidos por DRM, ni evita inicios de sesión ni muros de pago
- No puede abrir archivos ZIP protegidos con contraseña
- No tiene sincronización en la nube, ni cuenta, ni copia de seguridad entre dispositivos
- El bloqueo de anuncios es una lista curada de dominios, no un motor de suscripciones estilo uBlock

## Preguntas frecuentes

Respuestas cortas aquí, las largas en [FAQ.md](FAQ.md).

- **¿De verdad es gratis?** Sí. Sin cuenta, sin suscripción; la app se sostiene con anuncios, y los videos
  con recompensa los apagan — uno por 24 horas, cinco dentro de esas 24 horas por una semana.
- **¿Necesita root?** No. Usa el permiso estándar de acceso a todos los archivos.
- **¿Funciona sin conexión?** El gestor de archivos, los reproductores, el editor, el ZIP y la bóveda sí.
  Solo el navegador y el descargador necesitan red.
- **¿Qué versiones de Android?** 8.0 y superiores, incluidos los permisos de medios de Android 13–16.
- **¿Por qué dos APK?** Uno está optimizado con R8 (9,1 MB), el otro es el mismo código sin reducir (18,0 MB).

## Privacidad

Sin cuenta, sin SDK de analítica, sin subidas. La cámara, el micrófono y la ubicación solo se exponen a un
sitio que tú abriste y solo tras aprobarlo. Detalles en [PRIVACY.md](PRIVACY.md).

## Changelog

Cada versión y qué cambió, incluida la lista completa 0.9.91 → 0.9.103: [CHANGELOG.md](CHANGELOG.md)

## Soporte

- Errores y sugerencias: [abre un issue](https://github.com/balochscript/Exployer-App/issues)
- Email: balochscriptcom@gmail.com
- Sitio web: [balochscript.com](https://balochscript.com)

<sub>Exployer está hecho por Baloch Script. Android es una marca comercial de Google LLC. Este proyecto no está afiliado a Google.</sub>
