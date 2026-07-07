---
tags: [windows, powershell, herramientas, configuracion]
updated: 2026-07-01
---

# Windows — Setup y herramientas

## Sistema

- **OS:** Windows 11 Pro (10.0.26200)
- **Shell:** PowerShell 5.1 (`powershell.exe`)
- **Package manager:** `winget` (preferido para instalar software)

## Herramientas instaladas

| Herramienta         | Versión   | Ubicación / Notas                                  |
|--------------------|-----------|---------------------------------------------------|
| Node.js            | v24.15.0  | Sistema                                           |
| Python             | 3.12.10   | Instalado vía winget                              |
| Playwright         | Global    | npm global, incluye Chromium + Firefox + WebKit  |
| Tailscale          | 1.98.2    | IP: `100.70.74.73`, device: `home2026`           |
| Antigravity CLI    | 1.0.0     | `%LOCALAPPDATA%\agy\bin\`                        |
| Antigravity IDE    | —         | `%LOCALAPPDATA%\Programs\antigravity\`            |
| Antigravity SDK    | 0.1.1     | `google-antigravity` Python package               |
| Lively Wallpaper   | —         | Instalado vía winget                              |
| OpenCode           | desktop   | `%LOCALAPPDATA%\Programs\@opencode-aidesktop\`   |
| Ollama             | —         | Servicio sistema, puerto 11434                    |
| PM2                | —         | npm global, gestor de procesos                    |
| Spicetify          | —         | `C:\Users\Inmov\spicetify-cli\`                  |

## Convenciones PowerShell

- Usar PowerShell 5.1 (`powershell.exe`), no PowerShell 7
- `&&` no disponible en PS 5.1 — usar `;` o `if ($?) { ... }`
- Variables de entorno: `$env:NOMBRE`
- No usar `2>&1` en executables nativos (bug en PS 5.1)
- Archivos: encoding `UTF-8` con `-Encoding utf8`

## Tailscale

- VPN mesh para acceso remoto al stack
- IP estática: `100.70.74.73`
- Device name: `home2026`

## Notas relacionadas

- [[Proyectos/Stack-Servicios]]
- [[Proyectos/OpenCode]]
- [[Perfil/Alejandro]]
