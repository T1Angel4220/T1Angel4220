# Diseño del perfil

El [README.md](../README.md) muestra el perfil únicamente en inglés. [README.en.md](../README.en.md) conserva una copia inglesa compatible con enlaces anteriores. La versión española completa está preservada en [README.es.md](../README.es.md), sin selectores ni enlaces visibles desde el perfil principal. Los recursos españoles también se conservan. El diseño actual es `v3`, con una cabecera integrada en azul oscuro.

Vistas previas: [escritorio](./previews/perfil-escritorio.png) · [móvil](./previews/perfil-movil.png). Se generan a partir del HTML del renderizador de GitHub y una hoja de estilos de aproximación.

## Composición

1. Habitación animada, nombre, disponibilidad y terminal en inglés.
2. Portafolio, contacto y navegación interna.
3. Gestión de Eventos, Gestión Hospitalaria, Sistema de Ventas y LUPSI ChatOps, enlazados a los repositorios originales.
4. Stack de 53 tecnologías en ocho categorías: backend y APIs, interfaces web, datos, IA y visión, nube, herramientas y calidad, móvil y escritorio. Se distingue uso principal de conocimientos según las capturas del usuario.
5. Actividad pública automática.
6. Presentación personal con tarjetas de gatos y rock.
7. Contacto mediante `ayuquinaangel4220@gmail.com`.

El párrafo adicional de LUPSI y la lista de proyectos complementarios se retiraron por petición del usuario. LUPSI permanece como uno de los cuatro proyectos destacados. También se retiró la tarjeta de League of Legends y se redistribuyeron las dos tarjetas de intereses restantes.

## Cabecera y terminal

Los archivos `assets/v3/es/hero.svg`, `hero-mobile.svg` y sus equivalentes ingleses combinan la ilustración y la presentación. El README selecciona la versión móvil mediante `picture`.

La terminal muestra:

- `T1Angel4220: ~/perfil` en español y `T1Angel4220: ~/profile` en inglés.
- `whoami`: Angel Ayuquina - Ingeniero en Software / Software Engineer, según la petición del usuario.
- Presentación profesional: Full Stack Developer.
- `cat focus.txt`: Full Stack, con interfaces web, APIs, bases de datos y despliegue. La versión móvil usa una frase más corta.
- Disponibilidad para roles junior en full stack.

Las máscaras del efecto de escritura están ajustadas a las nuevas cadenas. Se verificó que las frases completas caben en la terminal en ambos tamaños e idiomas.

## Recursos y movimiento

`assets/v3/` contiene las cabeceras, el stack con iconos, los botones, la presentación personal y el cierre. El stack también dispone de una variante móvil. Las animaciones CSS incluyen reglas de movimiento reducido.

Las tecnologías y niveles de uso proceden de las capturas aportadas el 17 de noviembre de 2026. El [catálogo](./technology-usage.md) documenta los 53 elementos, la distinción de uso y la procedencia de los iconos. Los logotipos se incrustan en los SVG; no se utilizan iniciales genéricas para sustituir marcas disponibles.

Las tarjetas de proyectos conservan un ancho de 420 píxeles: se distribuyen en dos columnas cuando hay espacio y se apilan en pantallas estrechas. Las imágenes de los proyectos y sus procedencias se documentan en [tecnologías y capturas](./tecnologias-y-capturas.md) y en el [análisis de AgenteTelegram](./analisis-agente-telegram.md).

Los recursos originales del banner y las versiones anteriores se conservan. La carpeta de referencia `perfil-v2/` permanece local y no se incluye en esta publicación. El README no requiere paquetes npm.

## Actividad e idioma

El [workflow de contribuciones](../.github/workflows/contributions.yml) publica los SVG de actividad en la rama `output` a las 00:17 de Ecuador continental, con opción de ejecución manual. Las acciones están fijadas a commits; los resultados incluyen una regla de movimiento reducido y variantes para temas claro y oscuro.

El perfil principal no muestra un selector de idioma ni un bloque desplegable. La versión española se conserva en `README.es.md` y puede abrirse directamente desde los archivos del repositorio; queda fuera de la presentación principal, según la preferencia del usuario.

El botón de portafolio apunta a [angel-portafolio-eight.vercel.app](https://angel-portafolio-eight.vercel.app/).

Referencia: [renderizado de Markdown de GitHub](https://github.com/github/markup#github-markup).
