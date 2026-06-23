# Cronograma — FisioVital Digital

## Estimaciones recogidas del equipo
| Módulo/tarea | Responsable | Duración estimada | Depende de |
|---|---|---|---|
| Autenticación | Backend | 1 semana | Inicio del proyecto |
| Módulo Citas | Backend | 2 semanas | Autenticación |
| Módulo Pacientes/Historial | Backend | 2,5 semanas | Autenticación |
| Módulo Facturación | Backend | 3 semanas | Citas y Pacientes/Historial |
| Módulo Administración/Informes | Backend | 1,5 semanas | Citas, Pacientes, Facturación |
| Pantallas Autenticación | Frontend | 0,5 semana | Backend: Autenticación |
| Pantallas Citas | Frontend | 2 semanas | Backend: Citas + contrato API |
| Pantallas Pacientes/Historial | Frontend | 1,5 semanas | Backend: Pacientes/Historial |
| Pantallas Facturación | Frontend | 1,5 semanas | Backend: Facturación + contrato API |
| Panel Administración/Informes | Frontend | 1,5 semanas | Resto de módulos backend |
| Diseño plan de pruebas | QA | 1 semana | En paralelo, desde el inicio |
| Ejecución de pruebas por módulo | QA | 0,5 semana por módulo | Cierre de cada módulo |
| Regresión final | QA | 1 semana | Todos los módulos completos |
| Configuración de entornos | DevOps | 1 semana | Inicio del proyecto |
| Pipeline CI/CD | DevOps | 1 semana | Entornos configurados |
| Despliegue final y checklist | DevOps | 0,5 semana | Regresión final de QA |

```mermaid
gantt
    title Cronograma FisioVital Digital
    dateFormat YYYY-MM-DD
    axisFormat %d/%m
    section Planificación
    Definir alcance y EDT           :done, plan1, 2026-07-06, 5d
    section Backend
    Autenticación                   :back1, after plan1, 5d
    Módulo Citas                    :back2, after back1, 10d
    Módulo Pacientes/Historial      :back3, after back1, 12d
    Módulo Facturación              :back4, after back2 back3, 15d
    Módulo Administración/Informes  :back5, after back4, 7d
    section Frontend
    Pantallas Autenticación         :front1, after back1, 3d
    Pantallas Citas                 :front2, after back2, 10d
    Pantallas Pacientes/Historial   :front3, after back3, 7d
    Pantallas Facturación           :front4, after back4, 7d
    Panel Administración/Informes   :front5, after back5, 7d
    section QA
    Diseño plan de pruebas          :qa1, after plan1, 5d
    Pruebas Citas                   :qa2a, after back2, 3d
    Pruebas Pacientes/Historial     :qa2b, after back3, 3d
    Pruebas Facturación             :qa2c, after back4, 3d
    Pruebas Administración         :qa2d, after back5, 3d
    Regresión final                 :qa3, after front5, 5d
    section DevOps
    Entornos                        :dev1, after plan1, 5d
    Pipeline CI/CD                  :dev2, after dev1, 5d
    Despliegue final y checklist    :dev3, after qa3, 3d
    section Hitos
    Entrega final                   :milestone, m1, after dev3, 0d
```