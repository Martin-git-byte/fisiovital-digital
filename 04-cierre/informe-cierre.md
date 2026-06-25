# Informe de cierre del proyecto

## Comparativa planificado vs. real
| Dimensión | Planificado | Real | Desviación |
|---|---|---|---|
| Alcance | 5 módulos (Autenticación, Citas, Pacientes/Historial, Facturación, Administración/Informes) | Los 5 módulos + recordatorios automáticos por email (CR-001) | Ampliación controlada vía control de cambios |
| Plazo | 12 semanas (entrega prevista) | 13 semanas | +1 semana (≈8%), principalmente por Facturación |
| Coste | 30.000 € | 31.500 € | +1.500 € (+5%), dentro del rango aprobado por el cliente (25.000€–35.000€) |

## Estado final de los riesgos (de 02-planificacion/riesgos.md)
| ID | Riesgo | ¿Se materializó? | Notas |
|---|---|---|---|
| R1 | Retraso en la definición del contrato de API | Parcialmente | Se gestionó a tiempo en la Sesión 2, evitó bloqueos mayores en Frontend |
| R2 | Integración con sistemas externos no contemplada | No | No surgió ninguna solicitud de este tipo durante el proyecto |
| R3 | Falta de datos de prueba o indisponibilidad del único QA | No | El plan de pruebas de Facturación se ejecutó sin incidentes de este tipo |
| R4 | Cobertura de pruebas insuficiente en Facturación | Sí, parcialmente | El módulo se retrasó (SPI 0,84 en semana 6) pero la priorización de pruebas evitó incidencias críticas en producción |
| R5 | Cambio de proveedor cloud o fallo de backups | No | Sin incidentes relacionados con proveedor o backups |
| R6 | Presupuesto insuficiente para entorno de pre-producción | No | Se mantuvieron los 3 entornos previstos sin recorte |
| R7 | Nuevos requisitos legales o funcionales ampliando el alcance | Sí | Se materializó como CR-001 (recordatorios automáticos), gestionado vía control de cambios |
| R8 | Cambios en RGPD o protección de datos sanitarios | No | Sin cambios normativos durante el proyecto |
| R9 | Resistencia al cambio del personal de recepción | Sí, parcialmente | Hubo errores iniciales de marcado de facturas de seguro, ligados a adaptación del personal; resueltos durante la ejecución |
| R10 | Indisponibilidad de personal clave del cliente | No | Marta y Ana estuvieron disponibles en todos los hitos de validación |
| R11 | Cambios de configuración sin validación previa en local | Sí | Se materializó como INC-001 (caída de pre-producción, 14h, sin pérdida de datos) |

## Entregables generados durante el proyecto
- Project Charter, acta de descubrimiento, registro de interesados y acta de kick-off (Sesión 1)
- EDT, ADR de arquitectura, cronograma, plan de riesgos, plan de comunicación/presupuesto y contrato de API (Sesión 2)
- Informe de seguimiento, CR-001, INC-001, plan de pruebas de Facturación y estrategia de despliegue (Sesión 3)
- Acta de aceptación final, informe de cierre, lecciones aprendidas y postmortem (Sesión 4)
- Repositorio en GitHub con historial completo de commits, 3 Pull Requests fusionados, Issues documentados y tags v1.0-inicio, v1.0-planificacion, v1.0-ejecucion

## Cierre administrativo/contractual
- Acta de aceptación firmada por Marta Sánchez, con aceptación condicionada al seguimiento de las facturas de seguro durante 3 meses.
- Desviación de coste (+1.500 €) y plazo (+1 semana) documentadas y justificadas en este informe, dentro del rango de presupuesto aprobado por el cliente.