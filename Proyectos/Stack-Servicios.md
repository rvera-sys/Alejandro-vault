---
tags: [infraestructura, servicios, pm2]
updated: 2026-07-01
---

# Stack de servicios locales

Servicios configurados para auto-inicio al login en Windows.

## Tabla de servicios

| Servicio     | Puerto | Directorio                              | Comando                    |
|-------------|--------|-----------------------------------------|----------------------------|
| Open WebUI  | 8080   | `C:\Users\Inmov\open-webui-env`        | `python run_owui.py`       |
| Uptime Kuma | 3001   | `C:\Users\Inmov\uptime-kuma`           | `node server/server.js`    |
| n8n         | 5678   | Global npm                              | `n8n start`                |
| Homer       | 3000   | `C:\Users\Inmov\homer`                 | `python -m http.server 3000` |
| Ollama      | 11434  | Sistema                                 | `ollama serve`             |

## n8n

- Puerto: **5678**
- Instalado globalmente vía npm
- Usado para automatizaciones y flujos de trabajo
- Archivos PM2: `C:\Users\Inmov\ecosystem.config.cjs`

## Open WebUI

- Puerto: **8080**
- Virtualenv: `C:\Users\Inmov\open-webui-env`
- Script arranque: `run_owui.py`
- Logs: `open-webui.log` / `open-webui.err`

## Uptime Kuma

- Puerto: **3001**
- Directorio: `C:\Users\Inmov\uptime-kuma`
- Monitor de uptime para los servicios del stack

## Ollama

- Puerto: **11434**
- Modelo principal: `qwen3.5:9b`
- Usado por OpenCode como LLM local

## PM2

- Config principal: `ecosystem.config.cjs` en `C:\Users\Inmov\`
- Wrappers: `n8n-wrapper.cjs`, `n8n-pm2-wrapper.cjs`
- Scripts arranque: `n8n-start.cmd`, `n8n-start.ps1`

## Historial de cambios

- **2026-05-22:** Instalación completa del stack de infraestructura local
- **2026-07-01:** Volcado a Obsidian como memoria externa

## Notas relacionadas

- [[Proyectos/WhatsApp-CRM]]
- [[Proyectos/OpenCode]]
- [[Perfil/Alejandro]]
