# Guion de presentación final

## 1. Resumen del proyecto (1 min)
FisioVital Digital es un sistema de gestión documental para 5 clínicas de fisioterapia, desarrollado en 13 semanas bajo el curso IFCT055PO. Cubre autenticación, citas, historial clínico, facturación mixta (particular/seguro) y administración/informes, con arquitectura monolítica modular. El proyecto se cerró con una semana de retraso y un 5% sobre presupuesto, ambos justificados y documentados.

## 2. Recorrido por el repositorio (3 min)
- **Commits destacados:** desde el primer README (Sesión 1) hasta el postmortem (Sesión 4), con mensajes descriptivos siguiendo convención `docs(fase): descripción`.
- **Pull Requests fusionados:** Sesión 2 (#4), Sesión 3 (#7) y Sesión 4, cada uno integrando una rama de trabajo dedicada a `main`.
- **Issues cerrados:** #5 (INC-001) y #6 (CR-001), gestionados durante la ejecución; #1, #2 y #3 (riesgos) documentados y monitorizados durante todo el proyecto.
- **Tags:** v1.0-inicio, v1.0-planificacion, v1.0-ejecucion, v1.0.0.

## 3. Decisiones clave (2 min)
- ADR 001: arquitectura monolítica modular, elegida por el tamaño del equipo y el plazo ajustado, frente a microservicios o un monolito no modular.
- CR-001: aceptación de recordatorios automáticos solo por email, descartando SMS por su coste recurrente fuera de presupuesto.
- Respuesta a INC-001: reversión inmediata de la configuración y, después, incorporación de una regla obligatoria de validación previa en local antes de tocar pre-producción.

## 4. Lecciones aprendidas (2 min)
- El contrato de API debería cerrarse como primer entregable de la planificación, no como último ejercicio, para evitar bloqueos en cascada sobre Frontend.
- La complejidad de módulos como Facturación necesita una validación técnica más profunda antes de comprometer duraciones en el cronograma.
- La gestión de cambios de configuración sin proceso formal fue la causa raíz de INC-001; ya quedó incorporada como regla permanente del pipeline.

## 5. Cierre (1 min)
FisioVital Digital queda entregado y aceptado por la clienta, con una condición de seguimiento de 3 meses sobre el marcado de facturas de seguro. El proyecto completo —desde el Project Charter hasta este postmortem— queda documentado y trazable en el repositorio de GitHub.