# Checkpoint 4 - Integraciones avanzadas en n8n

Workflow desarrollado en n8n para gestionar correos de soporte mediante integraciones con Gmail, HubSpot y Slack.

## Objetivo

Automatizar la recepción y clasificación de correos, registrar contactos en HubSpot, generar una respuesta en borrador para revisión humana y notificar al equipo de operaciones mediante Slack.

## Funcionamiento

1. Gmail recibe un nuevo correo.
2. Se bloquean respuestas automáticas, mensajes fuera de oficina y correos no entregados.
3. Se normalizan el correo del cliente, el asunto y el mensaje.
4. HubSpot busca el contacto por email.
5. Si el contacto no existe, se crea automáticamente.
6. Gmail genera un borrador de respuesta.
7. El borrador queda pendiente de revisión humana antes del envío.
8. Se limpia el payload antes de enviarlo a Slack.
9. Slack notifica la creación del borrador en el canal de operaciones.

## Integraciones utilizadas

- Gmail
- HubSpot CRM
- Slack
- n8n

## Controles implementados

- Bloqueo de respuestas automáticas.
- Prevención de contactos duplicados.
- Permisos mínimos en HubSpot y Slack.
- Limpieza del payload.
- Human-in-the-loop mediante borrador de Gmail.
- El workflow no envía correos automáticamente.

## Archivo entregable

`checkpoint4_norberto_sanchez.json`

## Autor

Norberto Sánchez

## Fecha

17 de julio de 2026
