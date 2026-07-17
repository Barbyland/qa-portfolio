# Reportes de defectos

La severidad y la prioridad se normalizaron para esta versión del portfolio según el impacto funcional observado en el informe final.

## BR-02 - El sistema rechaza un CV en PDF válido

| Campo | Detalle |
|---|---|
| Tipo | Defecto funcional |
| Severidad | Alta |
| Prioridad | Alta |
| Estado al cierre | Abierto |
| Caso asociado | TC-02_F1 |

### Pasos para reproducir

1. Iniciar sesión con una cuenta válida.
2. Abrir la sección de perfil.
3. Seleccionar la opción para cargar un CV.
4. Adjuntar un archivo PDF válido dentro del límite permitido.
5. Confirmar la carga.

**Resultado esperado:** el archivo se carga y el sistema muestra una confirmación.<br>
**Resultado obtenido:** el sistema rechaza el archivo y muestra `Formato inválido`.

---

## BR-03 - La búsqueda por QA no devuelve vacantes existentes

| Campo | Detalle |
|---|---|
| Tipo | Defecto funcional |
| Severidad | Alta |
| Prioridad | Alta |
| Estado al cierre | Abierto |
| Caso asociado | TC-03_F1 |

### Pasos para reproducir

1. Iniciar sesión.
2. Abrir la sección de empleos.
3. Ingresar `QA` en el buscador.
4. Ejecutar la búsqueda.

**Resultado esperado:** se muestran las vacantes relacionadas con QA.<br>
**Resultado obtenido:** el sistema devuelve cero resultados aunque existen vacantes coincidentes.

---

## BR-04 - La postulación no confirma el envío

| Campo | Detalle |
|---|---|
| Tipo | Defecto funcional |
| Severidad | Alta |
| Prioridad | Alta |
| Estado al cierre | Abierto |
| Caso asociado | TC-04_F1 |

### Pasos para reproducir

1. Iniciar sesión con una cuenta que tenga un CV cargado.
2. Abrir una vacante disponible.
3. Seleccionar la opción para postularse.
4. Confirmar la acción.

**Resultado esperado:** el sistema confirma que la postulación fue enviada.<br>
**Resultado obtenido:** la operación queda en estado `Pendiente...` y no aparece la confirmación.

## Estado al finalizar

Los defectos BR-02, BR-03 y BR-04 continuaban abiertos después del segundo ciclo de ejecución.
