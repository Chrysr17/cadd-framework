# CADD

🌐 **Idiomas**

- 🇪🇸 Español (Actual)
- 🇺🇸 [English](README.md)

> **Context-Adaptive Development**
>
> *Una metodología ligera para el desarrollo de software asistido por IA, basada en un único contexto del proyecto, agentes especializados por repositorio, colaboración escalable entre agentes y documentación operativa mínima.*

---

# ¿Qué es CADD?

CADD es una metodología ligera para el desarrollo de software asistido por inteligencia artificial.

En lugar de depender de múltiples documentos de planificación y grandes especificaciones, CADD utiliza un **único contexto del proyecto** como fuente de verdad y agentes especializados por repositorio para transformar la planificación en implementación.

Su objetivo es reducir la sobrecarga documental manteniendo:

- Consistencia
- Mantenibilidad
- Trazabilidad
- Escalabilidad

---

# ¿Por qué CADD?

Los flujos tradicionales de desarrollo asistido por IA suelen generar:

- documentación duplicada;
- múltiples documentos de planificación;
- especificaciones excesivamente grandes;
- documentación que rápidamente queda desactualizada.

CADD resuelve estos problemas manteniendo todo el contexto del proyecto en un único lugar y permitiendo que agentes especializados generen y mantengan únicamente la documentación que realmente aporta valor.

---

# Principios Fundamentales

CADD se basa en los siguientes principios.

## Single Source of Truth

`CONTEXT.md` es el único documento de planificación del proyecto.

Todas las decisiones del proyecto parten de este documento.

---

## Agentes Especializados por Repositorio

Cada repositorio cuenta con un agente especializado.

Ejemplos:

- Backend
- Frontend
- IA
- Mobile
- DevOps

Cada agente se enfoca únicamente en las responsabilidades de su propio repositorio.

---

## Escalabilidad de Agentes

CADD soporta tanto desarrollo con un único agente como colaboración entre múltiples agentes.

Los proyectos pueden utilizar:

- un único agente por repositorio;
- múltiples agentes por repositorio;
- agentes especializados colaborando sobre el mismo sistema.

La cantidad de agentes dependerá de:

- el tamaño del proyecto;
- la complejidad del sistema;
- el tamaño del equipo;
- la experiencia de los desarrolladores.

CADD no requiere múltiples agentes.

La misma metodología escala de forma natural desde un único desarrollador hasta equipos de ingeniería de gran tamaño sin modificar sus principios.

### Estrategia Recomendada

| Tamaño del Proyecto | Estrategia Recomendada |
|----------------------|------------------------|
| Pequeño | Un único agente por repositorio |
| Mediano | Agentes especializados por repositorio |
| Grande | Colaboración entre múltiples agentes |

---

## Documentación Operativa Mínima

Generar únicamente la documentación que aporte valor.

La documentación operativa evoluciona junto con el proyecto en lugar de crearse completamente desde el inicio.

---

## Convention over Configuration

Las reglas técnicas pertenecen a `CONVENTIONS.md`.

La metodología permanece independiente de frameworks, lenguajes de programación y tecnologías específicas.

---

## Desarrollo Adaptativo

Los agentes se adaptan a:

- el repositorio;
- el proyecto;
- el stack tecnológico;
- el equipo de desarrollo.

Los proyectos nunca deberían adaptarse al agente.

---

## Integración Contract-First

Cuando existen contratos API:

- El Backend es propietario del contrato.
- El Frontend consume dicho contrato.

Las reglas específicas de integración pertenecen a `CONVENTIONS.md`.

---

# Inicio Rápido

Comenzar a utilizar CADD toma menos de cinco minutos.

## 1. Selecciona el agente adecuado

Actualmente existen los siguientes agentes:

- Backend
- Frontend

---

## 2. Copia AGENTS.md

Copia el `AGENTS.md` correspondiente en la raíz del repositorio.

Ejemplo:

```text
mi-proyecto/

AGENTS.md
README.md
src/
```

---

## 3. Crea CONTEXT.md

Crea un archivo `CONTEXT.md`.

Este documento representa la **Single Source of Truth** del proyecto.

Debe describir:

- objetivo del proyecto;
- alcance;
- arquitectura;
- stack tecnológico;
- módulos;
- integraciones;
- restricciones;
- roadmap;
- estado actual;
- idioma del proyecto (*Project Language*).

---

## 4. Inicia tu Agente de IA

El agente automáticamente:

- leerá `CONTEXT.md`;
- comprenderá el alcance del repositorio;
- generará la documentación operativa cuando sea necesario;
- mantendrá sincronizada la documentación con la implementación.

---

# Documentación Generada

Dependiendo del proyecto, el agente podrá generar automáticamente:

| Archivo | Propósito |
|----------|-----------|
| `CONVENTIONS.md` | Convenciones técnicas del proyecto |
| `TASKS.md` | Estado operativo del desarrollo |
| `DECISIONS.md` | Decisiones técnicas |
| `CHANGELOG.md` | Historial de cambios implementados |

Estos documentos evolucionan junto con el proyecto.

---

# Flujo de Trabajo

```text
              Planificación del Proyecto
                       │
                       ▼
                  CONTEXT.md
                       │
        ┌──────────────┼──────────────┐
        ▼              ▼              ▼
 Backend Agent   Frontend Agent    AI Agent
        │              │              │
        └──────────────┼──────────────┘
                       ▼
                 Implementación
                       │
        ┌──────────────┼──────────────┐
        ▼              ▼              ▼
    TASKS.md     DECISIONS.md   CHANGELOG.md
```

---

# Estructura Actual

```text
CADD/

├── Backend/
│   └── AGENTS.md
│
└── Frontend/
    └── AGENTS.md
```

En futuras versiones podrán incorporarse:

- Plantillas
- AI Agent
- Mobile Agent
- DevOps Agent
- Proyectos de ejemplo

---

# Filosofía

CADD sigue una idea muy simple.

> **El contexto guía al agente.  
> El agente impulsa la implementación.**

La documentación existe para apoyar el desarrollo, no para ralentizarlo.

Un proyecto solo debería contener la documentación que realmente aporta valor.

---

# Roadmap

## Disponible

- ✅ Backend Agent
- ✅ Frontend Agent

## Planificado

- ⬜ Plantilla de CONTEXT
- ⬜ Plantilla de CONVENTIONS
- ⬜ Plantilla de TASKS
- ⬜ Plantilla de DECISIONS
- ⬜ Plantilla de CHANGELOG
- ⬜ AI Agent
- ⬜ Mobile Agent
- ⬜ DevOps Agent
- ⬜ Proyectos de ejemplo

---

# Estado

**Experimental**

CADD continúa evolucionando a partir de experiencias reales de desarrollo de software.

---

# Versión

**CADD v1.0**

---

# Autor

Creado y mantenido por

**Christian Sánchez**

Software Engineer

Peru

---

# Licencia

Pendiente de definir.