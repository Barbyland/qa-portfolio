# Casos de prueba y resultados

## TC-01_F1 - Registro exitoso de persona usuaria

**Objetivo:** validar que el sistema permita registrar una nueva cuenta con datos válidos.<br>
**Precondición:** la persona no posee una cuenta registrada.<br>
**Datos:** correo válido y contraseña que cumpla la política definida.

### Pasos

1. Ingresar al portal TalentoLab.
2. Abrir la opción de registro.
3. Completar correo y contraseña válidos.
4. Enviar el formulario.

**Resultado esperado:** la cuenta se crea y aparece una confirmación de registro exitoso.<br>
**Sprint 1:** PASSED.<br>
**Sprint 2:** FAILED según el historial de reejecución registrado en Zephyr.

---

## TC-02_F1 - Carga exitosa de CV en PDF

**Objetivo:** comprobar que el sistema acepte un archivo PDF válido.<br>
**Precondición:** persona registrada, con sesión iniciada y acceso a su perfil.<br>
**Datos:** archivo PDF válido dentro del límite permitido.

### Pasos

1. Ingresar al perfil.
2. Seleccionar la opción para cargar el CV.
3. Adjuntar un archivo PDF válido.
4. Confirmar la carga.

**Resultado esperado:** el sistema acepta el archivo y confirma la carga.<br>
**Resultado obtenido:** el sistema rechaza el PDF válido y muestra `Formato inválido`.<br>
**Sprint 1:** FAILED.<br>
**Sprint 2:** FAILED.<br>
**Defecto asociado:** BR-02.

---

## TC-03_F1 - Búsqueda de empleos por palabra clave

**Objetivo:** validar que la búsqueda muestre vacantes relacionadas con la palabra ingresada.<br>
**Precondición:** persona con sesión iniciada y acceso al listado de empleos.<br>
**Dato:** palabra clave `QA`.

### Pasos

1. Abrir la sección de empleos.
2. Ingresar `QA` en el buscador.
3. Ejecutar la búsqueda.
4. Revisar los resultados.

**Resultado esperado:** se muestran vacantes relacionadas con QA.<br>
**Resultado obtenido:** la búsqueda devuelve cero resultados aunque existen vacantes relacionadas.<br>
**Sprint 1:** FAILED.<br>
**Sprint 2:** FAILED.<br>
**Defecto asociado:** BR-03.

---

## TC-04_F1 - Postulación desde la ficha de empleo

**Objetivo:** comprobar que una persona pueda postularse correctamente desde una vacante.<br>
**Precondición:** sesión iniciada, perfil disponible y CV cargado.<br>

### Pasos

1. Abrir una vacante.
2. Seleccionar la opción de postulación.
3. Confirmar la acción.
4. Verificar el estado final.

**Resultado esperado:** el sistema confirma el envío de la postulación.<br>
**Resultado obtenido:** la postulación permanece en estado `Pendiente...` y no se confirma el envío.<br>
**Sprint 1:** FAILED.<br>
**Sprint 2:** FAILED.<br>
**Defecto asociado:** BR-04.

## Trazabilidad resumida

| Caso | Funcionalidad | Sprint 1 | Sprint 2 | Defecto |
|---|---|---:|---:|---|
| TC-01_F1 | Registro | PASSED | FAILED | Sin defecto confirmado en el informe final |
| TC-02_F1 | Carga de CV | FAILED | FAILED | BR-02 |
| TC-03_F1 | Búsqueda | FAILED | FAILED | BR-03 |
| TC-04_F1 | Postulación | FAILED | FAILED | BR-04 |
