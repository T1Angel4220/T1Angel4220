# Diseño del perfil

El [README.md](../README.md) muestra el perfil únicamente en inglés. [README.en.md](../README.en.md) conserva una copia inglesa compatible con enlaces anteriores. La versión española completa está preservada en [README.es.md](../README.es.md), sin selectores ni enlaces visibles desde el perfil principal. Los recursos españoles también se conservan. El diseño actual es `v3`, con una cabecera integrada en azul oscuro.

Vistas previas: [escritorio](./previews/perfil-escritorio.png) · [móvil](./previews/perfil-movil.png). Se generan localmente desde el README con Mistune y una hoja de estilos que aproxima GitHub. Las capturas muestran el estado final del banner animado; el SVG original conserva el movimiento.

## Composición

1. Habitación animada, nombre, disponibilidad y terminal en inglés.
2. Portafolio, CV en español, contacto y navegación interna.
3. Gestión de Eventos, Gestión Hospitalaria, Sistema de Ventas y LUPSI ChatOps, enlazados a los repositorios originales.
4. Bloque principal de ocho herramientas Full Stack y catálogo completo de 53 tecnologías en ocho categorías: backend y APIs, interfaces web, datos, IA y visión, nube, herramientas y calidad, móvil y escritorio. Se distingue uso principal de conocimientos según las capturas del usuario.
5. Actividad pública automática.
6. Presentación personal con tarjetas de gatos y rock.
7. Contacto mediante `ayuquinaangel4220@gmail.com`, LinkedIn y acceso al CV original en PDF, identificado como español.

El párrafo adicional de LUPSI y la lista de proyectos complementarios se retiraron por petición del usuario. LUPSI permanece como uno de los cuatro proyectos destacados. También se retiró la tarjeta de League of Legends y se redistribuyeron las dos tarjetas de intereses restantes.

## Cabecera y terminal

Los archivos `assets/v3/es/hero.svg`, `hero-mobile.svg` y sus equivalentes ingleses combinan la ilustración y la presentación. El README selecciona la versión móvil mediante `picture`.

La terminal muestra:

- `T1Angel4220: ~/perfil` en español y `T1Angel4220: ~/profile` en inglés.
- `whoami` en inglés: Angel Ayuquina - Software Engineering Student, para coincidir con el CV. La versión móvil abrevia el título. La versión española archivada conserva su texto original.
- Presentación profesional: Full Stack Developer.
- `cat focus.txt`: Full Stack, con interfaces web, APIs, bases de datos y despliegue. La versión móvil usa una frase más corta.
- Disponibilidad para roles junior en full stack.

Las máscaras del efecto de escritura están ajustadas a las nuevas cadenas. Se verificó que las frases completas caben en la terminal en ambos tamaños e idiomas.

## Recursos y movimiento

`assets/v3/` contiene las cabeceras, el stack con iconos, los botones, la presentación personal y el cierre. Las secciones inglesas disponen de variantes móviles para mantener la legibilidad. Las animaciones CSS incluyen reglas de movimiento reducido.

Las tecnologías y niveles de uso proceden de las capturas aportadas el 17 de noviembre de 2026. El [catálogo](./technology-usage.md) documenta los 53 elementos, la distinción de uso y la procedencia de los iconos. Los logotipos se incrustan en los SVG; no se utilizan iniciales genéricas para sustituir marcas disponibles.

Las tarjetas de proyectos conservan un ancho de 420 píxeles: se distribuyen en dos columnas cuando hay espacio y se apilan en pantallas estrechas. Las imágenes de los proyectos y sus procedencias se documentan en [tecnologías y capturas](./tecnologias-y-capturas.md) y en el [análisis de AgenteTelegram](./analisis-agente-telegram.md).

Las tarjetas inglesas explican el propósito del sistema y la contribución personal, inferida a partir de cambios de código atribuidos a `T1Angel4220` en el historial público:

- Eventos: [API de inscripciones](https://github.com/T1Angel4220/eventconnect/commit/e2378f2467) e [integración del dashboard](https://github.com/T1Angel4220/eventconnect/commit/140240a03e).
- Hospitalaria: [gestión de pacientes](https://github.com/T1Angel4220/AD-GestionHospitalaria/commit/91dcc7e7d4), [calendario](https://github.com/T1Angel4220/AD-GestionHospitalaria/commit/3de19187f0) y [selección de bases distribuidas](https://github.com/T1Angel4220/AD-GestionHospitalaria/commit/6d6a567e66).
- Ventas: [APIs, imágenes y ubicaciones](https://github.com/T1Angel4220/SistemaVentas/commit/617377be4f) y [búsqueda de ubicación en la interfaz](https://github.com/T1Angel4220/SistemaVentas/commit/fd0f6bcd49). Su tarjeta utiliza la captura de inicio existente, sin crear sesiones ni datos.
- AgenteTelegram: [flujos del bot y PDFs](https://github.com/T1Angel4220/AgenteTelegram/commit/2ec01e13e3) e [integraciones y orquestación](https://github.com/T1Angel4220/AgenteTelegram/commit/9051517406).

Estos resúmenes no atribuyen la totalidad de los proyectos en equipo a una sola persona. Esta revisión no modifica ni audita la documentación de los repositorios destacados.

Los recursos originales del banner y las versiones anteriores se conservan. La carpeta de referencia `perfil-v2/` permanece local y no se incluye en esta publicación. El README no requiere paquetes npm.

## Actividad e idioma

El [workflow de contribuciones](../.github/workflows/contributions.yml) publica los SVG de actividad en la rama `output` a las 00:17 de Ecuador continental, con opción de ejecución manual. Las acciones están fijadas a commits; los resultados incluyen una regla de movimiento reducido y variantes para temas claro y oscuro.

El perfil principal no muestra un selector de idioma ni un bloque desplegable. La versión española se conserva en `README.es.md` y puede abrirse directamente desde los archivos del repositorio; queda fuera de la presentación principal, según la preferencia del usuario.

El botón de portafolio apunta a [angel-portafolio-eight.vercel.app](https://angel-portafolio-eight.vercel.app/).

Referencia: [renderizado de Markdown de GitHub](https://github.com/github/markup#github-markup).
