# Acta de kick-off interno

## Dudas/riesgos planteados por el equipo
- **Frontend:** Necesita conocer la guía de marca/colores corporativos de FisioVital antes de diseñar, y si las recepcionistas usarán tablet, ordenador o ambos. Advierte que el trabajo de interfaz se va a frenar si no se define pronto qué datos entregará el backend para citas y pacientes (riesgo de dependencia del contrato de API se retoma en la Sesión 2, Ejercicio 2.6).
- **Backend:** El historial clínico es un dato de salud, considerado categoría especial bajo protección de datos, por lo que necesita el alcance bien definido antes de diseñar el modelo de datos. La facturación con dos modalidades (particular y seguro) no es trivial y llevará tiempo. Coincide con Frontend en la urgencia de definir el contrato de la API cuanto antes.
- **QA:** Con un plazo de 3 meses, teme que solo dé tiempo a probar los casos "felices" y se cuelen errores justo en facturación, el módulo más delicado. Necesita definir cómo simular los pagos por seguro sin acceso real al sistema de la aseguradora. Pide criterios de aceptación claros y tempranos por módulo para poder preparar el plan de pruebas.
- **DevOps:** Al manejar datos de salud, el alojamiento debe estar obligatoriamente dentro de la Unión Europea (RGPD), y se necesita una política de copias de seguridad clara desde el inicio. Plantea que el presupuesto ajustado obliga a decidir pronto cuántos entornos se podrán mantener (¿solo desarrollo y producción, o también pre-producción?).

## Matriz RACI inicial (alto nivel)
| Actividad | Jefe de Proyecto | Frontend | Backend | QA | DevOps |
|---|---|---|---|---|---|
| Definir alcance | R/A | C | C | C | C |
| Diseño de interfaz | I | R/A | C | C | I |
| Lógica de negocio y datos | I | C | R/A | C | C |
| Pruebas | I | C | C | R/A | C |
| Despliegue | I | I | C | C | R/A |

*(R = Responsable, A = Aprobador, C = Consultado, I = Informado)*