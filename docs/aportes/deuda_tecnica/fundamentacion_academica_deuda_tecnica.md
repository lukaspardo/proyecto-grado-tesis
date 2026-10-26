Fundamentación Académica de Deuda Técnica

Ruta del archivo: docs/aportes/deuda_tecnica/fundamentacion_academica_deuda_tecnica.md

Markdown

# Fundamentación Académica de la Deuda Técnica en el Desarrollo de Software

## 1. Introducción y Contextualización

El concepto de Deuda Técnica (Technical Debt - TD) fue introducido originalmente por Ward Cunningham en 1992 como una metáfora financiera para explicar los costos a largo plazo asociados con tomar atajos técnicos deliberados durante el desarrollo de software. En la investigación académica moderna, la deuda técnica ha evolucionado hasta convertirse en un campo de estudio clave dentro de la Ingeniería de Software que abarca desde decisiones de arquitectura hasta defectos de documentación y pruebas.

---

## 2. Revisión Sistemática de Fuentes Académicas Reales

### Fuente 1: Li, Z., Avgeriou, P., & Liang, P. (2015)

* **Título:** A systematic mapping study on technical debt and its management
* **Autores:** Zengyang Li, Paris Avgeriou, Peng Liang
* **Año:** 2015
* **Revista/Publicación:** *Journal of Systems and Software*, Vol. 101, pp. 193–220
* **DOI / Enlace:** [https://doi.org/10.1016/j.jss.2014.12.027](https://doi.org/10.1016/j.jss.2014.12.027)

#### Síntesis de Contenido

* **Definición de Deuda Técnica:** Metáfora que refleja compromisos técnicos tomados durante el desarrollo que pueden generar beneficios a corto plazo (como un lanzamiento rápido al mercado), pero que perjudican la salud, mantenibilidad y evolución a largo plazo del sistema de software.
* **Categorías / Tipos de Deuda Técnica:**
  1. *Architecture Technical Debt* (Deuda arquitectónica).
  2. *Design Technical Debt* (Deuda de diseño).
  3. *Code Technical Debt* (Deuda de código).
  4. *Test Technical Debt* (Deuda de pruebas).
  5. *Documentation Technical Debt* (Deuda de documentación).
  6. *Requirement Technical Debt* (Deuda de requerimientos).
  7. *Build/Infrastructure Technical Debt* (Deuda de compilación/infraestructura).
* **Causas:** Presión por tiempos de entrega (*time-to-market*), restricciones presupuestarias, falta de experiencia del equipo, evolución apresurada de requerimientos y toma de decisiones intencionadas para ganar ventaja competitiva temporal.
* **Consecuencias:** Incremento exponencial en los costos de mantenimiento, ralentización de la velocidad de desarrollo en iteraciones futuras, fragilidad del sistema y aumento del esfuerzo para agregar nuevas características.
* **Conclusiones Principales:** La Deuda Técnica no es intrínsecamente mala si es intencional y gestionada; sin embargo, la falta de visibilidad y monitoreo de la acumulación de intereses dificulta la sostenibilidad del software a largo plazo.

---

### Fuente 2: Rios, N., Spínola, R. O., Mendonça, M., & Seaman, C. (2020)

* **Título:** The practitioners' point of view on the concept of technical debt and its causes and consequences: a design for a global family of industrial surveys and its first results from Brazil
* **Autores:** Nicolli Rios, Rodrigo O. Spínola, Manoel Mendonça, Carolyn Seaman
* **Año:** 2020
* **Revista/Publicación:** *Empirical Software Engineering*, Vol. 25, No. 5, pp. 3216–3287
* **DOI / Enlace:** [https://doi.org/10.1007/s10664-020-09832-9](https://doi.org/10.1007/s10664-020-09832-9)

#### Síntesis de Contenido

* **Definición de Deuda Técnica:** Conjunto de soluciones no óptimas, atajos o compromisos en cualquier etapa del ciclo de vida del software que proporcionan beneficios inmediatos (menor esfuerzo o tiempo), pero que imponen un costo adicional (interés) durante el mantenimiento futuro.
* **Categorías / Tipos de Deuda Técnica:**
  - Deuda Intencional vs. No Intencional (McConnell Taxonomy).
  - Deuda Admitida Explícitamente (*Self-Admitted Technical Debt - SATD*), presente en comentarios de código (`TODO`, `FIXME`).
* **Causas:** Falta de pruebas automatizadas, presión del negocio, sobrecarga de trabajo, baja capacitación del personal, mala comunicación entre stakeholders y arquitecturas obsoletas.
* **Consecuencias:** Degradación de los atributos de calidad (mantenibilidad, fiabilidad y desempeño), desmotivación del equipo de desarrollo e incremento incontrolado del esfuerzo operativo.
* **Conclusiones Principales:** Existe una brecha entre la teoría y la práctica en cómo los profesionales perciben la deuda técnica. Identificar y visibilizar las causas raíces en la industria es esencial para implementar estrategias eficaces de pago de deuda.

---

### Fuente 3: Lenarduzzi, V., Besker, T., Taibi, D., Martini, A., & Arcelli Fontana, F. (2021)

* **Título:** A systematic literature review on Technical Debt prioritization: Strategies, processes, factors, and tools
* **Autores:** Valentina Lenarduzzi, Terese Besker, Davide Taibi, Antonio Martini, Francesca Arcelli Fontana
* **Año:** 2021
* **Revista/Publicación:** *Journal of Systems and Software*, Vol. 171, Article 110827
* **DOI / Enlace:** [https://doi.org/10.1016/j.jss.2020.110827](https://doi.org/10.1016/j.jss.2020.110827)

#### Síntesis de Contenido

* **Definición de Deuda Técnica:** Deficiencias en los artefactos de software que no impiden el funcionamiento actual de la aplicación, pero que generan una penalización económica o técnica futura si no se refactorizan.
* **Categorías / Tipos de Deuda Técnica:**
  - Deuda Técnica Priorizable basada en Riesgo, Valor de Negocio y Severidad Técnica.
* **Causas:** Falta de procesos formales de refactorización, priorización enfocada únicamente en *features* visibles para el usuario y ausencia de herramientas integradas en los entornos de CI/CD.
* **Consecuencias:** Acumulación descontrolada del "Capital" y del "Interés" de la deuda, paralización de entregas de valor al cliente y elevado riesgo de fallas críticas en producción.
* **Conclusiones Principales:** Priorizar la deuda técnica no consiste en refactorizar todo el código defectuoso, sino en evaluar el equilibrio costo-beneficio del impacto económico e industrial que genera pagar cada ítem de deuda.

---

## 3. Diferenciación Conceptualmente Rigurosa

Para fundamentar correctamente el marco teórico del proyecto, es crítico diferenciar la **Deuda Técnica** de otros conceptos relacionados con la calidad del software:

| Concepto | Definición | ¿Es Deuda Técnica? | Criterio de Diferenciación |
| :--- | :--- | :---: | :--- |
| **Deuda Técnica (TD)** | Decisión o compromiso técnico (a menudo consciente) que acelera el corto plazo pero penaliza la mantenibilidad y evolución del software a largo plazo. | **SÍ** | Implica el pago de **intereses** (mayor esfuerzo futuro) y un **capital** (esfuerzo de refactorización para solucionarlo). El software funciona, pero cambiarlo es costoso. |
| **Defectos / Bugs** | Errores o desviaciones de la funcionalidad esperada que provocan un comportamiento incorrecto o fallo en el sistema en tiempo de ejecución. | **NO** | Un *bug* representa una **falla funcional inmediata** que debe corregirse para cumplir los requisitos. La deuda técnica es un problema de calidad interna (mantenibilidad), no necesariamente un error de cara al usuario final. |
| **Code Smells** | Síntomas visuales en el código fuente (ej. clases gigantes, métodos extensos) que sugieren un problema de diseño o violación de principios de programación (Clean Code). | **NO DIRECTAMENTE** | Los *code smells* son **indicadores o síntomas** de que podría existir deuda técnica. No toda deuda técnica es un *code smell* (ej. falta de arquitectura o documentación), ni todo *code smell* representa un interés financiero real. |
| **Problemas Generales de Calidad** | Atributos deficientes de calidad externa (usabilidad lenta, fallas de accesibilidad, bajo rendimiento en producción). | **NO** | La calidad general abarca factores tanto **internos como externos**. La Deuda Técnica concierne específicamente a la **calidad interna e ingeniería del software** (mantenibilidad, flexibilidad, escalabilidad). |

---

## 4. Aporte y Valor Agregado al Proyecto

1. **Aporte de Li et al. (2015):** Aporta la **taxonomía multidimensional** al proyecto. Permite que el equipo no clasifique la deuda técnica únicamente como "código feo", sino que identifique deuda en la documentación, las pruebas automatizadas y la arquitectura del sistema.
2. **Aporte de Rios et al. (2020):** Brinda el marco empírico sobre **causas reales e industriales**. Permite justificar por qué la presión del tiempo o la falta de pruebas durante las primeras etapas justifican las decisiones tomadas en el proyecto.
3. **Aporte de Lenarduzzi et al. (2021):** Otorga la metodología para **gestionar y priorizar la deuda técnica**. Ayuda al proyecto a definir criterios racionales de refactorización basados en el riesgo y el valor entregado al negocio, en lugar de realizar refactorizaciones a ciegas.

Información Preparada para la Matriz RAE Oficial (Resumen Analítico Educativo)

Con la siguiente estructura el integrante del equipo puede diligenciar la Matriz RAE oficial:

Ficha RAE 1

- Tipo de documento: Artículo de revisión científica (Systematic Mapping Study)
- Título: A systematic mapping study on technical debt and its management
- Autores: Zengyang Li, Paris Avgeriou, Peng Liang
- Publicación: Journal of Systems and Software (2015)
- DOI: 10.1016/j.jss.2014.12.027
- Palabras Clave: Technical Debt, Software Architecture, Code Quality, Software Management.
- Descripción del contenido: Mapeo sistemático de la literatura que clasifica la deuda técnica en 10 categorías clave, identifica sus causas organizacionales y mapea las actividades del ciclo de vida de gestión de la deuda (identificación, medición, priorización y pago).
- Aporte al proyecto: Proporciona la estructura taxonómica formal para categorizar las deudas detectadas dentro de nuestro sistema.

Ficha RAE 2

- Tipo de documento: Artículo de investigación empírica (Industrial Survey)
- Título: The practitioners' point of view on the concept of technical debt and its causes and consequences...
- Autores: Nicolli Rios, Rodrigo O. Spínola, Manoel Mendonça, Carolyn Seaman
- Publicación: Empirical Software Engineering (2020)
- DOI: 10.1007/s10664-020-09832-9
- Palabras Clave: Empirical Software Engineering, Technical Debt Causes, Technical Debt Consequences, Industry Survey.
- Descripción del contenido: Estudio global sobre cómo la industria percibe la deuda técnica, demostrando empíricamente que la presión del mercado y la mala planificación son los principales generadores de deuda técnica en proyectos reales.
- Aporte al proyecto: Justifica el análisis de las causas de la deuda dentro del marco contextual del proyecto.

Ficha RAE 3

- Tipo de documento: Revisión Sistemática de Literatura (SLR)
- Título: A systematic literature review on Technical Debt prioritization: Strategies, processes, factors, and tools
- Autores: Valentina Lenarduzzi, Terese Besker, Davide Taibi, Antonio Martini, Francesca Arcelli Fontana
- Publicación: Journal of Systems and Software (2021)
- DOI: 10.1016/j.jss.2020.110827
- Palabras Clave: Technical Debt Prioritization, Refactoring, Software Maintenance, Decision Making.
- Descripción del contenido: Análisis de los métodos y factores que permiten decidir qué ítems de deuda técnica se deben pagar y cuáles se deben posponer basándose en el balance riesgo/costo/beneficio.
- Aporte al proyecto: Fundamenta la toma de decisiones en el plan de refactorización del proyecto.
