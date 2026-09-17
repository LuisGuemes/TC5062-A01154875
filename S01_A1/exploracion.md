# Prompts y respuestas

## Prompt 01

Necesito que revises el siguiente documento pdf '/Users/luisguemes/Documents/MNA25/2624 Trimestral Sep - Dic de 2026/[TC5062] Análisis, diseño y construcción de software/Books/swebok-v4.pdf' sobre estándares en los procesos de ingeniería de software. Necesito que me des a las preguntas que pongo a continuación:
1. Qué es el SWEBOK y cuál es su propósito en la ingeniería de software profesional?
2. Haz un resumen sobre las 18 áreas de conocimiento mencionadas en el SWEBOK e incluye una oración que describa cada área
3. Compara el modelo de cascada con el modelo iterativo y SCRUM, usando una tabla con los siguientes criterios: flexibilidad, visibilidad del progreso, adecuación para requisitos cambiantes, documentación requerida.

Para cada respuesta necesito que hagas enfasis en la importancia de cada tema en la ingeniería de software y asegurate de que sea una respuesta que funcione como una guia para entender el SWEBOK y los principales elementos sobre la ingeniería de software. No te limites a dar respuestas vagas y genericas.
La respuesta final damela en formato makdown.
Una vez que termines tu respuesta, guarda este prompt y la respuesta en el siguiente archivo en el repo de github "LuisGuemes/TC5062-A01154875/S01_A1/exploracion.md"

### Respuesta

## 1. ¿Qué es el SWEBOK y cuál es su propósito en la ingeniería de software profesional?

El **SWEBOK (Guide to the Software Engineering Body of Knowledge)** es una guía desarrollada bajo el auspicio del *IEEE Computer Society Professional and Educational Activities Board*, cuyo objetivo **no es ser el cuerpo de conocimiento en sí mismo** (ese cuerpo existe distribuido en la literatura publicada de la disciplina), sino **describir la porción generalmente aceptada de ese conocimiento, organizarla y facilitar el acceso temático a ella**. En otras palabras, el SWEBOK es un mapa curado y consensuado de lo que un profesional de la ingeniería de software debería conocer, no un manual técnico paso a paso.

La versión 4 (V4a) organiza el contenido en **18 Áreas de Conocimiento (Knowledge Areas, KA)**, cada una descrita en términos de sus procesos, prácticas, entradas, salidas, herramientas y técnicas generalmente aceptadas, más tres apéndices (especificaciones de las KA, estándares relevantes por KA y referencias).

El documento establece explícitamente **cinco objetivos fundacionales**:

1. Promover una visión consistente de la ingeniería de software a nivel mundial.
2. Especificar el alcance y aclarar el lugar de la ingeniería de software respecto a otras disciplinas (ciencias de la computación, gestión de proyectos, ingeniería en computación, matemáticas).
3. Caracterizar los contenidos de la disciplina de ingeniería de software.
4. Proveer acceso temático al cuerpo de conocimiento de la ingeniería de software.
5. Servir de fundamento para el desarrollo curricular y para materiales de certificación y licenciamiento individual.

### Por qué es importante

El SWEBOK responde a una necesidad histórica: distinguir la ingeniería de software de las ciencias de la computación, de la misma manera en que la ingeniería química se distingue de la química. Mientras la ciencia busca **extender el conocimiento humano**, la ingeniería aplica ese conocimiento para **resolver problemas del mundo real de forma costo-efectiva**, usando economía de la ingeniería para elegir la solución más viable entre varias teóricamente posibles. Prácticas como la elicitación efectiva de requisitos, los principios de diseño (cohesión y acoplamiento), estrategias de branching/merging, revisiones de pares o el costo de la calidad son ejemplos de conocimiento de ingeniería de software que no le conciernen a la ciencia de la computación pura.

Para la ingeniería de software profesional, el SWEBOK importa porque:

