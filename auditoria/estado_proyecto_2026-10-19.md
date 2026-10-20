# Estado ejecutivo del proyecto al 19 de octubre de 2026

Fuente: [Inventario de aportes](inventario_aportes.md).  
Repositorio: https://github.com/lukaspardo/proyecto-grado-tesis  
Commit de referencia: 75bb53cf424948a1123e669170dc0e16fdf4c0c6.

Esta fotografía resume la evidencia registrada en el inventario; no constituye una nueva consulta de GitHub ni una aprobación académica. Los estados de los Issues corresponden a esa fecha de corte.

## 1. Estado general del repositorio

Existe una base investigativa sobre deuda técnica, SonarQube, LLM, alcance y metodología, pero los aportes están dispersos y requieren revisión antes de consolidarse. No se ha demostrado experimentalmente la utilidad del enfoque híbrido.

El inventario identifica cuatro archivos versionados en docs/ y seis adjuntos de Issues: diez ubicaciones correspondientes a ocho archivos distintos. Dos adjuntos son idénticos a sus copias versionadas según SHA-256. Los documentos de auditoría son registros de gestión y no se cuentan como nuevas entregas académicas.

No se ha reorganizado el proyecto ni consolidado un documento maestro. La falta de una aplicación desarrollada no constituye un vacío para el enfoque principalmente investigativo.

## 2. Estado de los Issues

Los títulos se conservan como aparecen registrados. El cierre administrativo no implica aceptación del aporte.

