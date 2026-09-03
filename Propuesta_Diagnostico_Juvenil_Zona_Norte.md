# Diagnóstico Juvenil Zona Norte y Mapas de Datos

### Propuesta de vinculación interdisciplinaria para liberación de Servicio Social

**Unidad responsable:** Centro Comunitario de Desarrollo Integral para las Juventudes
**Institución promotora:** Instituto Quintanarroense de la Juventud (IQJ)
**Instituciones académicas vinculadas:** Universidad del Caribe (UCaribe) y demás IES de la región con programas afines a STEM
**Cobertura geográfica:** Zona Norte de Quintana Roo — `[pendiente: confirmar municipios exactos que IQJ considera "zona norte", p. ej. Benito Juárez, Isla Mujeres, Puerto Morelos, Lázaro Cárdenas]`
**Proyectos relacionados:** [[Sistema de Gestión de Datos del Centro]] — el diagnóstico puede alimentar sus indicadores; [[Chatbot de Orientación Juvenil]] — puede usarse como canal de difusión de la encuesta
**Estatus del documento:** Borrador para revisión — completar campos marcados como `[pendiente]`

---

## 1. Datos generales del programa

| Campo | Información |
|---|---|
| Proyecto / programa | Diagnóstico Juvenil Zona Norte y Mapas de Datos |
| Responsable del programa | `[pendiente]` |
| Nombre del supervisor | `[pendiente]` |
| Puesto del supervisor | `[pendiente]` |
| Correo electrónico | `[pendiente]` |
| Vigencia del programa | Inicio: `[pendiente]` — Término: `[pendiente]` |
| Municipios cubiertos | `[pendiente]` |
| Sede de coordinación | Centro Comunitario de Desarrollo Integral para las Juventudes |

---

## 2. Justificación

Para diseñar programas y políticas públicas efectivas, el IQJ necesita información actualizada y georreferenciada sobre las condiciones, intereses y necesidades reales de los jóvenes de la zona norte del estado. `[pendiente: indicar si existe un diagnóstico previo o si este sería el primero]`.

Un diagnóstico con mapas de datos permite:

- Ubicar geográficamente dónde se concentran ciertas necesidades (educativas, laborales, de salud, de interés STEM).
- Priorizar en qué colonias o municipios enfocar nuevos programas del Centro Comunitario (incluyendo el huerto, talleres STEM, chatbot, etc.).
- Dar a los prestadores de servicio social de Datos, Industrial, Logística e IA un proyecto real de investigación aplicada con impacto directo en política pública juvenil.
- Generar evidencia cuantitativa que el IQJ pueda usar ante otras instancias de gobierno para gestionar recursos.

---

## 3. Objetivo general

Realizar un diagnóstico juvenil georreferenciado de la zona norte de Quintana Roo, mediante encuesta, análisis estadístico y mapas de datos, que sirva como insumo para el diseño de políticas públicas y programas del IQJ.

## 4. Objetivos específicos

1. Diseñar el instrumento de recolección (encuesta) con variables sociodemográficas, educativas, laborales y de interés STEM.
2. Definir la muestra y la estrategia de levantamiento por municipio/colonia.
3. Capacitar y coordinar brigadas de encuestadores (prestadores de servicio social y jóvenes voluntarios del Centro).
4. Procesar, limpiar y analizar los datos recolectados.
5. Generar mapas de datos (geolocalización de necesidades, densidad juvenil, acceso a servicios).
6. Elaborar un informe ejecutivo con hallazgos y recomendaciones para el IQJ.
7. Documentar el mecanismo de liberación de servicio social.

---

## 5. Marco institucional

| Actor | Rol en el proyecto |
|---|---|
| IQJ – Centro Comunitario | Coordinación general, validación de instrumento, receptor del informe final |
| Universidad del Caribe | Fuente de prestadores de servicio social, validación académica de horas |
| Coordinaciones de Datos, IA, Industrial y Logística | Asignación de estudiantes, revisión técnica de entregables |
| Autoridades municipales de la zona norte (si aplica) | Apoyo logístico o autorización de acceso a comunidades, `[pendiente confirmar]` |

---

## 6. Descripción general

- **Población objetivo:** jóvenes de `[pendiente: rango de edad, p. ej. 12–29 años]` en los municipios cubiertos.
- **Instrumento:** encuesta mixta (preguntas cerradas y abiertas), aplicable en formato digital y, como respaldo, en papel para zonas sin conectividad.
- **Georreferenciación:** cada encuesta se captura junto con su ubicación (colonia/municipio) para poder mapearla.
- **Salidas del proyecto:** base de datos limpia, mapas temáticos, segmentación de perfiles juveniles, informe ejecutivo y presentación de resultados al IQJ.

---

## 7. Participación por ingeniería

### 7.1 Ingeniería en Datos e Inteligencia Organizacional (líder del proyecto)
**Rol:** diseño metodológico, base de datos, análisis y mapas.

- Diseño del instrumento de encuesta (variables, escalas, validación).
- Diseño de la base de datos y del proceso de captura → limpieza → análisis.
- Análisis estadístico descriptivo e inferencial de los resultados.
- Construcción de mapas de datos con herramientas accesibles (p. ej. QGIS, Google My Maps o Power BI mapas).

