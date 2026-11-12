# Diseño del README del perfil

Los archivos [README.md](../README.md) y [README.en.md](../README.en.md) comparten composición y recursos. El banner conserva exactamente la imagen que seleccionó el usuario.

Vistas previas: [escritorio](./previews/perfil-escritorio.png) · [móvil](./previews/perfil-movil.png). Se generaron con el HTML del renderizador de Markdown de GitHub y una hoja de estilos de vista previa. El tema que elija cada visitante en GitHub determina el fondo y la tipografía del documento.

## Estructura

1. Idioma, banner, nombre y orientación profesional.
2. Accesos al portafolio y al correo.
3. Cuatro proyectos enlazados, con tarjetas ilustradas en azul oscuro.
4. Tecnologías, con iconos y texto accesible.
5. Información ampliable de backend y proyectos complementarios.
6. Presentación personal y contacto.

## Recursos locales

- [assets/profile-header.png](../assets/profile-header.png): banner original del usuario.
- `assets/projects/`: tarjetas de proyectos, con versiones `-es.svg` y `-en.svg`.
- `assets/icons/`: iconos de las tecnologías del frontend.
- `assets/ui/`: botones de contacto, portafolio y separador.

Las tarjetas son portadas gráficas de los proyectos; no son capturas de sus aplicaciones. Cada una contiene un enlace al repositorio y una descripción alternativa en el idioma correspondiente.

Los SVG usan tipografías del sistema y no necesitan paquetes, scripts ni servicios externos de imágenes. Su texto, colores e iconos se pueden editar directamente en los archivos. Al cambiar un proyecto, hay que actualizar sus dos tarjetas y los enlaces y descripciones alternativas de ambos README.

## Presentación en GitHub

Las tarjetas usan imágenes de 420 píxeles de ancho: se presentan en dos columnas cuando hay espacio y pasan a una columna en pantallas estrechas. Los encabezados, descripciones y enlaces del resto del documento conservan el formato nativo de GitHub. Los fondos oscuros de los recursos gráficos permiten usarlos con temas claros y oscuros.

El bloque de backend usa el elemento nativo `details` para ampliar la información. El selector de idioma enlaza los dos archivos; no detecta el idioma del navegador.

Referencia técnica: [cómo renderiza GitHub los archivos Markdown](https://github.com/github/markup#github-markup).
