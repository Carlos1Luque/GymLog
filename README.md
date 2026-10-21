# GymLog

Aplicación personal para registrar entrenamientos: ejercicios, series y repeticiones. Arranca como una interfaz estática y crece hacia una aplicación con backend propio.

## Objetivo

Llevar la cuenta de cada sesión de entrenamiento de forma simple, desde el celular o la PC, sin depender de aplicaciones de terceros.

## Estado actual — Etapa 1: interfaz estática

- Interfaz HTML + CSS con tema oscuro, moderna y responsive.
- Panel principal de entrenamiento y sección visual de ejercicios, series y repeticiones.
- Estados vacíos con mensajes claros y HTML semántico accesible.
- Los botones y el ejercicio mostrados son **demostrativos**: todavía no realizan acciones.
- Sin JavaScript, sin persistencia ni backend: por ahora es solo visual.

## Etapas futuras

- **Etapa 2:** lógica con JavaScript y persistencia en `localStorage` (guardar entrenamientos en el dispositivo).
- **Etapa 3:** backend en C# con ASP.NET Core Web API y base de datos.
- **Etapa 4 (posible):** autenticación y sincronización entre dispositivos.

## Estructura

```
GymLog/
├── frontend/            # Interfaz estática (HTML + CSS)
│   ├── index.html
│   └── css/styles.css
├── docs/ai/             # Contexto del proyecto para agentes IA
├── .claude/skills/      # Skills reutilizables de desarrollo asistido
├── AGENTS.md            # Reglas que siguen los agentes de programación
├── CLAUDE.md            # Punto de entrada para Claude Code
└── README.md
```

## Uso

Abrir `frontend/index.html` en cualquier navegador. En esta etapa no requiere servidor, dependencias ni instalación.

## Convenciones

- Commits convencionales: `feat:`, `fix:`, `docs:`, `test:`, `refactor:`, `chore:`.
- Flujo por etapas: `Desarollo` → `Testing` → `Produccion`, integrando mediante PR con squash.
- La rama de trabajo `feat/estructura-inicial` parte de `origin/Desarollo` (se actualiza con `git pull origin Desarollo`), respetando el flujo actual. No se renombran ramas ni se cambia la configuración remota.
- Las reglas de trabajo con agentes de programación están en [AGENTS.md](AGENTS.md).

## Licencia

Uso personal. Licencia a definir si se decide publicar el código.
