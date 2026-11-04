# Checkpoint 4: Sincronización del Cerebro Agéntico con Ecosistemas de Negocio
**Alumno:** Williams Joel De Simone

## Descripción del Workflow
Este proyecto implementa la interconexión bidireccional de un sistema multi-agente con herramientas externas (Gmail, HubSpot y Slack) mediante protocolos seguros OAuth2 y API Tokens, integrando los siguientes controles preventivos no-code:
- **Filtro Anti-Spam y Bucle Infinito:** Control inicial sobre los correos entrantes de soporte para descartar respuestas automáticas (`Auto-reply`, `Out of office`, `Undeliverable`).
- **Limpieza de Payload:** Normalización y estructuración de los datos del mensaje mediante nodos de asignación y filtrado.
- **Búsqueda (Look up) en HubSpot:** Verificación previa de contactos en el CRM antes de ejecutar acciones de escritura, previniendo de forma absoluta el *Error 409* por duplicados.
- **Gobernanza Human-in-the-loop:** Generación automática de borradores en Gmail (`Create Draft`) para asegurar la supervisión humana antes del envío definitivo.
- **Notificaciones a Slack:** Envío automatizado de resúmenes operativos al canal del equipo.

## Evidencia de Credenciales Activas
A continuación se evidencian las conexiones autenticadas en n8n:

### Gmail OAuth2 API
![Gmail Credencial] (credentials_gmail.png)

### Slack OAuth2 API
![Slack Credencial] (credentials_slack.png)

### HubSpot Service Key
![HubSpot Credencial] (credentials_hubspot.png)
