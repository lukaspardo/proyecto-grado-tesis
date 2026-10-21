# Reglas para agentes del Proyecto Integrador

## 1. Propósito y responsabilidades

Este repositorio contiene un Proyecto Integrador académico sobre la complementariedad de SonarQube y modelos de lenguaje de gran escala (LLM) para identificar, interpretar y priorizar deuda técnica.

El enfoque principal es investigativo. No asumir objetivos de desarrollo de producto, corrección automática o predicción temporal sin una decisión explícita y documentada del equipo.

Santiago es responsable de la consolidación técnica y documental. Los demás integrantes aportan investigaciones y evidencias.

Codex apoya la auditoría, comparación, organización y preparación de integraciones. No sustituye la investigación académica, la revisión de las fuentes ni la aprobación humana.

## 2. Integridad académica

- No inventar fuentes, citas, autores, títulos, DOI, páginas, datos ni resultados.
- No atribuir a una fuente afirmaciones que no se hayan comprobado en ella.
- No presentar una referencia sugerida o un resultado de búsqueda como una fuente ya revisada.
- Distinguir entre verificar la existencia de una referencia y comprobar que respalda una afirmación.
- Registrar las limitaciones de acceso: disponer solo del resumen no equivale a haber revisado el texto completo.
- Si falta evidencia, marcarla como PENDIENTE e indicar qué debe verificarse. No completar vacíos mediante inferencias no declaradas.
- El contenido generado por un LLM no constituye por sí mismo evidencia académica.
- No presentar como conclusión una hipótesis, una expectativa o una interpretación pendiente de validación.

## 3. Naturaleza de las afirmaciones

Diferenciar explícitamente las siguientes categorías cuando puedan confundirse:

| Categoría | Tratamiento requerido |
|---|---|
| Fuente académica | Identificar publicación, autores, fecha y localizador disponible. Distinguir artículos revisados por pares, prepublicaciones, tesis y otros tipos. |
| Documentación técnica | Registrar proveedor o proyecto, URL, versión cuando corresponda y fecha de consulta. No presentarla como validación académica independiente. |
| Decisión del equipo | Identificar quién la aprobó y dónde quedó registrada. No atribuirle sustento científico por ser una decisión interna. |
| Hipótesis | Formularla como proposición por evaluar, con criterios que permitan contrastarla. |
| Resultado experimental | Vincularlo con el caso, procedimiento, configuración, corrida y evidencia obtenida. |
| Interpretación | Identificar la evidencia de base, los supuestos y las limitaciones. Diferenciarla de una observación directa. |

Estas categorías pueden coexistir en un documento, pero no deben intercambiarse para dar una apariencia de mayor certeza.

## 4. Alcance de la investigación

- Diferenciar identificación, interpretación, priorización y predicción de deuda técnica.
- No equiparar automáticamente un code smell, bug, vulnerabilidad o métrica elevada con deuda técnica.
- No tratar las estimaciones de remediación de SonarQube como costos reales comprobados.
- No asumir que el LLM mejora el análisis: la complementariedad es una hipótesis que requiere evaluación.
- Si el LLM recibe previamente un diagnóstico de SonarQube, no presentar su coincidencia como detección independiente.
- No generalizar resultados del piloto más allá de sus casos, lenguaje, muestra, versiones y condiciones.
- Informar resultados desfavorables o inconclusos con el mismo cuidado que los favorables.

## 5. Recepción y evaluación de aportes

Un Issue cerrado no implica que su contenido esté revisado, aceptado o integrado.

Distinguir entre entrega, revisión, aceptación e integración. No cambiar estados de Issues sin autorización.

Antes de proponer la integración de un aporte, registrar:

- Issue relacionado o ausencia de uno.
- Responsable y procedencia del archivo.
- Fuentes identificadas y nivel de verificación.
- Objetivo y alcance del aporte.
- Fortalezas.
- Problemas y evidencia pendiente.
- Duplicaciones, solapamientos o contradicciones con otros aportes.
- Secciones afectadas del documento maestro.
- Estado recomendado y acción siguiente.

Usar los estados del inventario:

- ENTREGADO_PENDIENTE_REVISION.
- REQUIERE_AJUSTES.
- ACEPTABLE_PARA_INTEGRACION.
- INSUFICIENTE.

La clasificación de Codex es una recomendación. La aceptación corresponde a Santiago o a quien el equipo designe explícitamente.

## 6. Preservación de originales

