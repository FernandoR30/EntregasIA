## Resumenes
## Ingenieria del conocimiento
La Ingeniería de Conocimiento (IC) se define como una rama de la Inteligencia Artificial (IA) dedicada a la adquisición, representación y procesamiento del conocimiento para la construcción de Sistemas Expertos (SE) o Sistemas Basados en el Conocimiento (SBC). Su propósito central es capturar la experiencia de expertos humanos en dominios específicos y complejos —donde la informática convencional falla debido a la falta de estructura o a la imprecisión de los datos— y transformarla en una base de conocimiento inteligible para una computadora.

Los pilares de esta disciplina son el Ingeniero de Conocimiento (ICO), quien actúa como mediador y arquitecto del sistema, y el Experto Humano, fuente del conocimiento especializado. El proceso se articula a través de fases críticas que incluyen la adquisición, formalización, implementación y validación, utilizando diversos esquemas de representación que van desde la lógica simbólica y redes semánticas hasta estructuras de frames (marcos) y árboles de decisión.

Conceptos Fundamentales y Actores Clave
Para comprender la Ingeniería de Conocimiento, es preciso definir los elementos que la integran según la perspectiva de la IA:

El Conocimiento y sus Tipos

El conocimiento se interpreta como la combinación de estructuras de datos y procedimientos interpretativos que modelan el mundo real. Se clasifica en tres tipos principales:

Declarativo: Se expresa mediante hechos, atributos de objetos o conceptos y sus relaciones.
Procedural: Conjunto de reglas basadas en conocimiento que el experto emplea para resolver problemas.
Metaconocimiento: Conocimiento sobre el propio conocimiento y las capacidades de razonamiento del sistema (operación del motor de inferencia).
Roles Principales

Ingeniero de Conocimiento (ICO): Especialista informático que extrae el conocimiento del experto, conoce las herramientas de desarrollo y posee nociones de psicología para interpretar las manifestaciones del experto.
Experto Humano: Persona de reconocido prestigio que aporta su experiencia y saber hacer para ser integrados en el sistema.
Usuario: Persona final que utilizará el sistema; su nivel de conocimiento debe ser considerado durante el desarrollo.
El Proceso de la Ingeniería de Conocimiento
La IC puede definirse estrictamente como el ciclo de adquisición, representación, validación, inferenciación, explicación y mantenimiento del conocimiento. Su importancia radica en su capacidad para manejar dominios donde la información puede ser inconsistente, incompleta o mal estructurada.

Procesos Fundamentales

-Adquisición del Conocimiento (AC): Extracción de información de fuentes humanas o documentales.
-Representación del Conocimiento (KR): Codificación del conocimiento en una forma que la máquina pueda procesar.
-Base de Conocimiento: Repositorio donde la información se almacena, comúnmente mediante reglas de producción (implicaciones lógicas de causa-efecto).
-Validación: Asegurar que el sistema actúe con la misma fidelidad que el experto humano.
-Inferencia: Diseño del software que permite a la computadora realizar deducciones.
-Explicación y Justificación: Capacidad del sistema para mostrar al usuario el porqué de sus conclusiones.

Adquisición del Conocimiento (AC)

Este proceso busca comprender cómo un individuo realiza una actividad para automatizarla. Se nutre de dos tipos de fuentes:
-Estáticas (Secundarias): Conocimiento tangible e invariable (libros, revistas, artículos).
-Dinámicas (Primarias): Basadas en la experiencia cambiante del Experto Humano.

## Sistemas expertos basados en regla
Los sistemas basados en reglas (SBR) constituyen la metodología más sencilla y eficiente para abordar situaciones complejas de naturaleza determinista, como sistemas de control de tráfico, seguridad y transacciones bancarias. Estos sistemas operan mediante una base de conocimiento estática compuesta por reglas y una memoria de trabajo dinámica que almacena hechos. El motor de inferencia es el núcleo operativo que, aplicando lógica clásica y estrategias como el encadenamiento hacia adelante o hacia atrás, extrae conclusiones a partir de las premisas dadas. El éxito de estos sistemas depende críticamente del control de coherencia —para evitar contradicciones entre reglas y hechos— y de la capacidad de proporcionar explicaciones sobre las conclusiones alcanzadas. Si bien son herramientas robustas en entornos deterministas, su limitación reside en la incapacidad de la lógica clásica para gestionar la incertidumbre, lo que posiciona a los sistemas probabilísticos como su generalización necesaria.

Arquitectura de la Base de Conocimiento
El funcionamiento de un sistema experto basado en reglas se sustenta en la interacción de dos componentes principales:
-Hechos: Representan el conocimiento declarativo sobre una situación particular. Son de naturaleza dinámica y temporal, almacenándose en la memoria de trabajo del sistema.
-Reglas: Constituyen el conocimiento permanente y estático. Definen las relaciones generales entre objetos y gobiernan cómo se procesa la información. Se almacenan en la base de conocimiento.

Definición y Componentes de una Regla
Una regla es una afirmación lógica que relaciona dos o más objetos mediante la estructura: "Si premisa, entonces conclusión".
Premisa o Antecedente: Expresión lógica (simple o compuesta) que utiliza palabras clave como si y operadores lógicos (y, o, no).
Conclusión o Consecuente: Expresión lógica que sigue a la palabra clave entonces.
Restricciones y Sustitución de Reglas

Para facilitar la programación, algunos sistemas imponen restricciones, como prohibir el operador o en la premisa o limitar las conclusiones a expresiones simples. Sin embargo, esto no implica pérdida de generalidad gracias a la sustitución de reglas, donde una regla compleja se reemplaza por un conjunto equivalente de reglas simples.

Regla Original Reglas Equivalentes Si A o B, entonces C Si A, entonces C; Si B, entonces C Si A, entonces B y C Si A, entonces B; Si A, entonces C Si (A o B) y C, entonces D Si A y C, entonces D; Si B y C, entonces D