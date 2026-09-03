# Sistema de Gestión de Datos del Centro Comunitario

### Propuesta de vinculación interdisciplinaria para liberación de Servicio Social

**Unidad responsable:** Centro Comunitario de Desarrollo Integral para las Juventudes
**Institución promotora:** Instituto Quintanarroense de la Juventud (IQJ)
**Instituciones académicas vinculadas:** Universidad del Caribe (UCaribe) y demás IES de la región con programas afines a STEM
**Municipio:** Benito Juárez, Cancún
**Proyectos relacionados:** puede integrar datos de [[Chatbot de Orientación Juvenil]], [[Diagnóstico Juvenil Zona Norte y Mapas de Datos]] y del huerto comunitario como módulos o fuentes de información
**Estatus del documento:** Borrador para revisión — completar campos marcados como `[pendiente]`

---

## 1. Datos generales del programa

| Campo | Información |
|---|---|
| Proyecto / programa | Sistema de Gestión de Datos del Centro Comunitario |
| Responsable del programa | `[pendiente]` |
| Nombre del supervisor | `[pendiente]` |
| Puesto del supervisor | `[pendiente]` |
| Correo electrónico | `[pendiente]` |
| Vigencia del programa | Inicio: `[pendiente]` — Término: `[pendiente]` |
| Municipio | Benito Juárez, Cancún |
| Sede | Centro Comunitario de Desarrollo Integral para las Juventudes |

---

## 2. Justificación

El Centro Comunitario opera múltiples programas de forma simultánea (talleres STEM, huerto comunitario, chatbot de orientación, diagnósticos juveniles, servicio social de distintas carreras) sin un sistema centralizado que registre participantes, asistencia, horas de servicio social y resultados. Esto dificulta:

- Saber cuántos jóvenes se benefician realmente y de qué programas.
- Dar seguimiento ordenado a las horas de servicio social de cada estudiante.
- Generar reportes rápidos y confiables para el IQJ y otras instancias.
- Detectar a tiempo baja asistencia o abandono de jóvenes en los programas.

Un sistema de gestión de datos propio del Centro resuelve esto y, además, puede convertirse en la **columna vertebral** que conecta a los demás proyectos STEM del Centro (huerto, chatbot, diagnóstico).

---

## 3. Objetivo general

Diseñar e implementar un sistema de gestión de datos para el Centro Comunitario que centralice el registro de jóvenes, actividades, asistencia, servicio social y resultados de los programas en operación.

## 4. Objetivos específicos

1. Levantar los requerimientos de información del Centro Comunitario (qué necesita registrarse y para qué).
2. Diseñar la base de datos: padrón de jóvenes, catálogo de actividades/programas, asistencia y bitácora de servicio social.
3. Desarrollar el sistema (formularios de captura + backend + dashboard).
4. Integrar, cuando aplique, los datos generados por otros proyectos del Centro (huerto, chatbot, diagnóstico) como módulos o fuentes.
5. Establecer el proceso operativo de captura y mantenimiento de la información.
6. Definir el protocolo de privacidad y resguardo de datos de menores de edad.
7. Documentar el mecanismo de liberación de servicio social a través del propio sistema.

---

## 5. Marco institucional

| Actor | Rol en el proyecto |
|---|---|
| IQJ – Centro Comunitario | Sede del proyecto, usuario final del sistema, validación de indicadores |
| Universidad del Caribe | Fuente de prestadores de servicio social, validación académica de horas |
| Coordinaciones de Datos, Industrial, IA y Logística | Asignación de estudiantes, revisión técnica de entregables |
| Personal administrativo del Centro | Captura diaria de información, usuario principal del sistema |

---

## 6. Descripción general / Arquitectura conceptual

- **Módulo de padrón:** registro de jóvenes beneficiarios (datos básicos, consentimiento de tutores cuando sea menor de edad).
- **Módulo de actividades:** catálogo de talleres y programas del Centro, con responsables y fechas.
- **Módulo de asistencia:** registro de participación por actividad y fecha.
- **Módulo de servicio social:** bitácora de horas por estudiante y por proyecto (huerto, chatbot, diagnóstico, etc.), con generación de reportes para liberación.
- **Módulo de indicadores:** dashboard con métricas clave para la dirección del IQJ (jóvenes atendidos, horas de servicio social liberadas, actividades realizadas por periodo).

---

## 7. Participación por ingeniería

### 7.1 Ingeniería en Datos e Inteligencia Organizacional (líder del proyecto)
**Rol:** diseño y desarrollo del sistema.

- Diseño de la base de datos relacional (padrón, actividades, asistencia, servicio social).
- Desarrollo del dashboard de indicadores para la dirección del IQJ.
- Automatización de reportes periódicos (mensuales/trimestrales).

**Entregable:** Sistema funcional con base de datos y dashboard.

### 7.2 Ingeniería Industrial
**Rol:** estandarización de procesos de captura y uso del sistema.