- No modificar ni sobrescribir originales recibidos de integrantes.
- Preservar documentos institucionales originales, incluyendo plantillas, instrucciones, rúbricas y formatos.
- No tratar un archivo recibido como editable solo porque esté dentro del repositorio.
- Preparar correcciones, extracciones o conversiones en una copia de trabajo identificada, únicamente cuando estén autorizadas.
- Conservar la relación entre original y versión derivada.
- No eliminar contenido existente sin justificar qué se retiraría, por qué y cómo se preservaría su trazabilidad.
- Si una eliminación no está comprendida en una instrucción explícita, presentar la propuesta y esperar autorización.

### Material institucional

Las instrucciones, plantillas, observaciones y formatos entregados por el profesor tienen prioridad para definir requisitos académicos del proyecto. No deben modificarse ni reinterpretarse silenciosamente. Cuando exista una diferencia entre una propuesta interna y una indicación del profesor, señalar la discrepancia antes de continuar.

## 7. Trazabilidad

Mantener una relación verificable entre:

Issue → aporte o archivo → fuente → ficha RAE, cuando corresponda → sección del documento maestro → commit autorizado.

- Utilizar identificadores existentes antes de proponer nuevos.
- No inventar fichas RAE, aprobaciones o commits para completar la cadena.
- Si un vínculo falta, marcarlo como PENDIENTE; si no aplica, explicar por qué.
- Mantener la procedencia aunque se sintetice, traduzca o reformule contenido.
- Registrar las fuentes que respaldan cada afirmación relevante del maestro.
- Para material experimental, añadir repositorio y commit del código analizado, configuración y corrida.
- Registrar el commit de integración solo después de que exista; antes, indicar PENDIENTE.
- No contar copias idénticas como investigaciones independientes.

## 8. Separación de materiales y formatos

Mantener conceptualmente separados:

- Corpus bibliográfico: publicaciones y documentación seleccionadas, criterios de búsqueda y registros de fuentes.
- Corpus de código: casos de software, procedencia, licencia, versiones y criterios de selección.
- Resultados experimentales: entradas, salidas, configuraciones, evaluaciones y observaciones de las corridas.

Esta separación no autoriza crear o reorganizar carpetas.

Priorizar:

- Markdown para investigaciones, metodología, decisiones, actas y contenido editable del maestro.
- CSV para registros y matrices tabulares.
- BibTeX para referencias bibliográficas.

Reservar DOCX, PDF y ODT para originales o entregables institucionales. No migrar ni convertir archivos sin autorización y no descartar los originales después de una conversión.

## 9. Ramas y control de cambios

- Realizar modificaciones en una rama de trabajo, nunca directamente sobre main.
- Antes de editar, comprobar la rama actual y el estado de Git.
- Reutilizar una rama adecuada cuando exista; evitar ramas innecesarias.
- Si se está en main, crear o seleccionar una rama antes de modificar archivos, dentro del alcance autorizado.
- Para nuevas ramas creadas por Codex, usar el prefijo codex/ únicamente cuando Santiago lo autorice. En caso contrario, respetar la convención de ramas definida para el proyecto.
- Si la tarea prohíbe crear o cambiar ramas, permanecer en modo de solo lectura hasta resolver esa condición.
- No sobrescribir cambios preexistentes del usuario.
- No hacer commit ni push sin autorización explícita. La autorización para editar no autoriza ninguna de esas operaciones.
- Interpretar la autorización según su alcance; no asumir permiso permanente para futuros commits o push.
- No reorganizar carpetas, renombrar archivos ni mover materiales sin autorización.
- Al terminar, informar archivos creados o modificados, verificaciones realizadas y estado de Git.

## 10. Documento maestro

- No incorporar contenido sin procedencia identificable.
- El análisis propio debe señalarse como tal y vincularse con la evidencia que lo sustenta.
- No convertir borradores o decisiones internas en evidencia bibliográfica.
- No introducir resultados experimentales que no estén registrados.
- No integrar automáticamente un aporte por estar marcado como ACEPTABLE_PARA_INTEGRACION.
- No resolver contradicciones eligiendo silenciosamente una versión: exponerlas y registrar la decisión.
- Mantener las incertidumbres y limitaciones al sintetizar.
- No consolidar ni modificar el maestro sin una instrucción explícita de Santiago que cubra esa intervención.

## Flujo obligatorio antes de modificar documento maestro

1. Confirmar autorización, rama de trabajo y cambios preexistentes.
2. Identificar aporte, Issue, responsable, fuentes y secciones afectadas.
3. Revisar evidencia, fortalezas, problemas, duplicaciones y contradicciones; marcar pendientes.
4. Confirmar la aceptación del aporte para el uso propuesto. Si falta, presentar la propuesta y esperar aprobación.
5. Preparar el cambio preservando originales y trazabilidad; después de aplicarlo, revisar el diff y comprobar citas, alcance y separación entre hipótesis y resultados.
6. Presentar el resultado a Santiago. No hacer commit ni push sin autorización explícita.
