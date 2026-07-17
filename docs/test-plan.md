# Plan de pruebas - TalentoLab

## 1. Objetivo

Validar el flujo principal de postulaciones del portal TalentoLab y comprobar que una persona usuaria pueda registrarse, cargar su CV, buscar oportunidades y postularse correctamente.

## 2. Alcance

### Incluido

- Registro de personas usuarias.
- Carga de CV en formato PDF.
- Búsqueda de vacantes por palabra clave.
- Postulación desde la ficha de empleo.
- Reejecución de casos para verificar regresión.
- Registro y seguimiento de defectos.

### Fuera de alcance

- Pruebas de carga y rendimiento.
- Pruebas de penetración o seguridad avanzada.
- Automatización de pruebas.
- Validaciones sobre datos o servicios de producción.
- Compatibilidad exhaustiva entre navegadores y dispositivos.

## 3. Estrategia

Se aplicó testing funcional basado en requerimientos y criterios de aceptación. Los casos fueron diseñados y administrados en Zephyr, mientras que las historias, tareas y defectos se gestionaron en Jira.

La ejecución se organizó en dos ciclos:

1. **Sprint 1:** validación inicial del flujo y detección de defectos.
2. **Sprint 2:** reejecución de los mismos casos para evaluar regresión y verificar si los defectos habían sido corregidos.

## 4. Criterios de entrada

- Entorno de TalentoLab disponible.
- Requerimientos y criterios de aceptación definidos.
- Casos de prueba revisados y aprobados en Zephyr.
- Datos de prueba preparados.
- Acceso a Jira y Zephyr.

## 5. Criterios de salida

- Todos los casos planificados ejecutados en cada ciclo.
- Resultados y evidencias registrados.
- Defectos encontrados documentados y vinculados.
- Ciclos de prueba finalizados en Zephyr.
- Resumen de resultados elaborado.

## 6. Riesgos principales

| Riesgo | Impacto | Mitigación |
|---|---|---|
| Entorno de práctica inestable | Resultados no reproducibles | Registrar fecha, evidencia y resultado de cada ejecución |
| Datos de prueba inconsistentes | Falsos fallos | Definir datos y precondiciones en cada caso |
| Cambios durante el sprint | Regresiones | Reejecutar el conjunto completo en el segundo ciclo |
| Falta de trazabilidad | Defectos sin relación con los casos | Vincular ejecuciones, incidencias y ciclos en Jira/Zephyr |

## 7. Entregables

- Casos de prueba funcionales.
- Resultados de Sprint 1 y Sprint 2.
- Reportes de defectos.
- Evidencias visuales de Jira y Zephyr.
- Resumen de ejecución y métricas.
