# Chatbot de Orientación Juvenil

### Propuesta de vinculación interdisciplinaria para liberación de Servicio Social

**Unidad responsable:** Centro Comunitario de Desarrollo Integral para las Juventudes
**Institución promotora:** Instituto Quintanarroense de la Juventud (IQJ)
**Instituciones académicas vinculadas:** Universidad del Caribe (UCaribe) y demás IES de la región con programas afines a STEM
**Municipio:** Benito Juárez, Cancún
**Proyectos relacionados:** [[Sistema de Gestión de Datos del Centro]] — puede compartir base de datos/backend
**Estatus del documento:** Borrador para revisión — completar campos marcados como `[pendiente]`

---

## 1. Datos generales del programa

| Campo | Información |
|---|---|
| Proyecto / programa | Chatbot de Orientación Juvenil |
| Responsable del programa | `[pendiente]` |
| Nombre del supervisor | `[pendiente]` |
| Puesto del supervisor | `[pendiente]` |
| Correo electrónico | `[pendiente]` |
| Vigencia del programa | Inicio: `[pendiente]` — Término: `[pendiente]` |
| Municipio | Benito Juárez, Cancún |
| Sede | Centro Comunitario de Desarrollo Integral para las Juventudes |

---

## 2. Justificación

Los jóvenes que se acercan al IQJ y al Centro Comunitario no siempre conocen la oferta completa de programas disponibles: becas, servicio social, talleres STEM, orientación laboral, salud, deporte y cultura. Gran parte de esas dudas son repetitivas y consumen tiempo del personal del Centro que podría dedicarse a atención más especializada.

Un chatbot de orientación juvenil, disponible por WhatsApp o en el sitio web del IQJ, permite:

- Responder preguntas frecuentes las 24 horas, sin depender de que haya personal disponible.
- Servir como puerta de entrada digital hacia los demás programas del Centro (incluyendo el huerto, el diagnóstico juvenil y el propio sistema de gestión de datos).
- Reducir la carga de atención repetitiva del personal, dejando más tiempo para casos que requieren trato humano.
- Dar a los prestadores de servicio social de Inteligencia Artificial y Datos un caso de uso real y acotado para practicar su carrera.

---

## 3. Objetivo general

Diseñar, desarrollar e implementar un chatbot de orientación juvenil que informe y canalice a los jóvenes hacia los programas y servicios del IQJ / Centro Comunitario, desarrollado y mantenido por prestadores de servicio social de ingeniería.

## 4. Objetivos específicos

1. Mapear los programas, requisitos y trámites del IQJ que serán cubiertos por el chatbot.
2. Diseñar el flujo conversacional y la base de conocimiento (preguntas frecuentes, categorías, respuestas).
3. Desarrollar el motor del chatbot (reglas + clasificación básica de intención) y su canal de acceso (WhatsApp y/o widget web).
4. Integrar un panel de administración con estadísticas de uso y preguntas no resueltas.
5. Establecer el proceso de actualización y mantenimiento de contenido.
6. Definir el protocolo de privacidad y manejo de datos, considerando que gran parte de los usuarios son menores de edad.
7. Generar el mecanismo documental que permita a los estudiantes acreditar horas de servicio social.

---

## 5. Marco institucional

| Actor | Rol en el proyecto |
|---|---|
| IQJ – Centro Comunitario | Sede del proyecto, validación de contenido oficial, supervisión |
| Universidad del Caribe | Fuente de prestadores de servicio social, validación académica de horas |
| Coordinaciones de IA, Datos, Industrial y Logística | Asignación de estudiantes, revisión técnica de entregables |
| Personal de atención del Centro | Usuario final del panel de administración, punto de escalación humana |

---

## 6. Descripción general / Arquitectura conceptual

- **Canal de entrada:** WhatsApp (API oficial o herramienta de bajo costo) y/o widget de chat en el sitio del IQJ.
- **Motor conversacional:** basado en reglas + clasificación de intención (no requiere un modelo de lenguaje complejo para la primera versión).
- **Base de conocimiento:** catálogo estructurado de preguntas frecuentes por categoría (programas, requisitos, fechas, contacto, servicio social, becas, talleres).
- **Panel de administración:** listado de preguntas más frecuentes, tasa de resolución automática, preguntas sin respuesta (para retroalimentar la base de conocimiento).
- **Escalación humana:** cuando el chatbot no puede resolver una consulta, deriva al usuario a un contacto o agenda de cita con el Centro.

---

## 7. Participación por ingeniería

### 7.1 Ingeniería en Inteligencia Artificial
**Rol:** núcleo conversacional del chatbot.

- Diseño de intents (intenciones), entidades y flujos de conversación.
- Implementación del motor de clasificación de intención (reglas y/o modelo ligero de NLP).
- Pruebas de precisión de respuestas y ajuste iterativo con casos reales.
- Documentación técnica del modelo para su mantenimiento futuro.

**Entregable:** Chatbot funcional con al menos 15–20 intents cubiertos y reporte de precisión de respuestas.

### 7.2 Ingeniería en Datos e Inteligencia Organizacional
**Rol:** base de conocimiento, backend y analítica de uso.

- Diseño de la base de datos de programas, servicios y preguntas frecuentes.
- Desarrollo del panel de administración con métricas de uso (consultas por categoría, tasa de resolución, horarios de mayor demanda).
- Generación de reportes periódicos de uso para el IQJ.

**Entregable:** Backend del chatbot + dashboard de analítica de uso.

### 7.3 Ingeniería Industrial
**Rol:** estandarización del proceso de contenido y calidad de servicio.