- Levantamiento y estandarización de los procesos de captura de información (formularios, responsables, frecuencia de actualización).
- Elaboración del manual de usuario del sistema para el personal del Centro.
- Definición de indicadores operativos (tiempo de captura, calidad de los datos registrados).

**Entregable:** Manual de procesos y manual de usuario del sistema.

### 7.3 Ingeniería en Inteligencia Artificial (fase posterior, opcional)
**Rol:** capa analítica avanzada sobre los datos ya capturados.

- Modelo simple de alerta temprana (p. ej. jóvenes con baja asistencia o riesgo de abandono de un programa).
- Recomendación automática de talleres según los intereses registrados de cada joven.

**Entregable:** Prototipo de módulo de alertas o recomendación.

### 7.4 Ingeniería en Logística y Cadena de Suministro
**Rol:** módulo de inventario del Centro (opcional, según alcance).

- Módulo de inventario de materiales e insumos usados en los distintos programas del Centro.
- Definición del flujo de solicitud y resguardo de materiales para actividades.

**Entregable:** Módulo de inventario básico integrado al sistema (si se define dentro del alcance).

### 7.5 Componente STEM juvenil (jóvenes del Centro Comunitario)

- Son los usuarios finales registrados en el padrón y participan como beta-testers del sistema.
- Reciben un taller de "qué es un sistema de información" usando datos reales y anonimizados del propio Centro como ejemplo.

---

## 8. Fases y cronograma

| Fase | Actividades principales | Ingenierías líderes | Duración estimada |
|---|---|---|---|
| 1. Levantamiento de requerimientos | Qué debe registrar el sistema y para quién | Datos, Industrial | `[pendiente]` |
| 2. Diseño de base de datos y procesos | Modelo de datos, formularios, SOPs de captura | Datos, Industrial | `[pendiente]` |
| 3. Desarrollo del sistema | Backend, formularios de captura, dashboard | Datos | `[pendiente]` |
| 4. Migración y pruebas | Carga de datos existentes (si los hay) y pruebas del sistema | Datos, Industrial | `[pendiente]` |
| 5. Capacitación al personal | Uso del sistema por el personal del Centro | Industrial | `[pendiente]` |
| 6. Puesta en marcha y monitoreo | Operación regular, ajustes | Datos | `[pendiente]` |
| 7. Evaluación y cierre de ciclo | Reporte final, liberación de servicio social | Todas | `[pendiente]` |

---

## 9. Mecanismo de liberación de servicio social

1. **Registro inicial:** el estudiante se inscribe al proyecto a través de su coordinación de carrera, con carta de presentación de la Universidad del Caribe.
2. **Asignación de módulo:** se ubica al estudiante en el módulo correspondiente a su ingeniería (sección 7).
3. **Bitácora de actividades:** registro semanal de horas y actividades, firmado por el supervisor del Centro Comunitario — idealmente, una vez operando, **registrada directamente en el propio sistema** que se está construyendo.
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
| Administrador funcional del sistema (personal del Centro) | `[pendiente]` | `[pendiente]` | `[pendiente]` |
| Enlace académico UCaribe por carrera | `[pendiente]` | `[pendiente]` | `[pendiente]` |

---

## 11. Recursos y materiales necesarios

- Equipo de cómputo para el equipo de desarrollo.
- Hosting/servidor de bajo costo o gratuito, acorde al tamaño del sistema.
- Herramienta de desarrollo: puede iniciarse con una solución ligera (hoja de cálculo avanzada o plataforma no-code/low-code) y escalar a una base de datos propia si el alcance lo justifica.
- Acceso a la información actual del Centro (padrones o registros existentes, si los hay).

---

## 12. Indicadores de éxito

| Indicador | Meta sugerida |
|---|---|
| Jóvenes registrados en el padrón | `[pendiente]` |
| Actividades/programas gestionados en el sistema | `[pendiente]` |
| Horas de servicio social registradas a través del sistema | `[pendiente]` |
| Dashboard operativo y en uso regular por el personal | Sí/No |
| Tiempo de generación de reportes para el IQJ | Reducción medible respecto al proceso actual |

---

## 13. Riesgos y mitigación

| Riesgo | Mitigación |
|---|---|
| Privacidad de datos de menores de edad | Protocolo de datos, acceso restringido por rol, aviso de privacidad |
| Baja adopción por parte del personal del Centro | Capacitación y manual de usuario simple (Industrial) |
| Pérdida de continuidad entre generaciones de servicio social | Documentación técnica clara y control de versiones del sistema |
| Dependencia de una sola persona para el mantenimiento técnico | Transferencia de conocimiento documentada al cierre de cada ciclo |
| Datos duplicados o inconsistentes entre proyectos (huerto, chatbot, diagnóstico) | Definir este sistema como fuente única de verdad desde el diseño inicial |

---

## 14. Anexos sugeridos (a desarrollar)

- Anexo A: Diccionario de datos (campos del padrón, actividades, asistencia y servicio social).
- Anexo B: Manual de usuario del sistema.
- Anexo C: Aviso de privacidad para menores de edad (validar con área jurídica del IQJ).
- Anexo D: Bitácora de horas de servicio social.
