# INC-001 — Caída del entorno de pre-producción

## Fecha y detección
Caída ocurrida durante la noche del 02/08/2026. Detectada al intentar acceder QA al entorno de pre-producción esta mañana para ejecutar las pruebas programadas.

## Descripción
El entorno de pre-producción quedó inaccesible durante aproximadamente 14 horas. La aplicación no llegó a arrancar tras el incidente.

## Impacto
- Acceso al entorno caído ~14 horas.
- QA no pudo ejecutar las pruebas programadas para el día de ayer; se perdió un día completo de pruebas.
- No hubo pérdida de datos.

## Causa raíz (preliminar)
Se modificó una variable de entorno de conexión a la base de datos sin probarla previamente en local, lo que impidió que la aplicación arrancara correctamente.

## Acción de contingencia
Se revirtió la variable de entorno a su configuración anterior, restableciendo el acceso. Se perdió un día completo de pruebas de QA, que deberá reprogramarse.

## Issue relacionado
#5