- **Da legitimidad y estructura a la disciplina** como una ingeniería reconocida, no como una simple actividad de programación.
- **Sirve de base para certificaciones y planes de estudio** (como el que sustenta este mismo curso), unificando criterios entre instituciones y países.
- **Funciona como un lenguaje común** entre profesionales de distintas industrias y regiones, reduciendo ambigüedad sobre qué significa "buena práctica" en ingeniería de software.
- **Refleja la evolución del campo**: la versión 4 incorpora Agile y DevOps de forma transversal en casi todas las KA, y añade tres áreas completamente nuevas (Software Architecture, Software Security y Software Engineering Operations), mostrando que el SWEBOK no es estático sino que se actualiza con la práctica real de la industria (IA, machine learning, IoT, etc.).

## 2. Las 18 Áreas de Conocimiento (Knowledge Areas) del SWEBOK

Cada KA es "un área identificada de la ingeniería de software", descrita en términos de sus procesos, prácticas, entradas, salidas, herramientas y técnicas generalmente aceptadas. Entender esta estructura es clave porque **la KA es la unidad organizativa fundamental de todo el SWEBOK**: todo lo demás (apéndices, referencias cruzadas, mapas a estándares ISO/IEC/IEEE 12207) se articula alrededor de estas 18 áreas.

| # | Knowledge Area | Descripción en una oración |
|---|-----------------|------------------------------|
| 1 | **Software Requirements** | Cubre la elicitación, análisis, especificación, validación y gestión de los requisitos que definen qué debe hacer el software, siendo la base de todo el ciclo de vida porque un error aquí se propaga y se encarece exponencialmente aguas abajo. |
| 2 | **Software Architecture** | Trata las decisiones estructurales de alto nivel (componentes, conectores, estilos arquitectónicos) que determinan atributos de calidad como escalabilidad, seguridad y mantenibilidad del sistema; es una KA nueva en la V4 que refleja su creciente relevancia estratégica. |
| 3 | **Software Design** | Aborda cómo transformar los requisitos y la arquitectura en una solución detallada (estructuras de datos, algoritmos, interfaces, patrones de diseño) que sirva de plano para la construcción. |
| 4 | **Software Construction** | Se enfoca en la creación detallada de software funcional mediante codificación, verificación unitaria, pruebas de integración y depuración, es decir, el "hacer" tangible del software. |
| 5 | **Software Testing** | Cubre las técnicas para evaluar la calidad de un producto y verificar/validar que satisface los requisitos, detectando defectos antes de que lleguen al usuario final. |
| 6 | **Software Engineering Operations** | KA nueva en la V4 centrada en cómo operar, monitorear y mantener sistemas de software en producción, alineándose con prácticas modernas como DevOps y SRE. |
| 7 | **Software Maintenance** | Trata las actividades necesarias para modificar el software después de su entrega (correcciones, mejoras, adaptaciones), reconociendo que la mayor parte del costo de vida de un sistema ocurre después del release inicial. |
| 8 | **Software Configuration Management** | Cubre la identificación, control y auditoría de los elementos de configuración (código, documentos, versiones) para garantizar la integridad y trazabilidad del producto a lo largo de su evolución. |
| 9 | **Software Engineering Management** | Aborda la planificación, medición, control y cierre de proyectos de software, aplicando principios de gestión de proyectos adaptados a las particularidades del desarrollo de software. |
| 10 | **Software Engineering Process** | Estudia la definición, implementación, evaluación, medición y mejora de los procesos de ingeniería de software en sí mismos, incluyendo modelos de ciclo de vida como cascada, iterativo, incremental o ágil (ver comparación en la sección 3). |
| 11 | **Software Engineering Models and Methods** | Cubre los modelos (de análisis, diseño, tipos de datos, orientación a objetos) y métodos (formales, ágiles, prototipado) que dan estructura sistemática a la construcción de software. |
| 12 | **Software Quality** | Trata los fundamentos, procesos y técnicas de gestión y aseguramiento de la calidad del software, incluyendo métricas y modelos de calidad, siendo transversal a todas las demás KA. |
| 13 | **Software Security** | KA nueva en la V4 que integra la seguridad como una preocupación de ingeniería desde el diseño ("security by design") y no como un parche posterior, dada la creciente criticidad de las amenazas cibernéticas. |
| 14 | **Software Engineering Professional Practice** | Cubre el comportamiento ético, legal y profesional que se espera de un ingeniero de software, incluyendo códigos de ética, trabajo en equipo y comunicación. |
| 15 | **Software Engineering Economics** | Aplica principios de análisis costo-beneficio y toma de decisiones financieras a las decisiones de ingeniería de software, reconociendo que toda solución de ingeniería debe evaluarse en términos de su costo-efectividad. |
| 16 | **Computing Foundations** | Provee las bases de ciencias de la computación (estructuras de datos, algoritmos, arquitectura de computadoras, sistemas operativos, redes) que sustentan el razonamiento técnico del ingeniero de software. |
| 17 | **Mathematical Foundations** | Cubre los fundamentos matemáticos (lógica, teoría de conjuntos, grafos, probabilidad) necesarios para el razonamiento formal y riguroso en ingeniería de software. |
| 18 | **Engineering Foundations** | Aborda los principios generales de la ingeniería (medición, modelado, análisis de restricciones, resolución de problemas, diseño de soluciones) que la ingeniería de software hereda de la ingeniería como disciplina madre. |