**Entregable:** Base de datos limpia, mapas de datos y reporte estadístico.

### 7.2 Ingeniería en Inteligencia Artificial
**Rol:** análisis avanzado de la información recolectada.

- Análisis de texto de las respuestas abiertas (agrupamiento de temas y necesidades mencionadas).
- Modelo de segmentación (clustering) de perfiles juveniles según intereses, riesgos o necesidades.

**Entregable:** Reporte de segmentación de perfiles juveniles de la zona norte.

### 7.3 Ingeniería Industrial
**Rol:** estandarización del proceso de levantamiento y control de calidad.

- Diseño del flujo de levantamiento (tiempos, responsables, puntos de control).
- Capacitación de brigadas encuestadoras con un protocolo estandarizado de aplicación.
- Control de calidad y consistencia de los datos capturados en campo.

**Entregable:** Manual de levantamiento y protocolo de control de calidad de datos.

### 7.4 Ingeniería en Logística y Cadena de Suministro
**Rol:** planeación logística del trabajo de campo.

- Diseño de rutas y calendario de brigadas por municipio/colonia.
- Coordinación de recursos necesarios (transporte, materiales de encuesta, kits de campo).

**Entregable:** Plan logístico de levantamiento en campo.

### 7.5 Ingeniería Ambiental (participación opcional)
**Rol:** variables de entorno, si se decide ampliar el alcance del diagnóstico.

- Cruce de variables ambientales (acceso a áreas verdes, riesgo ambiental, servicios básicos de agua/saneamiento) con los resultados juveniles.

**Entregable:** Anexo de variables ambientales al diagnóstico (opcional, según alcance definido).

### 7.6 Componente STEM juvenil (jóvenes del Centro Comunitario)

- Participan como encuestadores voluntarios, capacitados junto con los prestadores de servicio social.
- Reciben un taller introductorio de "cómo se hace un diagnóstico con datos" (estadística básica y mapas).

---

## 8. Fases y cronograma

| Fase | Actividades principales | Ingenierías líderes | Duración estimada |
|---|---|---|---|
| 1. Diseño metodológico | Instrumento de encuesta, definición de muestra | Datos, Industrial | `[pendiente]` |
| 2. Capacitación de brigadas | Protocolo de aplicación, prueba piloto del instrumento | Industrial, Logística | `[pendiente]` |
| 3. Trabajo de campo | Levantamiento de encuestas por municipio/colonia | Logística, todas | `[pendiente]` |
| 4. Limpieza y procesamiento | Depuración y estructuración de la base de datos | Datos | `[pendiente]` |
| 5. Análisis, mapas y segmentación | Estadística, mapas temáticos, clustering | Datos, IA | `[pendiente]` |
| 6. Informe y presentación | Informe ejecutivo y presentación de resultados al IQJ | Todas | `[pendiente]` |
| 7. Evaluación y cierre de ciclo | Liberación de servicio social | Todas | `[pendiente]` |

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
| Coordinador de brigadas de campo | `[pendiente]` | `[pendiente]` | `[pendiente]` |
| Enlace académico UCaribe por carrera | `[pendiente]` | `[pendiente]` | `[pendiente]` |

---

## 11. Recursos y materiales necesarios

- Herramienta de encuesta digital georreferenciada (p. ej. Google Forms, KoboToolbox u otra herramienta gratuita/de bajo costo).
- Herramienta de mapas de datos (QGIS gratuito, Google My Maps o Power BI).
- Transporte para brigadas de campo.
- Material impreso de respaldo para zonas con baja conectividad.
- Formato de consentimiento informado para menores de edad (aval de tutores, cuando aplique).

---

## 12. Indicadores de éxito

| Indicador | Meta sugerida |
|---|---|
| Encuestas válidas levantadas | `[pendiente]` |
| Cobertura de municipios/colonias de la zona norte | `[pendiente]` % |
| Mapas de datos generados y publicados | ≥ 1 mapa por variable clave |
| Informe ejecutivo entregado y presentado a IQJ | Sí/No |
| Perfiles juveniles segmentados | ≥ 1 modelo de segmentación funcional |

---

## 13. Riesgos y mitigación

| Riesgo | Mitigación |
|---|---|
| Baja tasa de respuesta | Aplicar la encuesta durante eventos y talleres ya existentes del Centro |
| Datos de menores de edad | Consentimiento de tutores, anonimización, cumplimiento de protección de datos personales |
| Sesgo en el muestreo | Diseño muestral revisado conjuntamente por Datos e Industrial |
| Seguridad de las brigadas en campo | Rutas y horarios coordinados con supervisión del IQJ, siempre en pareja o grupo |
| Datos incompletos o inconsistentes | Protocolo de control de calidad en campo (Industrial) y validación en la limpieza (Datos) |

---

## 14. Anexos sugeridos (a desarrollar)

- Anexo A: Instrumento de encuesta completo.
- Anexo B: Formato de consentimiento informado (menores y tutores).
- Anexo C: Protocolo de levantamiento en campo.
- Anexo D: Bitácora de horas de servicio social.
