# Plan de pruebas — Módulo Facturación

## Alcance
Basado en el contrato 02-planificacion/api/openapi.yaml: endpoints /facturas,
/facturas/{id} y /facturas/{id}/pagar.

## Tipos de prueba
- Funcional
- Integración
- Regresión
- Aceptación

## Casos de prueba
| ID | Caso | Endpoint | Resultado esperado |
|---|---|---|---|
| TC01 | Crear factura particular | POST /facturas | 201 Created |
| TC02 | Crear factura con seguro | POST /facturas | 201 Created |
| TC03 | Crear factura con importe 0 o negativo | POST /facturas | 400 Bad Request |
| TC04 | Crear factura de tipo "seguro" sin paciente con seguro asociado | POST /facturas | 400 Bad Request |
| TC05 | Crear factura de una cita que no existe | POST /facturas | 404 Not Found |
| TC06 | Marcar como pagada una factura pendiente | PATCH /facturas/{id}/pagar | 200 OK |
| TC07 | Marcar como pagada una factura que ya está pagada | PATCH /facturas/{id}/pagar | 409 Conflict (o 400, a confirmar con Backend) |
| TC08 | Listar facturas cuando no hay ninguna creada | GET /facturas | 200 OK, lista vacía |
| TC09 | Obtener el detalle de una factura inexistente | GET /facturas/{id} | 404 Not Found |

## Criterios de salida a producción
- 100% de los casos de prueba ejecutados, sin bloqueantes abiertos.
- Cero incidencias críticas o de alta severidad sin resolver en el módulo de Facturación.
- Validado el caso de doble pago (TC07) antes de cualquier despliegue a producción, dado que afecta directamente a la facturación real del cliente.