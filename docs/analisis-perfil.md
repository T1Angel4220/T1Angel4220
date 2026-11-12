# Análisis del perfil de GitHub de Angel Ayuquina

Revisión realizada el **12 de noviembre de 2026** sobre los **19 repositorios públicos** de [T1Angel4220](https://github.com/T1Angel4220).

Se revisaron los metadatos, los árboles de archivos de las ramas predeterminadas, los README y manifiestos disponibles, y archivos de código representativos. Esta revisión sirve para seleccionar y presentar proyectos; no incluye ejecutar las aplicaciones, certificar su funcionamiento ni una auditoría exhaustiva de cada archivo o del historial de Git.

## Posicionamiento recomendado

**Desarrollador frontend con React y TypeScript, con experiencia práctica en proyectos full stack.**

React y TypeScript aparecen en varias aplicaciones con formularios, autenticación, roles, paneles y consumo de APIs. Node.js, Express, Laravel, PostgreSQL y MySQL respaldan la orientación full stack. Los proyectos móviles, Java y Python complementan esa presentación.

El README anterior destacaba Java, Python, PHP y MySQL, pero no mostraba React, TypeScript ni las aplicaciones web recientes. La nueva presentación pone esas evidencias al principio y conserva una breve nota personal.

## Revisión de los 19 repositorios

La prioridad indica su utilidad para la presentación profesional buscada, no una calificación de calidad. Las tecnologías se identificaron en documentación, dependencias y código; no se dedujeron solamente del lenguaje que muestra GitHub.

| Repositorio | Evidencia encontrada | Uso recomendado |
| :--- | :--- | :--- |
| [eventconnect](https://github.com/T1Angel4220/eventconnect) | React, TypeScript, Tailwind, Express y PostgreSQL; eventos, inscripciones, roles y reportes. | Proyecto principal para frontend y full stack. |
| [AD-GestionHospitalaria](https://github.com/T1Angel4220/AD-GestionHospitalaria) | React, TypeScript, Zustand, Express, MySQL y Docker; pacientes, consultas, calendarios y reportes. | Destacar interfaces administrativas e integración de servicios. |
| [SistemaVentas](https://github.com/T1Angel4220/SistemaVentas) | React, TypeScript, Tailwind, Express y PostgreSQL; catálogo, publicaciones, usuarios y moderación. | Mostrar navegación, filtros y flujos de un marketplace. |
| [Sistema_Mantenimiento](https://github.com/T1Angel4220/Sistema_Mantenimiento) | Frontend React, principalmente JSX, y backend Laravel; equipos, mantenimientos y reportes PDF. | Mostrar una segunda combinación de frontend y backend. |
| [eventconnect-movil](https://github.com/T1Angel4220/eventconnect-movil) | React Native, Expo, TypeScript, Axios y Expo Router; eventos, inscripciones y tema claro/oscuro. | Complementar EventConnect con el cliente móvil. |
| [AgenteTelegram](https://github.com/T1Angel4220/AgenteTelegram) | NestJS, TypeScript, Telegraf y Supabase; servicios de integración con GitHub y Trello. | Complemento para candidaturas full stack e integración de APIs. |
| [Combustible-SKT](https://github.com/T1Angel4220/Combustible-SKT) | Java, Spring Boot, gRPC, MongoDB, PostgreSQL y Docker; servicios y API Gateway para control de combustible. | Alternativa para vacantes que pidan Java o backend. |
| [Mensajes_VideoLlamada](https://github.com/T1Angel4220/Mensajes_VideoLlamada) | Python, Flask, JavaScript y WebRTC; chat, llamadas, separación por módulos y archivos de pruebas. | Complemento para explicar comunicación web y diseño de servicios. |
| [CalculadoraAproximacion](https://github.com/T1Angel4220/CalculadoraAproximacion) | Python, PySide6, NumPy y Matplotlib; regresión lineal/cuadrática, separación de capas y pruebas. | Evidencia adicional de arquitectura, lógica y trabajo con interfaces. |
| [Plataforma-UTA](https://github.com/T1Angel4220/Plataforma-UTA) | PHP, MySQL, HTML, CSS y JavaScript; formularios de acceso, sesiones e integraciones de autenticación. | Proyecto previo para explicar fundamentos web. |
| [Pagina-Web-Votos](https://github.com/T1Angel4220/Pagina-Web-Votos) | PHP y MySQL con un servicio Express/Nodemailer; páginas de candidatos, votación y resultados. | Proyecto previo de interfaz web y persistencia. |
| [Pagina-Blog](https://github.com/T1Angel4220/Pagina-Blog) | PHP y MySQL con PDO; publicaciones, categorías, comentarios y administración. | Ejemplo de CRUD y modelado de una aplicación de contenidos. |
| [Tamagochi-en-Python](https://github.com/T1Angel4220/Tamagochi-en-Python) | HTML, CSS y JavaScript con estado en localStorage, más una implementación Python orientada a objetos. | Buen complemento para explicar JavaScript sin frameworks e interacción. |
| [Juego-en-Java](https://github.com/T1Angel4220/Juego-en-Java) | Java Swing y clases para árboles y listas; juego del ahorcado. | Evidencia de programación orientada a objetos y estructuras de datos. |
| [KNN-IA](https://github.com/T1Angel4220/KNN-IA) | Python, NumPy, SciPy y Matplotlib; implementación de KNN para dígitos EMNIST. | Sección secundaria de algoritmos e inteligencia artificial. |
| [IA-EME](https://github.com/T1Angel4220/IA-EME) | Python, TensorFlow y Keras; red neuronal para clasificación de dígitos EMNIST. | Sección secundaria de aprendizaje automático. |
| [Captura](https://github.com/T1Angel4220/Captura) | Script Python con Tkinter, capturas de pantalla y peticiones HTTP; sin README ni manifiesto de dependencias. | Documentar propósito, instalación y demostración antes de destacarlo. |
| [T1Angel4220.github.io](https://github.com/T1Angel4220/T1Angel4220.github.io) | Portafolio HTML/CSS/JavaScript con Bootstrap. El sitio respondió HTTP 200 durante la revisión. | Actualizarlo con los proyectos recientes y una presentación bilingüe. |
| [T1Angel4220](https://github.com/T1Angel4220/T1Angel4220) | Repositorio del perfil; README e imágenes personales. | Punto de entrada profesional: presentación, proyectos y contacto. |

## Hallazgos que conviene atender

1. **Los 19 repositorios tienen vacíos los campos Description y Website en la API pública.** Añadir una descripción breve ayuda a entender cada proyecto desde la lista del perfil. El campo Website puede apuntar a una demostración cuando exista.
2. **El portafolio muestra cinco proyectos anteriores.** En [proyectos.html](https://github.com/T1Angel4220/T1Angel4220.github.io/blob/main/proyectos.html) aparecen Votos, Tamagotchi, Juego en Java, Plataforma UTA y Blog. Conviene incorporar las aplicaciones React y TypeScript que ahora encabezan el README.
3. **Hay páginas que concentran muchas responsabilidades.** [EventsManagement.tsx](https://github.com/T1Angel4220/eventconnect/blob/develop/frontend/src/pages/EventsManagement.tsx) tiene 3.404 líneas; [ReportesPage.tsx](https://github.com/T1Angel4220/AD-GestionHospitalaria/blob/release/1.0.0/hospital-app/frontend/vite-project/src/pages/ReportesPage.tsx), 902; y [la pantalla móvil de eventos](https://github.com/T1Angel4220/eventconnect-movil/blob/feat-notifications-client/app/%28tabs%29/index.tsx), 763. Separar filtros, formularios, listas y lógica de datos facilitaría explicar y mantener estas interfaces. El tamaño es una señal para revisar responsabilidades, no una prueba por sí sola de errores.
4. **Algunos README de subcarpetas conservan textos de plantilla.** Por ejemplo, [fronted/README.md](https://github.com/T1Angel4220/Sistema_Mantenimiento/blob/main/fronted/README.md) describe la plantilla React + Vite. Conviene reemplazarlo por instrucciones del proyecto y mantener coherencia con el README principal.
5. **La presentación debe distinguir proyectos de experiencia laboral.** El nuevo texto habla de aplicaciones académicas y personales. No atribuye años de experiencia, resultados comerciales, niveles de dominio, métricas de rendimiento ni autoría exclusiva que esta revisión no puede comprobar.

## Repositorios para fijar en el perfil

Orden sugerido según tu objetivo:

1. **eventconnect** — plataforma web con React y TypeScript.
2. **AD-GestionHospitalaria** — paneles, estado y backend con varios servicios.
3. **SistemaVentas** — catálogo, roles y moderación.
4. **Sistema_Mantenimiento** — React con Laravel.
5. **eventconnect-movil** — extensión móvil de un producto web.
6. **AgenteTelegram** — integraciones y servicios con NestJS.

Para una candidatura centrada en Java, sustituiría AgenteTelegram por Combustible-SKT. Para una centrada en fundamentos frontend, Tamagochi-en-Python permite explicar manejo del DOM y persistencia local.

## Descripciones listas para el campo About de GitHub

| Repositorio | Descripción sugerida |
| :--- | :--- |
| eventconnect | Plataforma de eventos e inscripciones con React, TypeScript, Express y PostgreSQL. |
| AD-GestionHospitalaria | Gestión hospitalaria con React, TypeScript, microservicios Express, MySQL y Docker. |
| SistemaVentas | Marketplace con catálogo, roles y moderación. React, TypeScript, Express y PostgreSQL. |
| Sistema_Mantenimiento | Gestión de equipos, mantenimientos y reportes PDF con React y Laravel. |
| eventconnect-movil | Cliente móvil de EventConnect con React Native, Expo y TypeScript. |
| AgenteTelegram | Bot de gestión de proyectos con NestJS, Telegram e integraciones con GitHub y Trello. |

Estas descripciones son propuestas; no se modificó la configuración de los repositorios remotos.

## Siguientes mejoras de mayor impacto

1. **Añadir una demostración visual a los cuatro proyectos principales:** captura de escritorio, vista móvil cuando corresponda y un recorrido corto de un flujo completo. Enlazar una demo pública si ya está disponible.
2. **Explicar tu participación:** si hubo equipo, indicar qué pantallas, servicios o decisiones desarrollaste tú. Describir un problema concreto, la solución y lo que aprendiste.
3. **Documentar cómo ejecutar cada aplicación:** requisitos, variables de ejemplo, instalación, datos de demostración y comandos reales. Publicar resultados de pruebas únicamente después de ejecutarlas.
4. **Actualizar el portafolio para que coincida con el perfil:** mismos proyectos principales, enlaces directos al código y texto en español e inglés.

## Archivos preparados en este repositorio

- [README.md](../README.md): presentación principal en español.
- [README.en.md](../README.en.md): versión equivalente en inglés.
- [assets/profile-header.png](../assets/profile-header.png): imagen adjunta elegida por el usuario, copiada sin cambios como cabecera. Ilustra una habitación de programación y rock con gatos, detalles de Viego y Teemo y un retrato de un gato alado.

El selector de idioma está al principio y al final de cada README. Cambia entre los dos archivos mediante enlaces; no detecta automáticamente el idioma del visitante. Al publicar los archivos juntos en este repositorio de perfil, las rutas relativas conservan la navegación y la imagen.
