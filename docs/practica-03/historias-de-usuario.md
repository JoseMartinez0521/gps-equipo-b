# Práctica 03 - Historias de usuario

## Criterio

Las historias se reconstruyen a partir de funciones observables en el
repositorio y de los controladores existentes.

Formato utilizado:

> Como [rol], quiero [acción], para [beneficio].

Cada historia incluye al menos dos criterios de aceptación y prioridad MoSCoW.

---

## HU-01 - Gestión de usuarios

**Como** Admin,  
**quiero** gestionar usuarios del sistema,  
**para** mantener actualizada la información de las personas que utilizan la plataforma.

**Vista:** relacionada con usuarios dentro de Vistas/modulos/  
**Controlador:** Controladores/usuariosC.php

**Criterios de aceptación:**
1. El sistema debe permitir consultar información de usuarios.
2. El sistema debe permitir realizar las operaciones disponibles para la gestión de usuarios.

**Prioridad:** Must

---

## HU-02 - Gestión de carreras

**Como** Admin,  
**quiero** administrar las carreras,  
**para** mantener actualizado el catálogo académico.

**Vista:** módulo de carreras dentro de Vistas/modulos/  
**Controlador:** Controladores/carrerasC.php

**Criterios de aceptación:**
1. Debe existir una opción para consultar carreras.
2. Deben existir operaciones para crear, actualizar y eliminar carreras cuando corresponda.

**Prioridad:** Must

---

## HU-03 - Gestión de materias

**Como** Admin,  
**quiero** administrar las materias,  
**para** mantener actualizado el catálogo académico.

**Vista:** módulo de materias dentro de Vistas/modulos/  
**Controlador:** Controladores/materiasC.php

**Criterios de aceptación:**
1. El sistema debe permitir consultar materias.
2. El sistema debe permitir realizar las operaciones de gestión disponibles.

**Prioridad:** Must

---

## HU-04 - Solicitud de residencia

**Como** Alumno,  
**quiero** gestionar mi solicitud de residencia,  
**para** iniciar y dar seguimiento al proceso correspondiente.

**Vista:** módulo de solicitud de residencia dentro de Vistas/modulos/  
**Controlador:** Controladores/SolicitudResidenciaC.php

**Criterios de aceptación:**
1. El alumno debe poder acceder a las funciones relacionadas con su solicitud.
2. La información enviada debe ser procesada por el controlador correspondiente.

**Prioridad:** Must

---

## HU-05 - Información de residencia

**Como** Alumno,  
**quiero** consultar la información relacionada con mi residencia,  
**para** conocer el estado y los datos de mi proceso.

**Vista:** módulo relacionado con información de residencia dentro de Vistas/modulos/  
**Controlador:** Controladores/infoResidenciaC.php

**Criterios de aceptación:**
1. El sistema debe mostrar la información disponible del proceso.
2. La información debe ser obtenida mediante el controlador correspondiente.

**Prioridad:** Must

---

## HU-06 - Documentos

**Como** Alumno,  
**quiero** gestionar los documentos de mi proceso,  
**para** mantener organizada la documentación requerida.

**Vista:** módulo de documentos dentro de Vistas/modulos/  
**Controlador:** Controladores/documentosEcenC.php

**Criterios de aceptación:**
1. El sistema debe permitir acceder a las funciones disponibles para documentos.
2. Las operaciones deben pasar por el controlador correspondiente.

**Prioridad:** Must

---

## HU-07 - Evaluaciones

**Como** asesor,  
**quiero** gestionar las evaluaciones relacionadas con los alumnos,  
**para** registrar el seguimiento académico correspondiente.

**Vista:** módulo de evaluaciones dentro de Vistas/modulos/  
**Controlador:** Controladores/evaluacionesC.php

**Criterios de aceptación:**
1. El asesor debe poder acceder a las funciones de evaluación disponibles.
2. La información debe procesarse mediante el controlador de evaluaciones.

**Prioridad:** Should

---

## HU-08 - Visitas

**Como** asesor,  
**quiero** registrar o consultar las visitas relacionadas con las residencias,  
**para** dar seguimiento al proceso en la empresa.

**Vista:** módulo de visitas dentro de Vistas/modulos/  
**Controlador:** Controladores/visitasC.php

**Criterios de aceptación:**
1. El sistema debe proporcionar las funciones disponibles para registrar o consultar visitas.
2. Las operaciones deben ser procesadas por isitasC.php.

**Prioridad:** Should

---

## HU-09 - Constancias

**Como** usuario autorizado,  
**quiero** generar constancias,  
**para** obtener un documento relacionado con el proceso.

**Vista:** módulo correspondiente a constancias dentro de Vistas/modulos/  
**Controlador:** Controladores/ConstanciaC.php

**Criterios de aceptación:**
1. El sistema debe permitir acceder a la generación de constancias disponible.
2. La generación debe ser procesada por el controlador de constancias.

**Prioridad:** Should

---

## HU-10 - Chat

**Como** usuario del sistema,  
**quiero** utilizar el chat disponible,  
**para** comunicarme mediante la funcionalidad proporcionada por la plataforma.

**Vista:** módulo de chat dentro de Vistas/modulos/  
**Controlador:** Controladores/ChatC.php

**Criterios de aceptación:**
1. El usuario debe poder acceder a la funcionalidad de chat disponible.
2. Las operaciones deben ser procesadas por ChatC.php.

**Prioridad:** Could

---

## HU-11 - Ajustes

**Como** Admin,  
**quiero** administrar los ajustes disponibles del sistema,  
**para** mantener configuradas las opciones correspondientes.

**Vista:** módulo de ajustes dentro de Vistas/modulos/  
**Controlador:** Controladores/ajustesC.php

**Criterios de aceptación:**
1. El administrador debe poder acceder a las funciones de ajustes disponibles.
2. Las operaciones deben ser procesadas por el controlador correspondiente.

**Prioridad:** Should

---

## HU-12 - Plantilla y navegación

**Como** usuario,  
**quiero** visualizar el menú correspondiente a mi rol,  
**para** acceder únicamente a las funciones disponibles para mi tipo de usuario.

**Vista:** Vistas/plantilla.php  
**Controlador:** Controladores/plantillaControlador.php

**Criterios de aceptación:**
1. El sistema debe cargar la plantilla principal.
2. El menú mostrado debe depender del rol identificado por el sistema.

**Prioridad:** Must

---

## Resumen MoSCoW

| Prioridad | Historias |
|---|---|
| Must | HU-01, HU-02, HU-03, HU-04, HU-05, HU-06, HU-12 |
| Should | HU-07, HU-08, HU-09, HU-11 |
| Could | HU-10 |
| Won't | No se definieron funciones como Won't porque no existe evidencia suficiente en esta etapa para afirmar que una función concreta será descartada. |

> Nota: las historias deben validarse contra el funcionamiento real del sistema si el docente proporciona una instalación funcionando.
