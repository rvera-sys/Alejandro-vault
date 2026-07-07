---
tags: [opencode, llm, ollama, configuracion]
updated: 2026-07-01
---

# OpenCode — Setup y configuración

## Instalación

- **App desktop:** `%LOCALAPPDATA%\Programs\@opencode-aidesktop\`
- **Config global:** `C:\Users\Inmov\.config\opencode\opencode.json`

## Modelo

- `ollama/qwen3.5:9b` (local, vía Ollama en puerto 11434)

## Estructura de archivos config

```
C:\Users\Inmov\.config\opencode\
├── opencode.json          ← config principal
├── SYSTEM_MEMORY.md       ← prompt de sistema (memoria v2)
├── AGENTS.md              ← preferencias del usuario y workspace facts
└── skills/
    ├── powershell/
    └── git-workflow/
```

## Plugins instalados

- `opencode-continual-learning`
- `@tarquinen/opencode-dcp@latest`
- `opencode-plugin-openspec@latest`

## MCP conectados

- `sequential-thinking`
- `playwright`

## Instrucciones de config

- Usa `instructions` (NO `systemPrompt`, está deprecado) apuntando a `SYSTEM_MEMORY.md`
- Modelo: `ollama/qwen3.5:9b`

## Reglas importantes (`opencode.json`)

### Modalities
En `modalities.output`, solo se aceptan: `["text", "audio", "image", "video", "pdf"]`  
**El valor `"embedding"` NO es válido** aunque sea semánticamente correcto.

Si aparece `ConfigInvalidError` en una versión nueva, verificar que ningún modelo tenga `"embedding"` en `modalities.output`.

## Historial de fixes

### Fix 2026-05-25
`SYSTEM_MEMORY.md` estaba truncado — faltaban: formato YAML de notas, sesiones diarias, `/memory`, `/commit-memory`, inicialización. Restaurado contenido completo v2.

### Fix 2026-06-24
`ConfigInvalidError` en v1.17.9 causado por `modalities.output: ["embedding"]` en modelos de LM Studio.  
**Solución:** eliminar el campo `modalities` de los modelos `google/gemma-4-e4b` y `text-embedding-nomic-embed-text-v1.5`.

## Notas relacionadas

- [[Proyectos/Stack-Servicios]]
- [[Configuraciones/Windows-Setup]]