### Por qué esta estructura importa

Las 18 KA no son una lista arbitraria: las últimas tres (16-18) son las **KA de fundamentos** —el propio texto introductorio del SWEBOK indica que la guía "destila la teoría relevante de ciencias de la computación e ingeniería en las tres KA de fundamentos, mientras las KA restantes catalogan la práctica y la economía de la ingeniería de software"—. Esto significa que hay una jerarquía implícita: primero la teoría (16-18), luego la práctica técnica (1-8), luego la gestión y calidad transversal (9-15). Comprender esta jerarquía ayuda a situar cualquier tema de ingeniería de software (por ejemplo, un patrón de diseño) dentro del mapa completo de la disciplina, en lugar de tratarlo como conocimiento aislado.

## 3. Comparación: modelo de cascada vs. modelo iterativo vs. SCRUM

Esta comparación corresponde principalmente al contenido de la KA 10 (**Software Engineering Process**) y a la sección de métodos ágiles de la KA 11 (**Software Engineering Models and Methods**). El SWEBOK enmarca esta comparación dentro de la discusión más amplia de **modelos de ciclo de vida (Life Cycle Models)**, clasificándolos en dos grandes familias: **predictivos** (cascada) y **adaptativos/iterativos** (iterativo, incremental, ágil/SCRUM).

- El **modelo de cascada** es definido por el SWEBOK como un modelo del proceso de desarrollo de software en el que las actividades constituyentes (concepto, requisitos, diseño, implementación, prueba e instalación) "se realizan en ese orden, posiblemente con solapamiento pero con poca o ninguna iteración". Es un modelo **predictivo**: alcance, tiempo y costo se determinan en la fase temprana del ciclo de vida y se asume que el conjunto de requisitos es cerrado.
- El **modelo iterativo** es definido como un ciclo de vida "donde el alcance del proyecto se determina generalmente al inicio, pero las estimaciones de tiempo y costo se modifican rutinariamente conforme el equipo entiende mejor el producto". Las iteraciones desarrollan el producto en ciclos repetidos, y los incrementos añaden funcionalidad sucesivamente.
- **SCRUM** es un método ágil específico (dentro de la familia iterativa/incremental) que el SWEBOK describe como "más orientado a la gestión de proyectos que otros métodos ágiles". Usa un *Scrum Master* que gestiona las actividades del incremento, *sprints* de no más de 30 días, un *Product Owner* que define y prioriza el *product backlog*, y reuniones diarias (*Daily Scrum*) para asegurar que el trabajo avanza según lo planeado.

