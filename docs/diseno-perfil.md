# Diseño del perfil

Los archivos [README.md](../README.md) y [README.en.md](../README.en.md) presentan las mismas secciones en español e inglés. La composición adapta la propuesta `perfil-v2/` que proporcionó el usuario.

Vistas previas: [escritorio](./previews/perfil-escritorio.png) · [móvil](./previews/perfil-movil.png). Se generan a partir del HTML del renderizador de GitHub y una hoja de estilos de aproximación; GitHub determina el ancho, el tema y la tipografía finales.

## Composición actual

1. Idioma y habitación ilustrada animada.
2. Presentación gráfica con nombre, especialidad, disponibilidad y ventana de código.
3. Estudios, ubicación, portafolio, contacto y navegación interna.
4. EventConnect, HospitalApp, Sistema de Ventas y LUPSI ChatOps, enlazados al código.
5. Stack con chips de tecnologías por categorías e integraciones de IA.
6. Actividad pública automática, intereses y contacto.

El [análisis de AgenteTelegram](./analisis-agente-telegram.md) explica la sustitución de Mantenimiento y qué capacidades respalda el código.

## Recursos gráficos

- `assets/v2/es/` y `assets/v2/en/`: adaptación bilingüe del diseño de referencia.
- `assets/v2/shared/`: separador compartido.
- `assets/projects/`: tarjetas de los proyectos.
- `assets/screens/`: capturas de aplicaciones y vista de Telegram proveniente de su repositorio.
- `assets/profile-header.png`: imagen original, conservada como alternativa estática.
- `assets/profile-header.svg`: SVG original del usuario, conservado como fuente.
- `assets/banner-animado.svg`: versión animada del banner.

La carpeta `perfil-v2/` y el archivo RAR originales se conservan como materiales del usuario y no se publican con estos cambios.

## Adaptación móvil y movimiento

La introducción, los títulos, el stack, los intereses y el cierre tienen variantes móviles seleccionadas mediante `picture`. El texto se vuelve a componer y los grupos se apilan en lugar de reducir una lámina de escritorio completa.

Los proyectos usan tarjetas de 420 píxeles de ancho: dos columnas cuando hay espacio y una columna en pantallas estrechas. Las cuatro tarjetas comparten proporciones. Las tecnologías mantienen Angular expresamente asociado a cursos y práctica personal.

Las animaciones nuevas de la introducción se implementan con CSS. El README selecciona además variantes estáticas explícitas de la presentación cuando se solicita `prefers-reduced-motion`. Las animaciones SMIL del ejemplo se retiraron durante la adaptación. El banner conserva sus movimientos de gatos, colas, luces y reflejos; el README selecciona su PNG original cuando se solicita movimiento reducido.

Los SVG no usan scripts ni descargas externas. Los recursos informativos incluyen textos alternativos y las secciones conservan encabezados HTML y navegación mediante anclas.

## Procedencia de las vistas

Las capturas de EventConnect, HospitalApp y Sistema de Ventas se obtuvieron ejecutando sus frontends públicos localmente, sin iniciar sesión ni modificar sus interfaces. La tarjeta de LUPSI usa una vista incluida por el autor en AgenteTelegram y la identifica de esa manera; no se afirma haber validado una sesión real del bot.

Los commits y el alcance de las capturas anteriores se documentan en [tecnologías y capturas](./tecnologias-y-capturas.md). Las imágenes de Mantenimiento se conservan como material de esa revisión, aunque el proyecto deja de estar destacado.

## Actividad y publicación

El [workflow de contribuciones](../.github/workflows/contributions.yml) publica los SVG de actividad en la rama `output` a las 00:17 de Ecuador continental, con opción de ejecución manual. Las acciones están fijadas a commits y los resultados incluyen una regla de movimiento reducido. El README selecciona el gráfico claro u oscuro mediante `prefers-color-scheme`.

El selector de idioma enlaza los dos documentos; no detecta automáticamente el idioma del navegador. No se necesitan paquetes npm para mostrar el perfil.

Referencia: [renderizado de Markdown de GitHub](https://github.com/github/markup#github-markup).