| Issue | Título | Responsable | Estado | Situación según el inventario |
|---|---|---|---|---|
| [#1](https://github.com/lukaspardo/proyecto-grado-tesis/issues/1) | Organizar repositorio,  backlog y documento maestro | lukaspardo | Cerrado | README mínimo; no se localizó maestro. La relación de AP-01 con el Issue es inferida. |
| [#2](https://github.com/lukaspardo/proyecto-grado-tesis/issues/2) | Definir deuda tecnica y buscar fuentes academicas | lukaspardo | Cerrado | AP-03: resumen insuficiente para el objetivo bibliográfico. |
| [#3](https://github.com/lukaspardo/proyecto-grado-tesis/issues/3) | Investigar metricas de sonarqube aplicables al estudio | deyvi0297 | Cerrado | AP-04: PDF entregado; requiere ajustes. |
| [#4](https://github.com/lukaspardo/proyecto-grado-tesis/issues/4) | Investigar que puede aportar un LLM al analisis del codigo | KarmaDevz | Cerrado | AP-05 requiere ajustes; AP-06 pendiente de revisión. |
| [#5](https://github.com/lukaspardo/proyecto-grado-tesis/issues/5) | Delimitar alcanze y criterios del proyecto | shibito9 | Cerrado | AP-02 aceptable como documento de alcance interno. |
| [#6](https://github.com/lukaspardo/proyecto-grado-tesis/issues/6) | Definir metodologia de evaluación SonarQube + LLM | deyvi0297 | Cerrado | AP-07: propuesta entregada; todavía no es un protocolo operativo. |
| [#7](https://github.com/lukaspardo/proyecto-grado-tesis/issues/7) | Seleccionar metricas de SonarQube para evaluar deuda tecnica | lukaspardo | Cerrado | AP-08: documento entregado; requiere ajustes. |
| [#8](https://github.com/lukaspardo/proyecto-grado-tesis/issues/8) | Seleccionar LLM y seleccionar el protocolo de analisis de codigo | KarmaDevz | Abierto | Hay antecedentes en AP-05; sin selección final ni protocolo específico localizado. |
| [#9](https://github.com/lukaspardo/proyecto-grado-tesis/issues/9) | Diseñar caso de estudio para prueba piloto del proyecto | shibito9 | Abierto | Sin diseño de un caso concreto localizado. |

Balance: siete Issues cerrados y dos abiertos. No se propone cambiar sus estados mediante este documento.

## 3. Entregables y clasificación recomendada

| Estado | Cantidad | Aportes |
|---|---:|---|
| ACEPTABLE_PARA_INTEGRACION | 1 | AP-02: Delimitacion_alcance_y_criterios.odt. |
| REQUIERE_AJUSTES | 4 | AP-04: Métricas seleccionadas.pdf; AP-05: investigacion-llm-analisis-estatico.md; AP-07: Propuesta Metodológica.pdf; AP-08: SonarQube.docx. |
| INSUFICIENTE | 2 | AP-01: docs/README.md; AP-03: Deuda Tecnica.docx. |
| ENTREGADO_PENDIENTE_REVISION | 1 | AP-06: apuntes.txt. |

AP-02 es aceptable como documento de alcance interno; no constituye evidencia bibliográfica ni protocolo metodológico definitivo. La recomendación no equivale a aprobación formal del equipo.

AP-01 es orientación del repositorio, no una investigación académica. AP-06 es un antecedente de trabajo y no debe contarse como una segunda investigación independiente de AP-05. Las clasificaciones restantes tampoco autorizan integración automática.

## 4. Material fuera del árbol Git

Cuatro archivos distintos se localizaron únicamente como adjuntos: AP-04 en #3, AP-05 y AP-06 en #4, y AP-07 en #6. Fueron leídos en memoria; no se incorporaron al repositorio.

Los adjuntos de #2 y #7 sí tienen copias idénticas en docs/. Las direcciones originales, responsables y huellas están en el inventario y no se repiten aquí.

El comentario de entrega de #4 menciona un documento Word compartido en el grupo. Su disponibilidad y contenido no están acreditados en este inventario; no se cuenta como entrega recuperada.

## 5. Vacíos actuales

| Elemento | Situación |
|---|---|
| Corpus bibliográfico | Hay referencias dispersas, pero no un corpus registrado ni protocolo de búsqueda y selección. |
| Matriz RAE | No se localizó. La matriz de evaluación del PDF metodológico no la sustituye. |
| Metodología operativa | Existe AP-07; faltan muestra, rúbrica, evaluadores, desacuerdos, controles, repeticiones y reglas de decisión. |
| Selección definitiva del LLM | Hay candidatos y criterios en AP-05; no una decisión final con versión y factibilidad documentadas. |
| Caso piloto | Hay bosquejos; no caso concreto, commit, licencia, configuración ni evidencia de ejecución registrados. |
| Documento maestro | No se localizó un documento consolidado. |
| Actas | No se localizaron actas versionadas. |

La revisión bibliográfica también está incompleta: AP-03 no cubre las fuentes académicas solicitadas y en AP-05 quedan verificaciones pendientes.

## 6. Inconsistencias de alcance

- El alcance interno prioriza investigación y piloto exploratorio, pero el encabezado de AP-05 conserva un título de prototipo predictivo. Deben acordarse título y pregunta únicos.
- La metodología anticipa reducción de deuda y mejoras de calidad sin resultados que las demuestren; deben formularse como hipótesis evaluables.
- Entregar al LLM el diagnóstico de SonarQube permite estudiar interpretación, pero no demuestra detección independiente.
- Los aportes de métricas se solapan y requieren distinguir deuda de mantenibilidad, complejidad, defectos, seguridad y cobertura antes de seleccionar indicadores.

## 7. Riesgos principales

| Riesgo | Consecuencia |
|---|---|
| Entregas dispersas y aceptación no documentada | Una clonación queda incompleta y se confunde entrega con integración. |
| Fuentes o afirmaciones sin verificar | La consolidación puede presentar como sustentadas conclusiones preliminares. |
| Beneficios anticipados y comparación sin controles | Se sesga la evaluación del enfoque híbrido. |
| Confusión entre priorización y predicción | Se asumen compromisos que el diseño actual no puede demostrar. |
| Versiones, parámetros y registros ausentes | El piloto no sería reproducible. |
| Documentos binarios y copias paralelas | Se dificultan la revisión de cambios y el control de versiones. |

## 8. Prioridades inmediatas

1. Confirmar la línea base del inventario, sus responsables y las clasificaciones propuestas.
2. Acordar título, pregunta y alcance investigativo, separando identificación, interpretación, priorización y predicción.
3. Definir criterios de aceptación de aportes y un registro de decisiones de revisión, sin equiparar cierre de Issue con aprobación.
4. Planificar los ajustes bibliográficos y técnicos de AP-03, AP-04, AP-05 y AP-08; revisar AP-06 como antecedente.
5. Definir protocolo de búsqueda, corpus bibliográfico y campos de la matriz RAE.
6. Convertir AP-07 en metodología operativa con línea base, rúbrica, controles y reglas para resultados favorables, desfavorables o inconclusos.
7. Completar #8 y #9 con selección justificada del LLM y diseño reproducible del caso piloto.
8. Evaluar posteriormente la reorganización y consolidación, preservando originales y procedencia.

## 9. Próxima fase recomendada

Realizar una fase de revisión y acuerdos antes de reorganizar: aprobar el alcance interno, establecer criterios de aceptación y preparar un plan de ajustes por aporte con responsable y evidencia exigida. Los integrantes entregarían sus investigaciones y correcciones; el responsable de integración revisaría los aportes y Codex apoyaría el contraste y la síntesis bajo aprobación humana.

La salida esperada sería un conjunto de decisiones trazables y un plan de trabajo aprobado para bibliografía, metodología y piloto. Esta recomendación no autoriza modificar documentos, trasladar adjuntos, cambiar Issues, consolidar el maestro ni realizar commits o push.
