# CADD

🌐 **Idiomas**

* 🇺🇸 [English](README.md)
* 🇪🇸 Español (Actual)

> **Context-Adaptive Development**
>
> *Una metodología ligera de desarrollo asistido por IA basada en un único contexto de proyecto, agentes especializados, colaboración escalable entre agentes y documentación operativa mínima.*

---

# ¿Qué es CADD?

CADD es una metodología ligera para el desarrollo asistido por IA.

En lugar de depender de múltiples documentos de planificación y especificaciones extensas, CADD utiliza un **único contexto de proyecto** como fuente de verdad y agentes especializados para transformar la planificación en implementación.

El objetivo es reducir la carga documental, manteniendo:

* Consistencia
* Mantenibilidad
* Trazabilidad
* Escalabilidad

---

# ¿Por qué CADD?

Los flujos tradicionales de desarrollo asistido por IA suelen generar:

* documentación duplicada;
* múltiples documentos de planificación;
* especificaciones demasiado extensas;
* documentación que se desactualiza rápidamente.

CADD aborda estos problemas manteniendo el contexto del proyecto en un solo lugar y permitiendo que agentes especializados generen y mantengan únicamente la documentación que aporta valor.

---

# Principios Fundamentales

CADD se basa en los siguientes principios.

## Fuente Única de Verdad

`CONTEXT.md` es el documento principal de planificación del proyecto.

Todas las decisiones del proyecto parten de este documento.

---

## Agentes Especializados

Cada agente tiene una responsabilidad clara.

Los agentes pueden organizarse por:

* repositorio;
* capa técnica;
* área del sistema;
* rol de desarrollo;
* especialización de dominio.

Ejemplos:

* Backend Agent
* Frontend Agent
* Fullstack Agent
* Control Systems Agent
* AI Agent
* Mobile Agent
* DevOps Agent

Cada agente se enfoca únicamente en su alcance definido y evita asumir responsabilidades fuera de su rol.

---

## Agentes Orientados a Repositorio y Dominio

CADD soporta tanto agentes orientados a repositorio como agentes orientados a dominio.

Los agentes orientados a repositorio son útiles cuando un proyecto está dividido en bases de código separadas, como repositorios backend y frontend.

Los agentes orientados a dominio son útiles cuando el trabajo requiere conocimiento especializado, como sistemas de control, inteligencia artificial, infraestructura, ciberseguridad, procesamiento de datos o sistemas embebidos.

Esto permite que CADD pueda aplicarse tanto a proyectos tradicionales de software como a flujos de ingeniería más especializados.

---

## Escalabilidad de Agentes

CADD soporta tanto desarrollo con un solo agente como desarrollo multiagente.

Los proyectos pueden usar:

* un único agente de repositorio;
* un agente fullstack;
* múltiples agentes orientados a repositorio;
* agentes especializados colaborando sobre el mismo sistema.

La cantidad de agentes debe determinarse según:

* tamaño del proyecto;
* complejidad del sistema;
* tamaño del equipo;
* experiencia del desarrollador;
* complejidad del dominio.

CADD no exige el uso de múltiples agentes.

La misma metodología escala naturalmente desde un solo desarrollador hasta equipos de ingeniería grandes sin cambiar sus principios base.

### Estrategia Recomendada

| Tamaño / Contexto del Proyecto | Estrategia Recomendada                          |
| ------------------------------ | ----------------------------------------------- |
| Proyecto pequeño               | Un solo agente de repositorio o Fullstack Agent |
| Proyecto mediano               | Agentes orientados a repositorio                |
| Proyecto grande                | Colaboración multiagente                        |
| Dominio especializado          | Agente orientado a dominio                      |
| Proyecto para principiantes    | Fullstack Agent con convenciones guiadas        |

---

## Documentación Operativa Mínima

Genera solo la documentación que aporta valor.

La documentación operativa evoluciona junto con el proyecto en lugar de crearse completamente desde el inicio.

---

## Convención sobre Configuración

Las reglas técnicas pertenecen a `CONVENTIONS.md`.

La metodología se mantiene independiente de frameworks, lenguajes de programación y tecnologías específicas.

---

## Desarrollo Adaptativo

Los agentes se adaptan a:

* el repositorio;
* el proyecto;
* el stack tecnológico;
* el equipo de desarrollo;
* el dominio;
* el nivel de experiencia del desarrollador.

Los proyectos nunca deben verse obligados a adaptarse al agente.

---

## Integración Contract-First

Cuando existen contratos de API:

* Backend es dueño del contrato.
* Frontend consume el contrato.

Las reglas de integración específicas del proyecto pertenecen a `CONVENTIONS.md`.

---

# Inicio Rápido

Empezar con CADD toma menos de cinco minutos.