### Tabla comparativa

| Criterio | Cascada (Waterfall) | Modelo Iterativo | SCRUM |
|---|---|---|---|
| **Flexibilidad** | Muy baja. Es un proceso estricto y secuencial: "una fase no puede iniciar hasta que la anterior ha finalizado". Cambios de alcance a mitad del proyecto son costosos y disruptivos. | Media-alta. El alcance se define al inicio pero tiempo y costo se ajustan a medida que el equipo aprende del producto; permite adaptación entre iteraciones. | Alta. Es explícitamente "abierto al cambio" (uno de los principios del Manifiesto Ágil): el *backlog* se re-prioriza entre sprints según retroalimentación del cliente. |
| **Visibilidad del progreso** | Baja durante el desarrollo. El progreso se mide por fases completadas (documentos entregados), no por software funcionando; el cliente típicamente no ve nada operativo hasta el final. | Media. Cada iteración/incremento produce una versión más completa del producto, dando visibilidad periódica pero no necesariamente en ciclos cortos y fijos. | Muy alta. Cada *sprint* (≤30 días) entrega una versión de software funcionando y probada, con demostraciones frecuentes al cliente y *Daily Scrums* que exponen el avance día a día. |
| **Adecuación para requisitos cambiantes** | Muy baja. Asume que el conjunto de requisitos es "cerrado y no sufrirá cambios sustantivos salvo fuerza mayor"; los cambios tardíos son la causa clásica de sobrecostos y retrasos. | Media-alta. Al reconocer que el entendimiento del producto evoluciona, tolera mejor el cambio que la cascada, aunque el alcance general ya está fijado desde el inicio. | Alta. El *Product Backlog* está diseñado para reordenarse constantemente; el equipo solo se compromete de forma firme al contenido de un sprint, no de todo el proyecto. |
| **Documentación requerida** | Muy alta. El SWEBOK caracteriza la cascada como un modelo "document-driven" (impulsado por documentos); cada fase produce documentación formal que sirve de entrada a la siguiente. | Media. Se sigue documentando (arquitectura, diseño), pero de forma incremental y con foco en lo que sustenta la iteración en curso. | Baja-media. El Manifiesto Ágil no elimina la documentación (el propio SWEBOK aclara que "los documentos son necesarios"), pero prioriza software funcionando y comunicación directa (cara a cara) sobre documentación exhaustiva. |

### Por qué esta comparación es central en la ingeniería de software

El SWEBOK subraya que la controversia histórica entre cascada y modelos ágiles debe entenderse en perspectiva: cada modelo surgió para resolver un problema de su época. La cascada introdujo **sistematización** en un momento en que el desarrollo de software era caótico (la llamada "crisis del software"), y sigue siendo válida en contextos con requisitos genuinamente estables y regulados (por ejemplo, sistemas críticos certificados). Los modelos iterativos y SCRUM surgieron para atender la realidad de que **los requisitos casi nunca son completamente conocidos de antemano**, y que el valor de negocio se entrega mejor en incrementos frecuentes y verificables.

El SWEBOK también advierte contra un malentendido común: **Agile no es "más rápido" que cascada por no producir documentación** —esa es una idea errónea que el propio texto señala explícitamente—; la diferencia real está en el *mindset*: cascada se enfoca en cumplir una especificación fijada de antemano, mientras que el mindset ágil se centra en comunicación constante, apertura al cambio y entrega continua de valor. Elegir entre estos modelos no es una cuestión de moda, sino una **decisión de ingeniería** que depende de qué tan bien conocidos y estables son los requisitos, del nivel de involucramiento posible del cliente, y del grado de riesgo que el proyecto puede tolerar — exactamente el tipo de análisis costo-beneficio que la KA 15 (Software Engineering Economics) exige aplicar a toda decisión de ingeniería de software.

### Fuente

Guide to the Software Engineering Body of Knowledge (SWEBOK), Version 4.0a, IEEE Computer Society Professional and Educational Activities Board.
