# Diseño del README del perfil

Los archivos [README.md](../README.md) y [README.en.md](../README.en.md) comparten estructura y recursos. El selector de idioma enlaza ambos documentos. La presentación está orientada a oportunidades junior de Frontend / Full Stack y conserva los intereses personales del autor.

Vistas previas: [escritorio](./previews/perfil-escritorio.png) · [móvil](./previews/perfil-movil.png). Se generan a partir del HTML del renderizador de Markdown de GitHub y una hoja de estilos de aproximación. GitHub determina el fondo, la tipografía y el ancho final de su interfaz.

## Composición

1. Selector de idioma, habitación animada, nombre, especialidad y disponibilidad.
2. Accesos al portafolio y al correo, y navegación interna.
3. Tres tarjetas de capacidades: componentes, interfaces e integración.
4. Cuatro proyectos enlazados; los dos primeros muestran interfaces reales.
5. Stack frontend e información ampliable de backend y otros proyectos.
6. Actividad pública de GitHub con una animación de contribuciones.
7. Gatos, rock y League of Legends, bienvenida con efecto de escritura y contacto.

## Banner y movimiento

- [Imagen original](../assets/profile-header.png): se conserva sin modificar y funciona como alternativa estática.
- [SVG original del usuario](../assets/profile-header.svg): se conserva como fuente editable.
- [Banner animado](../assets/banner-animado.svg): variante del SVG con movimientos más suaves y protección adicional para movimiento reducido.

La ilustración está incrustada en el SVG; no requiere una descarga externa. Las máscaras y animaciones CSS dan movimiento a la respiración y las colas de los gatos, las luces, los reflejos y otros detalles de la habitación. No se utilizan scripts dentro del SVG. Se comprobó que la animación cambia entre fotogramas al cargarla mediante un elemento `img` normal.

El elemento `picture` de ambos README selecciona explícitamente el PNG cuando el navegador indica `prefers-reduced-motion: reduce`. Las animaciones de los demás SVG incluyen reglas para detenerse con esta preferencia. La bienvenida se mantiene fuera del encabezado para distribuir el movimiento entre secciones.

## Capturas reales de proyectos

Las primeras dos tarjetas incluyen capturas de los frontends públicos ejecutados localmente. Son las pantallas de acceso: no implican una prueba completa del backend ni del producto. No se iniciaron sesiones ni se modificaron las interfaces para producir las capturas.

| Proyecto | Fuente capturada | Pantalla |
| --- | --- | --- |
| EventConnect | `develop`, commit `4694884334b3ee9f36c4c2168f29f12036f4609c` | Acceso en temas claro y oscuro, mediante el selector nativo de la aplicación. |
| HospitalApp | `release/1.0.0`, commit `c1814be5c695bdf94913033bb142c71044b56b90` | Acceso de la aplicación. Las credenciales de demostración visibles pertenecen a su interfaz pública. |

Las imágenes completas están en [assets/screens](../assets/screens). Las tarjetas de EventConnect alternan las capturas de sus dos temas con una transición CSS. Las tarjetas de Sistema de Ventas y Mantenimiento conservan sus portadas ilustradas; no se presentan como capturas.

## Recursos y adaptación

- `assets/features/`: tres capacidades con variantes en español e inglés.
- `assets/projects/`: cuatro tarjetas por idioma.
- `assets/icons/`: iconos de tecnologías.
- `assets/ui/`: botones, separador y bienvenida.
- `assets/interests/`: distintivos de gatos, rock y League of Legends.

Las capacidades tienen un ancho de presentación de 280 píxeles; las tarjetas de proyectos, de 420. Se distribuyen en filas cuando hay espacio y se apilan en pantallas estrechas. Las imágenes usan el estilo `max-width: 100%` de GitHub. Los fondos azules oscuros se mantienen legibles con temas claros y oscuros. Cada recurso informativo incluye texto alternativo en el idioma correspondiente.

Los SVG utilizan tipografías del sistema y recursos incrustados. Se editan sin instalar React ni paquetes npm: el README se presenta mediante Markdown y HTML admitidos por GitHub. Al cambiar un proyecto, deben actualizarse las dos versiones de su tarjeta, los enlaces y los textos alternativos.

## Actividad automática

El [workflow de contribuciones](../.github/workflows/contributions.yml) genera dos SVG con la actividad pública real de la cuenta y los publica en la rama `output`. Se ejecuta diariamente a las 00:17 de Ecuador continental, permite ejecución manual y vuelve a ejecutarse al cambiar el propio workflow en `main`.

Las acciones externas están fijadas a commits. El único permiso de escritura es el necesario para publicar los SVG en este repositorio. Se añade a los resultados una regla de movimiento reducido. El README elige la variante clara u oscura mediante `prefers-color-scheme`.

Referencia: [renderizado de Markdown de GitHub](https://github.com/github/markup#github-markup).
