# Ampliación del stack y capturas

Revisión del **13 de noviembre de 2026** de los **19 repositorios públicos** de [T1Angel4220](https://github.com/T1Angel4220), complementaria al [análisis inicial](./analisis-perfil.md).

Se consultaron nuevamente los árboles de las ramas predeterminadas y 121 manifiestos, README y archivos de configuración. Se contrastaron las dependencias y la documentación; no se asignaron niveles de dominio ni se presentaron proyectos como experiencia laboral.

## Tecnologías representadas

| Área | Evidencia pública representativa |
| --- | --- |
| React, TypeScript, JavaScript, Tailwind CSS y Vite | [EventConnect: frontend/package.json](https://github.com/T1Angel4220/eventconnect/blob/4694884334b3ee9f36c4c2168f29f12036f4609c/frontend/package.json). |
| React Router, Zustand y Context API | Manifiestos y código de los frontends de HospitalApp, EventConnect y SistemaVentas. |
| Material UI, Radix UI, Framer Motion, React Hook Form, Zod y Recharts | [Mantenimiento: fronted/package.json](https://github.com/T1Angel4220/Sistema_Mantenimiento/blob/ce947d149b47abdb23c90e9aca29adc7a90c697a/fronted/package.json). |
| Node.js, Express, PostgreSQL y JWT | [EventConnect: backend/package.json](https://github.com/T1Angel4220/eventconnect/blob/4694884334b3ee9f36c4c2168f29f12036f4609c/backend/package.json) y [Ventas: backend/package.json](https://github.com/T1Angel4220/SistemaVentas/blob/c235082c546747b4fab5b03727c3f573e6421768/backend/package.json). |
| PHP y Laravel | [Mantenimiento: backend/composer.json](https://github.com/T1Angel4220/Sistema_Mantenimiento/blob/ce947d149b47abdb23c90e9aca29adc7a90c697a/backend/composer.json). |
| MySQL | [HospitalApp: servicio de autenticación](https://github.com/T1Angel4220/AD-GestionHospitalaria/blob/c1814be5c695bdf94913033bb142c71044b56b90/hospital-app/microservices/auth-service/package.json), dependencia mysql2. |
| NestJS y Supabase | [AgenteTelegram: package.json](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/package.json). |
| Java, Spring Boot, gRPC, MongoDB y PostgreSQL | [Combustible SKT](https://github.com/T1Angel4220/Combustible-SKT/tree/bf9dc74e1d8175f79027308b060e2a8e52ba1954): manifiestos Maven, servicios y Docker Compose. |
| Python, Flask y WebRTC | [Mensajes y videollamadas](https://github.com/T1Angel4220/Mensajes_VideoLlamada/tree/591a5f5b51b962450ce37cc9962faedbaa7a9c3c). |
| React Native, Expo, Expo Router, React Navigation, AsyncStorage y notificaciones | [EventConnect Mobile: package.json](https://github.com/T1Angel4220/eventconnect-movil/blob/fcfd02b5383a9ce4a121465e9a84b4c98b40ac9a/package.json). |
| Azure, Docker, Nginx y Linux | [HospitalApp: recursos de Azure](https://github.com/T1Angel4220/AD-GestionHospitalaria/tree/c1814be5c695bdf94913033bb142c71044b56b90/hospital-app/azure): guía de despliegue, Compose, configuración Nginx y script de instalación. |
| GitHub Pages | [Portafolio público](https://t1angel4220.github.io/) y su [repositorio](https://github.com/T1Angel4220/T1Angel4220.github.io). |
| GitHub Actions | [Automatización de contribuciones de este perfil](../.github/workflows/contributions.yml). |

**Angular:** el usuario confirmó que lo conoce mediante cursos y práctica personal. La referencia a Angular en la base de conocimiento de AgenteTelegram no demuestra una implementación Angular en ese repositorio. Por eso el perfil lo etiqueta expresamente como formación y práctica, sin atribuirle una aplicación pública.

**Despliegue:** el usuario afirmó que sabe publicar proyectos. Se incorporó esa capacidad con tareas concretas: preparar builds, configurar variables de entorno y conectar frontend, APIs y bases de datos. La presencia de recursos de despliegue en el repositorio respalda la selección de herramientas; esta revisión no certifica disponibilidad actual de las máquinas de Azure. No se añadieron proveedores por simples menciones: por ejemplo, el agradecimiento a Vercel en el README de Ventas no demuestra un despliegue allí.

## Nuevas capturas

| Proyecto | Fuente | Captura |
| --- | --- | --- |
| Sistema de Ventas | Rama `develop`, commit `c235082c546747b4fab5b03727c3f573e6421768` | [Acceso](../assets/screens/sales.png) e [inicio](../assets/screens/sales-home.png). |
| Mantenimiento | Rama `main`, commit `ce947d149b47abdb23c90e9aca29adc7a90c697a` | [Acceso](../assets/screens/maintenance.png). |

Los frontends se ejecutan desde copias temporales. Las capturas se obtienen con Chrome y conservan la interfaz original. No se inician sesiones ni se agregan datos ficticios. Mostrar estas pantallas no implica haber validado el backend.

Las cuatro tarjetas de proyectos tienen ahora el mismo formato, con captura real, descripción, tecnologías y enlace al código. El stack se presenta en seis tarjetas por idioma: frontend, interfaces, backend, datos, móvil y cloud. Las tecnologías antes ocultas en un bloque desplegable quedan visibles.
