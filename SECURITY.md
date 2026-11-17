# Política de seguridad — Proyecto Aquiles

## Reporte de vulnerabilidades
No abras issues públicos para vulnerabilidades de seguridad.

- **Contacto:** security@<dominio-del-proyecto> (sustituir por el canal oficial)
- **Incluye:** descripción, impacto, pasos de reproducción, versión/commit afectado y, si es posible, mitigación propuesta.
- **Plazo objetivo de respuesta inicial:** 72 horas.

## Alcance sensible
- Autenticación, autorización y control de acceso.
- Pagos y datos de transacciones.
- Almacenamiento y tratamiento de vídeos/imágenes de usuarios.
- Exposición de datos personales o secretos.
- Integridad del análisis de vídeo y de las métricas de salto.

## Buenas prácticas requeridas
- Secretos solo en gestores seguros/variables de entorno, nunca en el repo.
- Dependencias actualizadas y alertas de seguridad atendidas.
- Revisión obligatoria para cambios en áreas sensibles (auth, pagos, IA/visión, datos).
