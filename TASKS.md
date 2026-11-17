# Tareas asignadas — Proyecto Aquiles

**Asignado a:** Dayron (CEO)  
**Ámbito:** configuración y gobierno del repositorio GitHub `proyecto_aquiles`  
**Objetivo:** dejar el repositorio operativo, trazable y con estándar de matrícula de honor.

---

## 1. Gobierno del repositorio (prioridad alta)

- [ ] **Crear/validar el repositorio** `proyecto_aquiles` en GitHub (organización o cuenta oficial) y definir visibilidad (público/privado).
- [ ] **Configurar descripción y topics** del repositorio: `sports-tech`, `computer-vision`, `ai`, `jump-analysis`, `coaching`, `marketplace`.
- [ ] **Definir rama por defecto** (`main`) y estrategia de ramas (`main`, `develop` opcional, `feature/*`, `fix/*`, `docs/*`).
- [ ] **Activar protección de rama en `main`:**
  - Requerir Pull Request para merge.
  - Requerir al menos 1 aprobación.
  - Requerir checks de CI en verde antes de merge.
  - Bloquear force-push y eliminación de rama.
- [ ] **Configurar roles y permisos:** propietario(s), mantenedores, colaboradores y acceso mínimo necesario.

## 2. Gestión de trabajo y planificación (prioridad alta)

- [ ] **Crear GitHub Project (Kanban/Roadmap)** con columnas: `Backlog`, `Ready`, `In Progress`, `Review`, `Done`.
- [ ] **Crear etiquetas (labels) estándar:**
  - Tipo: `feature`, `bug`, `docs`, `chore`, `research`, `security`
  - Área: `frontend`, `backend`, `ai-vision`, `payments`, `ux`, `devops`
  - Prioridad: `priority:high`, `priority:medium`, `priority:low`
  - Estado: `blocked`, `needs-info`, `good-first-issue`
- [ ] **Cargar issues iniciales del MVP** (épicas + tareas):
  - Medición de salto parado y con carrerilla + regla en cm
  - Registro/login y perfiles (jugador/entrenador/admin)
  - Verificación de entrenadores certificados por federación
  - Marketplace, contratación y pagos
  - Reseñas 0–5 estrellas post-servicio
  - Grabación/subida de vídeo y análisis IA con recomendaciones y ejemplos
  - Historial de progreso y métricas
- [ ] **Asignar responsables y fechas objetivo** (milestones) para cada fase del roadmap.
- [ ] **Definir plantilla de seguimiento semanal** (issue de reporte o discusión fijada).

## 3. Documentación y estándar del repositorio (prioridad alta)

- [ ] **Publicar README.md principal** (visión, funcionalidades, arquitectura, roadmap, puesta en marcha).
- [ ] **Añadir LICENSE** acorde a la estrategia (propietaria, MIT, Apache-2.0, etc.).
- [ ] **Crear CONTRIBUTING.md** con normas de ramas, commits, PRs y revisión.
- [ ] **Crear CODE_OF_CONDUCT.md** y `SECURITY.md` (reporte de vulnerabilidades y contacto).
- [ ] **Añadir plantillas en `.github/`:**
  - `ISSUE_TEMPLATE/bug_report.md`
  - `ISSUE_TEMPLATE/feature_request.md`
  - `ISSUE_TEMPLATE/task.md`
  - `PULL_REQUEST_TEMPLATE.md` con checklist (tests, docs, capturas, impacto)

## 4. Calidad, CI/CD y seguridad (prioridad media)

- [ ] **Configurar GitHub Actions** (workflows mínimos):
  - `ci.yml`: lint + tests + build en PR y push a `main`
  - `dependency-review` o escaneo de dependencias
- [ ] **Activar Dependabot** para actualizaciones de dependencias y alertas de seguridad.
- [ ] **Habilitar análisis de seguridad** (secret scanning, code scanning si aplica al stack).
- [ ] **Definir entornos** (`dev`, `staging`, `prod`) y reglas de despliegue cuando exista infraestructura.
- [ ] **Configurar versionado y releases:** convención de tags (`vX.Y.Z`), changelog y notas de release.

## 5. Producto y cumplimiento (prioridad media)

- [ ] **Documentar flujo de verificación de entrenadores certificados** (evidencia requerida, estados, revisión).
- [ ] **Definir política de reseñas 0–5 estrellas:** cuándo se habilitan, moderación, apelaciones y antifraude.
- [ ] **Redactar políticas de privacidad y consentimiento** para grabación y análisis de vídeo con IA.
- [ ] **Definir requisitos de pagos** (proveedor, comisiones, reembolsos, facturación) y responsabilidades.
- [ ] **Acordar KPIs iniciales:** precisión de medición, tiempo de análisis, conversión a contratación, NPS/valoración media.

## 6. Hitos sugeridos

| Hito | Entregable | Responsable | Fecha objetivo |
|---|---|---|---|
| M0 — Repositorio listo | Repo configurado, README, plantillas, protección de ramas | Dayron | ____/____/____ |
| M1 — Planificación MVP | Project, labels, issues y milestones cargados | Dayron | ____/____/____ |
| M2 — Base técnica | CI, estructura de carpetas y convenciones acordadas | Dayron + equipo técnico | ____/____/____ |
| M3 — MVP funcional | Medición + perfiles + flujo inicial de entrenador/reseña | Equipo | ____/____/____ |

---

## Criterio de finalización

- Repositorio con documentación completa, navegación clara y decisiones trazables.
- Trabajo gestionado por issues/project con prioridades y responsables definidos.
- Calidad automatizada (CI, revisiones, plantillas) y medidas básicas de seguridad activas.
- Alineación explícita entre producto descrito y backlog ejecutable.
