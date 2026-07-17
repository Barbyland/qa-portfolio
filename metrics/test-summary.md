# Resumen de ejecución y métricas

## Resumen cuantitativo

| Métrica | Resultado |
|---|---:|
| Casos de prueba diseñados | 4 |
| Ciclos de ejecución | 2 |
| Ciclos finalizados | 2 (100 %) |
| Ejecuciones registradas | 8 |
| Defectos confirmados al cierre | 3 |
| Defectos abiertos después de la regresión | 3 |

## Sprint 1

- 4 casos ejecutados.
- 1 caso aprobado.
- 3 casos fallidos.
- Tasa de aprobación: 25 %.
- Defectos confirmados: BR-02, BR-03 y BR-04.

## Sprint 2

- Se reejecutaron los cuatro casos.
- Los ciclos quedaron finalizados al 100 % en Zephyr.
- Los defectos BR-02, BR-03 y BR-04 permanecieron abiertos.
- El historial de TC-01_F1 registra un cambio de PASSED a FAILED, considerado una señal de regresión o inestabilidad del entorno.

## Conclusiones

1. El flujo principal no estaba listo para aprobación debido a defectos bloqueantes en carga de CV, búsqueda y postulación.
2. La reejecución permitió comprobar que los defectos principales no habían sido corregidos.
3. El cambio de estado de TC-01_F1 justificaba una investigación adicional antes de cerrar el ciclo.
4. Se recomendó corregir los defectos, estabilizar el entorno y ejecutar nuevamente la suite completa.

## Evidencias relacionadas

- [Casos documentados en Zephyr](../evidence/zephyr-test-cases-overview.png)
- [Ciclos finalizados](../evidence/zephyr-test-cycles.png)
- [Backlog y defectos](../evidence/jira-backlog-bug-reports.png)
- [Historial de ejecución](../evidence/zephyr-execution-history.png)
