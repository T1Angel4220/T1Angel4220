# AgenteTelegram como proyecto destacado

Revisión del **13 de noviembre de 2026**, sobre [AgenteTelegram](https://github.com/T1Angel4220/AgenteTelegram), rama `main`, commit `c1a1ad3c4be2b5c5c4c36a948639274a888d23f4`.

## Qué demuestra

**LUPSI ChatOps** es un asistente de gestión de proyectos que usa Telegram como interfaz. Su valor para el perfil es mostrar integración de APIs, orquestación de modelos de IA, persistencia y automatización, complementando las interfaces web de EventConnect, HospitalApp y Sistema de Ventas.

Sustituye a Mantenimiento entre los cuatro proyectos destacados. Esto cambia la selección del perfil; Laravel y otras tecnologías de Mantenimiento siguen siendo parte del stack respaldado por repositorios públicos.

## Funciones contrastadas con código

| Capacidad | Evidencia |
| --- | --- |
| Bot e interacción en Telegram | [bot.service.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/bot.service.ts): Telegraf, comandos, mensajes y botones con callbacks. |
| Integraciones con Trello y GitHub | [trello.service.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/trello.service.ts) y [github.service.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/github.service.ts): lectura de tableros y commits, y operaciones sobre tarjetas, issues y pull requests. |
| Orquestación de IA | [ai.service.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/ai.service.ts): llamadas a OpenRouter y NVIDIA NIM con alternativas de modelos y credenciales. |
| Contexto documental | [docs.service.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/docs.service.ts): lectura de documentos, fragmentación y recuperación por relevancia para las consultas. |
| Flujos de aprobación humana | [autonomy.service.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/autonomy.service.ts) y callbacks de aprobación/rechazo en `bot.service.ts`. No se afirma que todas las operaciones estén protegidas por este flujo. |
| Reportes y automatización | [pdf.service.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/pdf.service.ts), PDFKit, y [cron.service.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/cron.service.ts), rutinas de seguimiento y reportes. |
| Persistencia | [supabase.service.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/supabase.service.ts): almacenamiento y recuperación de sesiones. |
| Eventos externos | [webhook.controller.ts](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/src/webhook.controller.ts): recepción de eventos de Telegram, Trello y GitHub, incluyendo workflows. |

El stack confirmado por [package.json](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/package.json) incluye NestJS, TypeScript, Telegraf, Axios, Supabase, PDFKit, pdf-parse y NestJS Schedule.

## Límites de la presentación

- La recuperación documental implementada puntúa coincidencias de palabras clave. El perfil la describe como recuperación de contexto; no afirma que exista una base vectorial o un sistema de embeddings.
- Render, Docker y Cloudinary aparecen en la documentación. En este commit no se encontró un Dockerfile ni una configuración de Render. Estas menciones no se incorporaron como prueba de un despliegue operativo del bot.
- Existe `public/index.html`, una interfaz web que consulta `/metrics`. No se presenta como una demo pública funcional: requiere conectar datos y servicios.
- No se inició el bot ni se usaron credenciales, se enviaron mensajes o se modificaron tableros para esta revisión. El análisis es de código y recursos públicos.

## Vista incorporada al perfil

La nueva tarjeta utiliza [telegram_hitl.png del repositorio](https://github.com/T1Angel4220/AgenteTelegram/blob/c1a1ad3c4be2b5c5c4c36a948639274a888d23f4/telegram_hitl.png), copiada sin modificar a [assets/screens/telegram-hitl.png](../assets/screens/telegram-hitl.png). El SVG encuadra esa imagen y la identifica como **vista del repositorio**. No se presenta como una captura de una sesión verificada por esta revisión.

Los archivos `telegram_estado.png` y `telegram_pdf.png` también se revisaron. No fue necesario inventar conversaciones ni generar imágenes nuevas.

## Diseño de referencia

La carpeta `perfil-v2/` proporcionada por el usuario se conserva intacta. Se adaptaron sus recursos a `assets/v2/`, manteniendo el lenguaje gráfico de gradientes, ventanas de código, títulos con iconos y chips de tecnologías sobre azul oscuro.

Se añadieron composiciones móviles para la introducción, las cinco cabeceras, el stack, los intereses y el cierre. La introducción usa animaciones CSS con movimiento reducido; las animaciones SMIL del ejemplo se retiraron al adaptar los recursos. El banner ilustrado y su alternativa estática permanecen intactos.

El archivo RAR y la carpeta de referencia no forman parte de la publicación. La implementación utiliza los archivos adaptados en `assets/v2/`.
