# Proyecto Aquiles

Plataforma para medir el salto vertical, conectar jugadores con entrenadores certificados y mejorar el rendimiento deportivo mediante análisis de vídeo con IA.

> **Objetivo del repositorio:** ofrecer una base de producto y documentación con estándar profesional, clara para desarrollo, despliegue y evaluación.

---

## Visión general

**Proyecto Aquiles** es una aplicación orientada a deportistas de todos los niveles que combina medición objetiva del salto, formación guiada y feedback inteligente. La aplicación permite:

- Medir la altura de salto en **centímetros** en dos modalidades: **salto parado** y **salto con carrerilla**.
- Visualizar una **referencia/regla digital** sobre la captura para mostrar los cm alcanzados de forma clara y comparable.
- Acceder a un espacio de **aprendizaje y mejora** con recursos y seguimiento.
- Conectar **jugadores** con **entrenadores certificados por la federación** mediante un servicio de pago dentro de la plataforma.
- Evaluar el servicio con **reseñas de 0 a 5 estrellas** tras su uso.
- Grabar vídeo y recibir un **análisis por IA** con puntos de mejora, recomendaciones prácticas y ejemplos de ejecución correcta.

---

## Funcionalidades principales

### 1. Medición de salto
- **Modalidades:** salto parado (Squat Jump/CMJ según configuración) y salto con carrerilla.
- **Salida:** altura estimada en centímetros con visualización de regla/escala.
- **Historial:** registro de intentos para comparar progreso en el tiempo.
- **Calidad de captura:** guías para encuadre, distancia y condiciones de luz para mejorar la precisión.

### 2. Aprendizaje y mejora
- Biblioteca de contenidos por nivel (iniciación, intermedio, avanzado).
- Planes y rutinas orientadas a mejorar potencia, técnica y consistencia.
- Seguimiento de objetivos y evolución del deportista.

### 3. Marketplace de entrenadores certificados
- Perfiles de entrenadores con **certificación federativa verificable**.
- Búsqueda y filtrado por disciplina, nivel, disponibilidad e idioma.
- Contratación del servicio desde la aplicación (flujo de compra integrado).
- **Reseñas y valoración:** sistema de 0 a 5 estrellas disponible tras completar/probar el servicio.
- Políticas de calidad, moderación de reseñas y resolución de incidencias.

### 4. Análisis de vídeo con IA
- **Grabación/subida de vídeo** del gesto o ejercicio.
- **Detección de aspectos mejorables** (técnica, postura, fase de impulso/aterrizaje, ritmo, etc.).
- **Recomendaciones personalizadas** y priorizadas.
- **Ejemplos de referencia** (clips o guías visuales) que muestran cómo ejecutar correctamente el movimiento.
- Comparativa antes/después para seguimiento de mejora.

---

## Público objetivo

- Jugadores que quieren medir y mejorar su salto.
- Deportistas que buscan entrenamiento guiado y feedback continuo.
- Entrenadores certificados que desean ofrecer servicios y construir reputación mediante reseñas verificadas.
- Clubes y academias interesadas en seguimiento objetivo del rendimiento.

---

## Arquitectura propuesta (alto nivel)

> Ajustar según el stack definitivo del proyecto.

| Capa | Responsabilidad | Tecnologías sugeridas |
|---|---|---|
| Cliente (App/Web) | Captura de vídeo, UI de medición, perfiles, pagos y reseñas | Flutter / React Native / React |
| Backend/API | Autenticación, lógica de negocio, pagos, gestión de usuarios y reservas | Node.js (NestJS) / Python (FastAPI) |
| Visión por computador | Estimación de salto, calibración de escala/regla, extracción de métricas | OpenCV, MediaPipe, modelos propios |
| IA de análisis | Feedback técnico, detección de errores y recomendaciones | Modelos de pose/acción + LLM para explicaciones |
| Datos | Usuarios, sesiones, métricas, reseñas, transacciones | PostgreSQL + almacenamiento de objetos (S3 compatible) |
| Infra/DevOps | CI/CD, entornos, observabilidad y seguridad | GitHub Actions, Docker, monitorización |

---

---

## Puesta en marcha (plantilla)

### Requisitos previos
- Git
- Runtime del stack elegido (Node.js / Python / Flutter, etc.)
- Gestor de dependencias correspondiente
- Variables de entorno configuradas (`.env`)

### Instalación
```bash
# Clonar repositorio
git clone https://github.com/<organizacion>/proyecto_aquiles.git
cd proyecto_aquiles

# Instalar dependencias (ejemplo)
# npm install
# pip install -r requirements.txt
```

### Ejecución en desarrollo
```bash
# Ejemplo: levantar servicios
# npm run dev
# uvicorn app.main:app --reload
```

### Pruebas y calidad
```bash
# Lint
# npm run lint

# Tests
# npm test
```

---

## Modelo de datos (entidades clave)

- **Usuario:** jugador, entrenador, administrador; perfil, credenciales, estado.
- **Entrenador:** certificación federativa, especialidades, disponibilidad, tarifa.
- **Sesión de salto:** modalidad, vídeo/captura, altura en cm, fecha, metadatos.
- **Análisis IA:** hallazgos, recomendaciones, ejemplos sugeridos, puntuación técnica.
- **Servicio contratado:** reserva, pago, estado, relación jugador-entrenador.
- **Reseña:** autor, entrenador/servicio, puntuación (0–5), comentario, fecha.

---

## Seguridad, privacidad y cumplimiento

- **Consentimiento y privacidad:** tratamiento explícito de vídeos e imágenes de usuarios.
- **Protección de datos:** cifrado en tránsito y en reposo, control de accesos por rol.
- **Verificación de entrenadores:** validación de certificación federativa antes de publicar perfil.
- **Pagos:** integración con proveedor PCI-compliant; no almacenar datos sensibles de tarjeta en servidores propios.
- **Moderación:** políticas para reseñas, reporte de abuso y gestión de disputas.

---

## Roadmap inicial

- [ ] MVP de medición de salto (parado y carrerilla) con regla en cm
- [ ] Registro de usuarios y perfiles de jugador/entrenador
- [ ] Verificación de certificación federativa
- [ ] Flujo de contratación y pagos
- [ ] Sistema de reseñas 0–5 estrellas post-servicio
- [ ] Pipeline de análisis de vídeo con IA y ejemplos de corrección
- [ ] Panel de métricas y progreso
- [ ] Endurecimiento de seguridad, observabilidad y escalado

---

## Contribución

1. Crear rama desde `main` (`feature/`, `fix/`, `docs/`).
2. Abrir issue o enlazar tarea existente.
3. Commits claros y atómicos.
4. Pull Request con descripción, evidencia (capturas/tests) y checklist completado.
5. Revisión por al menos un responsable antes de merge.

Ver [TASKS.md](TASKS.md) para tareas asignadas y prioridades.

---

## Licencia

Definir licencia del proyecto en `LICENSE` (por ejemplo, MIT, Apache-2.0 o privada según estrategia comercial).

---

## Contacto y gobierno del proyecto

- **CEO / Responsable de producto:** Dayron
- **Repositorio:** `proyecto_aquiles`
- **Estado:** en definición / desarrollo inicial

Para dudas de producto, alcance o prioridades, abrir un issue con la etiqueta `product` o `question`.
