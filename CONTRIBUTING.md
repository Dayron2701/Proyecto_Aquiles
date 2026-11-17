# Guía de contribución — Proyecto Aquiles

## Flujo de trabajo
1. **Issue primero:** toda tarea o cambio relevante debe tener un issue enlazado.
2. **Ramas:**
   - `feature/<descripcion-corta>` para nuevas funcionalidades
   - `fix/<descripcion-corta>` para correcciones
   - `docs/<descripcion-corta>` para documentación
   - `chore/<descripcion-corta>` para tareas de mantenimiento
3. **Commits:** claros y atómicos. Recomendado: Conventional Commits (`feat:`, `fix:`, `docs:`, `chore:`).
4. **Pull Request:** abrir PR hacia `main` con descripción, evidencia (capturas/tests) y checklist completado.
5. **Revisión:** mínimo 1 aprobación y checks de CI en verde antes de merge.

## Estándares mínimos
- Código con lint y tests pasando.
- Documentación actualizada cuando el cambio lo requiera.
- Sin secretos, credenciales ni datos sensibles en el repositorio.
- Cambios en medición/IA con notas sobre impacto en precisión y validación.

## Reporte de bugs y propuestas
Usar las plantillas de Issues en `.github/ISSUE_TEMPLATE/` e incluir contexto, pasos de reproducción y resultado esperado.
