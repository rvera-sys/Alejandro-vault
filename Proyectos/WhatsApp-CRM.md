---
tags: [whatsapp, crm, baileys, sqlite, pm2]
updated: 2026-07-01
---

# WhatsApp CRM

## Stack

- **Biblioteca:** Baileys (sin browser, WhatsApp Web API unofficial)
- **Base de datos:** SQLite
- **Gestor de procesos:** PM2
- **Directorio:** `C:\wa-crm\`

## Procesos y puertos

| Proceso      | Puerto | Descripción          |
|-------------|--------|----------------------|
| wa-bridge   | 3459   | Bridge WhatsApp      |
| wa-dashboard | 3458  | Dashboard de gestión |

## Bot Joaquín

- **Nombre:** "Joaquín, asistente de Alejandro"
- **Modelo:** Ollama `tinyllama` (local)
- **Sesión:** persistente en `C:\wa-crm\auth\` (multi-file-auth)

## Estado

- Procesos PM2 salvados, auto-inicio por script en Startup\
- SQLite como persistencia local de contactos/mensajes

## Notas relacionadas

- [[Proyectos/Stack-Servicios]]
- [[Perfil/Alejandro]]