## 1. Elegir el agente apropiado

Agentes disponibles actualmente:

* Backend Agent
* Frontend Agent
* Fullstack Agent
* Control Systems Agent

Usa el agente que mejor coincida con el repositorio o alcance del proyecto.

Uso recomendado:

| Agente                | Cuándo usarlo                                                                                                                  |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| Backend Agent         | Repositorios solo backend, APIs, servicios, bases de datos y lógica de negocio                                                 |
| Frontend Agent        | Repositorios solo frontend, interfaces, páginas, componentes e integración cliente                                             |
| Fullstack Agent       | Proyectos pequeños o para principiantes donde frontend y backend se manejan juntos                                             |
| Control Systems Agent | Proyectos relacionados con sistemas de control, automatización, modelado, simulación o análisis del comportamiento de sistemas |

---

## 2. Copiar AGENTS.md

Copia el `AGENTS.md` correspondiente en la raíz de tu repositorio.

Ejemplo:

```text
my-project/

AGENTS.md
README.md
src/
```

Para un espacio de trabajo multiagente, cada agente puede vivir en su propia carpeta:

```text
CADD/

backend-agent/
frontend-agent/
fullstack-agent/
control-systems-agent/
```

---

## 3. Crear CONTEXT.md

Crea un archivo `CONTEXT.md`.

Este documento es la **Fuente Única de Verdad** del proyecto.

Debe describir:

* objetivo del proyecto;
* alcance;
* arquitectura;
* stack tecnológico;
* módulos;
* integraciones;
* restricciones;
* roadmap;
* estado actual;
* idioma del proyecto.

---

## 4. Iniciar tu Agente de IA

El agente automáticamente:

* leerá `CONTEXT.md`;
* entenderá el alcance del proyecto;
* aplicará sus responsabilidades especializadas;
* generará documentación operativa cuando sea necesario;
* mantendrá la documentación sincronizada con la implementación.

---

# Documentación Generada

Dependiendo del proyecto, el agente puede generar automáticamente:

| Archivo          | Propósito                                      |
| ---------------- | ---------------------------------------------- |
| `CONVENTIONS.md` | Convenciones técnicas específicas del proyecto |
| `TASKS.md`       | Trabajo operativo actual                       |
| `DECISIONS.md`   | Decisiones técnicas                            |
| `CHANGELOG.md`   | Cambios implementados                          |

Estos documentos evolucionan junto con el proyecto.

---

# Flujo de Trabajo Típico

```text
                  Planificación del Proyecto
                            │
                            ▼
                       CONTEXT.md
                            │
          ┌─────────────────┼─────────────────┬──────────────────────┐
          ▼                 ▼                 ▼                      ▼
 Backend Agent      Frontend Agent      Fullstack Agent      Control Systems Agent
          │                 │                 │                      │
          └─────────────────┼─────────────────┴──────────────────────┘
                            ▼
                     Implementación
                            │
          ┌─────────────────┼─────────────────┐
          ▼                 ▼                 ▼
      TASKS.md        DECISIONS.md      CHANGELOG.md
```

---

# Estructura Actual de Carpetas

```text
CADD/

├── backend-agent/
│   └── AGENTS.md
│
├── frontend-agent/
│   └── AGENTS.md
│
├── fullstack-agent/
│   └── AGENTS.md
│
└── control-systems-agent/
    └── AGENTS.md
```

Versiones futuras pueden incluir:

* Plantillas
* AI Agent
* Mobile Agent
* DevOps Agent
* Data Agent
* Cybersecurity Agent
* Proyectos de ejemplo

---

# Filosofía

CADD sigue una idea simple.

> **El contexto guía al agente.
> El agente guía la implementación.**

La documentación existe para apoyar el desarrollo, no para ralentizarlo.

Los proyectos deben contener solo la documentación que aporta valor.

---

# Roadmap

## Disponible

* ✅ Backend Agent
* ✅ Frontend Agent
* ✅ Fullstack Agent
* ✅ Control Systems Agent

## Planificado

* ⬜ Plantilla de CONTEXT
* ⬜ Plantilla de CONVENTIONS
* ⬜ Plantilla de TASKS
* ⬜ Plantilla de DECISIONS
* ⬜ Plantilla de CHANGELOG
* ⬜ AI Agent
* ⬜ Mobile Agent
* ⬜ DevOps Agent
* ⬜ Data Agent
* ⬜ Cybersecurity Agent
* ⬜ Proyectos de ejemplo

---

# Estado

Estado actual

**Experimental**

CADD evoluciona activamente a partir de experiencias reales de desarrollo de software.

---

# Versión

**CADD v1.0**

---

# Autor

Creado y mantenido por

**Christian Sánchez**

Software Developer

Perú

---

# Licencia

Licencia por definir.