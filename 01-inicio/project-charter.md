# Project Charter — FisioVital Digital

## 1. Justificación del proyecto
FisioVital gestiona actualmente sus 5 clínicas con un sistema basado en Excel cuyo contrato de soporte vence en 3 meses y no será renovado. Esto obliga a sustituirlo por un sistema de gestión documental propio que reduzca errores operativos (citas duplicadas), permita una facturación correcta entre pacientes particulares y de seguro, y dé visibilidad sobre la ocupación de cada clínica.

## 2. Objetivos SMART
- Implementar un sistema web (accesible desde navegador, sin app móvil) que cubra agenda, fichas de pacientes y facturación, operativo en las 5 clínicas antes del 22/09/2026, dentro de un presupuesto de 25.000€–35.000€.
- Reducir a 0 los errores de citas duplicadas durante el primer mes de uso post-lanzamiento.
- Habilitar la generación de un informe de ocupación por clínica disponible a demanda desde el primer día de uso.
- Garantizar el cumplimiento de protección de datos (RGPD) en el manejo de historiales clínicos desde el diseño inicial del sistema.

## 3. Alcance de alto nivel
**Incluye:**
- Gestión de agenda de citas (5 clínicas)
- Fichas de pacientes (historial clínico)
- Facturación, diferenciando paciente particular y de seguro
- Informe de ocupación por clínica
- Acceso vía navegador desde ordenador y tablet de recepción
- Cumplimiento de protección de datos (historiales clínicos)

**No incluye:**
- App móvil nativa
- Pagos online (se evalúa para una fase posterior)
- Mantenimiento/soporte post-lanzamiento (a definir en contrato aparte)

## 4. Hitos principales
| Hito | Fecha estimada |
|---|---|
| Cierre de planificación y diseño | 06/07/2026 |
| Entrega de MVP (agenda + fichas de pacientes) | 05/08/2026 |
| Entrega de facturación e informes de ocupación | 05/09/2026 |
| Despliegue y cierre del proyecto | 22/09/2026 |

## 5. Presupuesto estimado de alto nivel
Entre 25.000 € y 35.000 €, sin incluir mantenimiento posterior al lanzamiento.

## 6. Riesgos de alto nivel
- Resistencia al cambio en parte del personal de recepción, con ~20 años trabajando en papel.
- Riesgo de incumplimiento de protección de datos al migrar historiales clínicos (RGPD).
- Plazo fijo e improrrogable (vencimiento del contrato actual), sin margen de extensión.
- Alcance de "mantenimiento posterior" aún sin definir, riesgo de expectativas distintas con el cliente.

## 7. Jefe de proyecto y autoridad
Martín Contrera — autoridad para: definir prioridades dentro del alcance aprobado, coordinar al equipo (Frontend, Backend, QA, DevOps), y escalar a Marta Sánchez cualquier cambio de presupuesto, plazo o alcance.

## 8. Criterios de éxito y aceptación
- Cero (o mínimas) citas duplicadas tras el lanzamiento.
- Facturación sin errores entre pacientes particulares y de seguro.
- Informe de ocupación por clínica disponible a demanda.
- Adopción efectiva por parte del personal de recepción, con acompañamiento en la transición.