# SONA

Plataforma musical multiplataforma con diseño **Liquid Glass**, estética negra y morada, y una sola interfaz para Windows, Linux, tablets y móviles Android y navegador (PWA).

> Estado: **Fase 1 de 12** (estructura, identidad visual y sistema Liquid Glass). El proyecto está en desarrollo temprano; todavía no reproduce música.

## Objetivo
Reunir YouTube, Spotify y Apple Music en una sola app usando **únicamente APIs y SDK oficiales**: sin extraer audio, sin saltarse DRM y sin simular suscripciones.

## Stack
| Capa | Tecnología |
|---|---|
| Interfaz | React + TypeScript + Vite, CSS variables, `backdrop-filter` |
| Web | PWA (Service Worker + manifest) |
| Escritorio | Tauri (Windows y Linux) |
| Android | Capacitor + Kotlin para funciones nativas |
| Backend | Node.js, API REST, PostgreSQL |

## Estructura
```
sona/
├─ apps/
│  └─ web/            Interfaz compartida (React + TS + Vite)
├─ packages/          Núcleo, reproductor, proveedores, letras, configuración (próximas fases)
├─ docs/              Arquitectura y documentación por fase
└─ .github/           CI y plantillas de issues
```

## Empezar
Requisitos: Node.js 20 o superior y npm.
```bash
npm install
npm run dev          # http://localhost:5173
npm run typecheck
npm run build
```

## Fases
| # | Fase | Estado |
|---|---|---|
| 1 | Estructura, identidad y Liquid Glass | En pruebas |
| 2 | Versión de escritorio | Pendiente |
| 3 | Tablets Android | Pendiente |
| 4 | Móvil Android | Pendiente |
| 5 | Reproductor | Pendiente |
| 6 | Biblioteca, playlists y favoritos | Pendiente |
| 7 | Integraciones oficiales | Pendiente |
| 8 | Cuentas y sincronización | Pendiente |
| 9 | Instaladores Windows y Linux | Pendiente |
| 10 | APK y AAB | Pendiente |
| 11 | Pruebas de calidad y seguridad | Pendiente |
| 12 | Documentación y distribución | Pendiente |

## Seguridad
Nunca subas claves ni tokens. Usa `.env` (ignorado por Git) a partir de `.env.example`.

## Documentación
- [Arquitectura](docs/ARCHITECTURE.md)
- [Fase 1](docs/PHASE-1.md)

## Licencia
Todos los derechos reservados. Ver [LICENSE](LICENSE).
