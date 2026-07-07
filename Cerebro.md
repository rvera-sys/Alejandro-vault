---
tags: [cerebro, central, todo]
updated: 2026-07-07
---

# Cerebro — Alejandro

> Un solo archivo con todo. Fuente de verdad única.

---

## Identidad

- **Nombre completo:** René Alejandro Vera
- **Apodo:** Alejandro
- **Nacimiento:** 1982
- **Ubicación:** Granbur, Malvinas Argentinas, Buenos Aires
- **Familia:**
  - Esposa: Sabrina Noelia Monges
  - Hijo: Ian Uriel Vera
  - Hermano: Sebastián Juan Mauricio Vera (1.5 años menor)

## Contacto

- **Email personal:** inmovera2011@outlook.com
- **Email empresa:** inmovera2011@gmail.com (Google account, acceso Gemini Pro)
- **Email trabajo:** rvera@remax.com.ar
- **GitHub:** rvera-sys
- **Organización:** RE/MAX

---

## Profesión

- **Título:** Martillero, Corredor y Tasador Inmobiliario
- **Credenciales:** CPI 6778 / CMCPSI 5848
- **Rol actual:** Corredor matriculado responsable en Red/Remax
- **Importante:** NO es dueño de la oficina, solo responsable inmobiliario
- **Equipo:** Lidera aproximadamente 50 agentes y staff
- **Propuesta de valor:** Vende seguridad y responsabilidad

### Trayectoria laboral

1. **Registro Automotor:** 2 años
2. **Escribanía:** 4-6 meses
3. **Martillero:** 14 años (recibido alrededor de 2012)

### Formación académica

- **Análisis de Sistemas:** A los 19-20 años
- **Economía Industrial:** Universidad Nacional de General Sarmiento (UNSAM)
- **Ingeniería en Informática:** Universidad Abierta (UA), sede San Isidro — no pasó el ingreso
- **Martillería:** Cámara Inmobiliaria Argentina (CIA)
- **Título universitario:** Universidad de Morón

---

## Intereses personales

- **Pasión principal:** Inteligencia Artificial (IA generativa, automatización)
- **Prompt Engineering:** 40 técnicas avanzadas (role assignment, chain of thought, few-shot, meta-prompting)
- **Deportes:** Tenis (Partido de Tortuguitas y Bella Vista)
- **Hobbies:** Scrabble, tecnología, trading (BTC perpetual futures en Bitget)

## Relación con IA

- **Descubrimiento:** ChatGPT (fin de 2022)
- **Evolución:** ChatGPT → Claude → sistemas autónomos
- **Mentalidad técnica** desde análisis de sistemas (20 años atrás), IA le dio la herramienta para ejecutar
- **Enfoque:** Más rápido, no delegación total — aprende y controla

---

## Entorno de trabajo

| Recurso | Versión / Valor |
|---|---|
| OS | Windows 11 Pro (10.0.26200) |
| Shell | PowerShell 5.1 |
| Node.js | v24.15.0 |
| Python | 3.12.10 (winget) |
| Tailscale | v1.98.2 — IP: 100.70.74.73, device: home2026 |

## Stack tecnológico

- **Workflow:** n8n, Supabase, Evolution API (WhatsApp)
- **Frontend:** Next.js/Vercel, React, HTML/CSS
- **Backend:** FastAPI, Node.js, Python
- **DB:** PostgreSQL, SQLite, ChromaDB
- **IA:** Ollama, LM Studio, Claude API/Code/OpenCode, OpenAI APIs, Gemini Pro
- **Auth:** Google OAuth2
- **Notas:** Obsidian vault local
- **Versionado:** GitHub

## Preferencias de colaboración

- Responder en **español**, tono amable y cercano
- **Directo y output-focused:** sin explicaciones overhead
- **Autonomía total:** actuar sin delegar pasos ni pedir permiso para lo obvio
- `winget` para instalar software en Windows
- Soluciones prácticas sobre perfectas
- Herramientas locales y open-source

---

## Proyectos

### TITAN-CEO
- **Estado:** Fase de configuración
- **Objetivo:** Sistema autónomo CEO-operator para René Vera Bienes Raíces
- **Arquitectura:** 6 sub-agentes (captación, tasaciones, doc-legales, datos-mercado, marketing, agenda)
- **Stack:** Ollama local (llama3.1:8b), FastAPI, Telegram, Hostinger VPS (16 GB RAM mínimo)
- **Contexto:** Argentina, UIF compliance, CCyC, RE/MAX CREA branding
- **Prioridad:** Captación de negocios (cuello de botella)
- **Filosofía:** Primero dominar en su operación, iterar, después escalar y vender
- **Próximo paso:** Comprar VPS Hostinger y deployar

### E.L.I.O.T
- **Estado:** Roadmap 20 semanas en progreso (3-5 meses a MVP)
- **Tipo:** SaaS white-label para inmobiliarias de 5-50 agentes
- **Departamentos:** Ventas, Marketing, Setting, Desarrollo, Análisis, Operaciones
- **Stack:** React + FastAPI + PostgreSQL + Claude API
- **Precios:** Starter $199/mes — Enterprise $1,999/mes

### Documentos 3.1
- **Estado:** ✅ Completo y deployado
- **Tipo:** Generación legal de documentos multi-usuario
- **Cobertura:** 17 templates (8 compra, 9 alquiler) + 100+ cláusulas dinámicas
- **Stack:** GitHub Pages + Vercel Functions + Supabase + Google OAuth2

### Reporte Precios
Sistema automatizado de reportes PDF de mercado inmobiliario.

### HMM Market Regime Detection
Hidden Markov Model para análisis de regímenes de mercado (trading).

### n8n WhatsApp Automation
Chatbot inmobiliario + catálogo + booking + recordatorios vía n8n + Evolution API.

### TasaciónPRO / InformeTasacion
Generador HTML de informes de tasación profesional.

### Trading Tools
5 estrategias BTC perpetual futures en Bitget: RSI, EMA, MACD, Bollinger, Stochastic.

---

## Stack de servicios (PM2, auto-inicio)

| Servicio | Puerto | Ruta |
|---|---|---|
| Open WebUI | 8080 | C:\Users\Inmov\open-webui-env |
| Uptime Kuma | 3001 | C:\Users\Inmov\uptime-kuma |
| n8n | 5678 | global npm |
| Homer | 3000 | C:\Users\Inmov\homer |
| Ollama | 11434 | sistema |

## WhatsApp CRM (C:\wa-crm\)

- Baileys (sin navegador) + SQLite + PM2
- wa-bridge: puerto 3459 | wa-dashboard: puerto 3458
- Bot "Joaquín, asistente de Alejandro" con Ollama tinyllama local
- Sesión persistente en C:\wa-crm\auth\ (multi-file-auth)
- Procesos PM2 salvados, auto-inicio por script en Startup

---

## Metodología de sesiones

- Cada sesión se documenta en `sessions/YYYY-MM-DD-tema.md`
- Este cerebro se actualiza cuando hay cambios
- La memoria persistente del agente (agentmemory) se mantiene sincronizada