- Procedimiento estandarizado (SOP) de actualización de contenido: quién propone, quién valida, cada cuánto se revisa.
- Definición de indicadores de calidad de servicio (tiempo de respuesta, tasa de resolución automática, tasa de escalación).
- Protocolo de escalación hacia personal humano del Centro.

**Entregable:** Manual de operación y actualización del chatbot.

### 7.4 Ingeniería en Logística y Cadena de Suministro
**Rol:** enrutamiento de solicitudes hacia servicios físicos del Centro.

- Mapeo de trámites/servicios que requieren atención presencial (inscripción a talleres, citas, entrega de documentos).
- Diseño del flujo de derivación: chatbot → agenda/cita → confirmación.

**Entregable:** Flujo de canalización de servicios y, si aplica, calendario de citas vinculado al chatbot.

### 7.5 Componente STEM juvenil (jóvenes del Centro Comunitario)

- Participan como beta-testers del chatbot antes del lanzamiento oficial, dando retroalimentación de usabilidad.
- Reciben un taller de "cómo se construye un chatbot" impartido por los propios prestadores de servicio social.

---

## 8. Fases y cronograma

| Fase | Actividades principales | Ingenierías líderes | Duración estimada |
|---|---|---|---|
| 1. Levantamiento de información | Mapeo de programas y trámites del IQJ a cubrir | Industrial, Datos | `[pendiente]` |
| 2. Diseño conversacional | Definición de intents, flujos y base de conocimiento | IA, Datos | `[pendiente]` |
| 3. Desarrollo | Construcción del motor y canal (WhatsApp/web) | IA, Datos | `[pendiente]` |
| 4. Pruebas piloto | Beta-testing con jóvenes del Centro, ajustes | IA, todas | `[pendiente]` |
| 5. Lanzamiento y monitoreo | Puesta en marcha, seguimiento de métricas | Datos, Industrial | `[pendiente]` |
| 6. Evaluación y cierre de ciclo | Reporte final, liberación de servicio social | Todas | `[pendiente]` |

---

## 9. Mecanismo de liberación de servicio social

1. **Registro inicial:** el estudiante se inscribe al proyecto a través de su coordinación de carrera, con carta de presentación de la Universidad del Caribe.
2. **Asignación de módulo:** se ubica al estudiante en el módulo correspondiente a su ingeniería (sección 7).
3. **Bitácora de actividades:** registro semanal de horas y actividades, firmado por el supervisor del Centro Comunitario.
4. **Entregable por módulo:** cada estudiante o equipo produce el entregable definido en su sección correspondiente.
5. **Reporte final:** documento que integra evidencia de horas cumplidas + entregable técnico.
6. **Carta de liberación:** emitida por el Centro Comunitario/IQJ conforme al número de horas requerido por la Universidad del Caribe para cada plan de estudios.

> **Nota importante:** el número exacto de horas de servicio social debe confirmarse con la Dirección de Servicio Social de la Universidad del Caribe antes de operar el proyecto.

---

## 10. Roles y responsables

| Rol | Nombre | Puesto | Contacto |
|---|---|---|---|
| Autoriza | `[pendiente]` | `[pendiente]` | `[pendiente]` |
| Responsable del programa | `[pendiente]` | `[pendiente]` | `[pendiente]` |
| Supervisor de campo (Centro Comunitario) | `[pendiente]` | `[pendiente]` | `[pendiente]` |
| Enlace académico UCaribe por carrera | `[pendiente]` | `[pendiente]` | `[pendiente]` |

---

## 11. Recursos y materiales necesarios

- Cuenta de WhatsApp Business (API oficial o herramienta intermediaria de bajo costo/gratuita para volúmenes pequeños).
- Hosting/servidor para el backend del chatbot (plan gratuito o de bajo costo es suficiente en una primera etapa).
- Equipo de cómputo para el equipo de desarrollo.
- Acceso a información oficial y actualizada de los programas del IQJ.
- Widget de chat para el sitio web del IQJ (opcional, según alcance).

---

## 12. Indicadores de éxito

| Indicador | Meta sugerida |
|---|---|
| Intents/preguntas cubiertas | ≥ 15–20 en el lanzamiento |
| Tasa de resolución automática | `[pendiente]` |
| Usuarios/jóvenes atendidos por mes | `[pendiente]` |
| Tiempo promedio de respuesta | `[pendiente]` |
| Preguntas sin respuesta identificadas y resueltas | Seguimiento mensual |

---

## 13. Riesgos y mitigación

| Riesgo | Mitigación |
|---|---|
| Privacidad de datos de menores de edad | Aviso de privacidad simplificado, evitar recolectar datos sensibles innecesarios, validar con área jurídica del IQJ |
| Información desactualizada en el chatbot | SOP de actualización de contenido (Industrial) |
| Baja adopción por parte de los jóvenes | Difusión en talleres y redes del IQJ, pruebas piloto con jóvenes del Centro |
| Dependencia de un solo estudiante para el mantenimiento técnico | Documentación técnica clara para relevo entre generaciones de servicio social |
| Respuestas incorrectas o engañosas del chatbot | Revisión y validación de contenido por personal oficial del IQJ antes de publicarlo |

---

## 14. Anexos sugeridos (a desarrollar)

- Anexo A: Catálogo de intents y respuestas del chatbot.
- Anexo B: Aviso de privacidad simplificado para menores de edad (validar con área jurídica).
- Anexo C: Bitácora de horas de servicio social.
- Anexo D: Manual técnico de mantenimiento del chatbot.
