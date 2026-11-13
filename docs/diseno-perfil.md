# Diseño del perfil

Los archivos [README.md](../README.md) y [README.en.md](../README.en.md) comparten estructura y recursos equivalentes en español e inglés. La versión actual publica el diseño `v3` preparado por el usuario, con una cabecera integrada en azul oscuro.

Vistas previas: [escritorio](./previews/perfil-escritorio.png) · [móvil](./previews/perfil-movil.png). Se generan a partir del HTML del renderizador de GitHub y una hoja de estilos de aproximación.

## Composición

1. Selector de idioma, habitación animada, nombre, disponibilidad y terminal.
2. Portafolio, contacto y navegación interna.
3. Gestión de Eventos, Gestión Hospitalaria, Sistema de Ventas y LUPSI ChatOps, enlazados a los repositorios originales.
4. Stack por categorías: frontend, backend, móvil, datos, despliegue e integraciones de IA.
5. Actividad pública automática.
6. Presentación personal con tarjetas de gatos y rock.
7. Contacto mediante `ayuquinaangel4220@gmail.com`.

El párrafo adicional de LUPSI y la lista de proyectos complementarios se retiraron por petición del usuario. LUPSI permanece como uno de los cuatro proyectos destacados. También se retiró la tarjeta de League of Legends y se redistribuyeron las dos tarjetas de intereses restantes.

## Cabecera y terminal

Los archivos `assets/v3/es/hero.svg`, `hero-mobile.svg` y sus equivalentes ingleses combinan la ilustración y la presentación. El README selecciona la versión móvil mediante `picture`.

La terminal muestra:

- `T1Angel4220: ~/perfil` en español y `T1Angel4220: ~/profile` en inglés.
- `whoami`: Angel Ayuquina - Ingeniero en Software / Software Engineer, según la petición del usuario.
- `cat focus.txt`: Frontend + Full Stack, con React, TypeScript, APIs y datos. La versión móvil usa una frase más corta.
- Disponibilidad para roles junior en frontend o full stack.

Las máscaras del efecto de escritura están ajustadas a las nuevas cadenas. Se verificó que las frases completas caben en la terminal en ambos tamaños e idiomas.

## Recursos y movimiento

`assets/v3/` contiene las cabeceras, el stack con iconos, los botones, la presentación personal y el cierre. El stack también dispone de una variante móvil. Las animaciones CSS incluyen reglas de movimiento reducido.

Las tarjetas de proyectos conservan un ancho de 420 píxeles: se distribuyen en dos columnas cuando hay espacio y se apilan en pantallas estrechas. Las imágenes de los proyectos y sus procedencias se documentan en [tecnologías y capturas](./tecnologias-y-capturas.md) y en el [análisis de AgenteTelegram](./analisis-agente-telegram.md).

Los recursos originales del banner y las versiones anteriores se conservan. La carpeta de referencia `perfil-v2/` permanece local y no se incluye en esta publicación. El README no requiere paquetes npm.

## Actividad e idioma

El [workflow de contribuciones](../.github/workflows/contributions.yml) publica los SVG de actividad en la rama `output` a las 00:17 de Ecuador continental, con opción de ejecución manual. Las acciones están fijadas a commits; los resultados incluyen una regla de movimiento reducido y variantes para temas claro y oscuro.

El selector de idioma enlaza `README.md` y `README.en.md`. Cada botón abre la versión completa del idioma elegido en GitHub. No hay un bloque de inglés al final del documento ni desplazamiento entre traducciones. GitHub no permite reemplazar dinámicamente el README del perfil: cada idioma se presenta como un archivo separado.

El botón de portafolio apunta a [angel-portafolio-eight.vercel.app](https://angel-portafolio-eight.vercel.app/).

Referencia: [renderizado de Markdown de GitHub](https://github.com/github/markup#github-markup).
