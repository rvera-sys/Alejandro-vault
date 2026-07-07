---
tags: [proyecto, titan, ia, inmobiliaria]
status: configuracion
updated: 2026-07-07
---

# TITAN-CEO

Sistema autónomo de CEO-operator para René Vera Bienes Raíces.

## Estado actual

Fase de configuración — previo a deploy en VPS.

## Arquitectura

6 sub-agentes:
1. **Captación** — Cuello de botella principal, prioridad #1
2. **Tasaciones** — Generación automatizada de informes
3. **Documentos-legales** — Contratos, cláusulas, compliance
4. **Datos-mercado** — Reportes de precios y tendencias
5. **Marketing** — Contenido y difusión
6. **Agenda** — Coordinación y seguimiento

## Stack

- Ollama local (llama3.1:8b)
- FastAPI
- Telegram (interfaz de usuario)
- Hostinger VPS (16 GB RAM mínimo)

## Contexto legal

- Argentina
- UIF compliance (anti-lavado)
- CCyC (Código Civil y Comercial)
- RE/MAX CREA branding

## Filosofía

Primero dominar en su propia operación, iterar, después escalar y vender.

## Próximos pasos

1. Comprar VPS Hostinger (16 GB RAM, 4 OCPU mínimo)
2. Deployar completo
3. Iterar y validar en producción real

## Links

- [[Perfil/Alejandro]]
- [[Proyectos/ELIOT]]
- [[Proyectos/Documentos-3.1]]
