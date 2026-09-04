1. Técnica elegida

    La técnica elegida para conocer al grupo de usuarios primarios identificado en el TP 1 es la **encuesta** o **cuestionario**. Decidimos elegir esta técnica dado que nuestro grupo de usuarios es muy grande y tienen una diversidad académica considerable. Ya que nuestro proyecto se encarga de centralizar los eventos de los distintos departamentos, consideramos que el uso de las encuestas para conocer la satisfacción de muchos de estos nos otorgará información muy precisa con respecto a lo que los usuarios quieren.

2. Instrumento

    Cuestionario autoadministrado de **19 preguntas** distribuido por formulario web, en cuatro bloques: perfil (1–5), interés y conducta (6–8, escalas 1–5), hábitos de información (9–13) y fricción y expectativa (14–19). La guía de preguntas completa y las respuestas crudas están versionadas como evidencia en `docs/evidencia/tp2/`.

    Una decisión de diseño condicionó lo que se pudo encontrar: **el interés por los eventos del propio departamento y por los de los demás se preguntaron por separado** (6 y 7), en lugar de asumir que eran igual de altos. Es la pregunta que termina refutando el recorte del supuesto crítico. También se preguntó el motivo de perderse un evento como multiselección (15), lo que permitió separar tres problemas distintos, y se incluyó una pregunta abierta opcional (17) que aportó 9 respuestas.

    **Nota.** La pregunta 4 (*Rol*) se incorporó con la encuesta ya en curso: las 10 primeras respuestas la tienen vacía. Se las cuenta igualmente como alumnos porque respondieron desde una casilla `@alumno.unlam.edu.ar` y declaran año de carrera, cosa que ningún docente hizo.

3. Análisis de los resultados

    **Ficha del relevamiento.** Encuesta respondida el 30 y 31 de agosto de 2026. **22 respuestas: 20 de alumnos** —el grupo primario, al que estaba dirigido el relevamiento— y 2 de docentes, espontáneas. **El análisis se hace sobre las 20 respuestas de alumnos**: los docentes son grupo secundario no relevado, y dos respuestas incidentales no constituyen evidencia sobre ese grupo. Cada respondente se identifica como **U1** a **U22**; no se consignan nombres ni direcciones de correo.

    **Limitaciones.** Las 20 respuestas provienen todas del **DIIT, carrera de Ingeniería en Informática**: nada puede extrapolarse al resto de la universidad. **No respondió ningún administrativo**, uno de los tres grupos de usuarios del brief. Y **5 de los respondentes son integrantes de este equipo**, lo que introduce un sesgo de proximidad al problema.

    **3.1. Perfil del usuario**

    Estudiante de **Ingeniería en Informática del DIIT, de 21 a 27 años** (18 de 20; los extremos son 17 y 39), **cursando entre 3.º y 5.º año** (17 de 20). Lo define la **distancia entre lo que le interesa y lo que hace**:

    - Le interesan los eventos de su departamento: **3,60 sobre 5**, con 12 de 20 respondiendo 4 o 5.
    - Casi no asiste: **1,95 sobre 5**. El valor más alto que eligió alguien es 3; **ningún alumno respondió 4 ni 5**.
    - **8 de 20 combinan interés alto (4–5) con asistencia baja (1–2)**: gente que quiere ir y no va.

    Es **pasivo en la búsqueda**: 12 de 20 buscan información sobre eventos "Nunca" o solo "Esporádicamente". **U6**: *"los medios de comunicación oficial suelen tener la información, pero es raro que los revise… no voy a estar revisando múltiples medios en busca de que aparezca un evento"*.

    Su dieta informativa es **mayoritariamente informal**: 16 de 20 se enteran por Instagram y otros 16 por un canal informal —WhatsApp, Discord o un compañero—. **3 alumnos no usan ningún canal institucional.**

    **3.2. Necesidades reales**

    1. **Un único lugar donde esté todo** — única respuesta unánime: **20 de 20**. Hoy la información está repartida en 10 canales, 3,7 por alumno, y 14 de 20 usan 3 o más.
    2. **Que la información los alcance en vez de tener que buscarla** — con 12 de 20 que casi nunca buscan, toda solución que dependa de que el usuario entre a consultar reproduce el problema actual.
    3. **Enterarse con tiempo para poder ir** — antelación percibida **2,05 sobre 5**; *"apareció demasiado cerca de la fecha"* es el segundo motivo más marcado (**11 de 20**).
    4. **Información completa, no solo el aviso** — **U22**: *"la información provista en las publicaciones suelen ser escazas o poco claras, y es dificil encontrar detalles adicionales"*; **U13**: *"no profundizan tanto como para generar un interés"*.
    5. **Relevancia filtrada** — el interés se concentra en el propio departamento (3,60) frente a los demás (2,20).

    **3.3. Problemas y frustraciones concretas**

    **13 de 20 quisieron ir a un evento y no pudieron** porque no se enteraron a tiempo o no encontraron la información. Los motivos que marcaron no son un problema sino **tres distintos**, que no se resuelven con la misma funcionalidad:

    | Problema | Motivo marcado | Frec. | Qué falla |
    |---|---|---|---|
    | **Alcance** | "No vi la publicación." | **15 / 20** | La publicación existió y no llegó. **No es un problema de centralización**: centralizar no sirve si el usuario nunca mira dónde se centralizó. |
    | **Oportunidad** | "Apareció demasiado cerca de la fecha." | **11 / 20** | Llegó tarde para organizarse. |
    | **Dispersión — hallazgo** | "No sabía dónde buscar." | **8 / 20** | No hay un lugar canónico identificable. |
    | **Dispersión — fragmentación** | "Estaba distribuida en distintos canales." | **8 / 20** | Hay que reconstruirla juntando pedazos. |

    Las respuestas abiertas ponen palabras a la fragmentación: *"Hay información esparcida por muchos canales diferentes"* (**U5**); *"uno se pierde al buscar la información"* (**U22**). Y **U10** expone la dependencia de un canal ajeno a la universidad: *"si no fuese porque los tengo en instagram, no me enteraría de casi nada"*. La eficiencia percibida de la comunicación de la UNLaM promedia **2,50 sobre 5**, con 10 de 20 puntuándola en 1 o 2.

    **3.4. Contexto de uso**

    - **Dispositivo:** celular, 19 de 20, y **8 no usan ningún otro**. Computadora 12, tablet 1.
    - **Momento:** no hay uno. Con 12 de 20 que casi nunca buscan, el consumo es incidental —mientras usan el teléfono para otra cosa, entre clases o fuera de la facultad—. El producto no compite por un rato reservado.
    - **Condición:** apurados y en modo pasivo. El primer impacto decide: el motivo más marcado es no haber visto la publicación (15 de 20), no que no interesara.
    - **Compañía:** la información circula por rebote social — 9 se enteran por un compañero, 8 por un docente, 13 participan de grupos de WhatsApp y 5 de Discord.
    - **Conectividad: no se relevó.** No afirmamos nada sobre uso sin conexión.
    - **Barrera que no es de información:** **U12** y **U19** señalan que los eventos **se superponen con su horario de cursada**. Se retoma en 4.1.

4. Confrontación de los supuestos del TP1

    **Criterio.** El relevamiento se dirigió al **grupo primario (alumnos)**. Los supuestos que aplican a grupos no relevados —docentes, secundario; administrativos, que no respondieron— se clasifican **Sin evidencia**: dos respuestas docentes espontáneas no constituyen evidencia sobre ese grupo.

    | # | Supuesto del TP1 | ¿Se confirmó? | Evidencia |
    |---|---|---|---|
    | **1** *(crítico)* | Estudiantes y docentes tienen dificultades para enterarse de los eventos **de otros departamentos**. | **Refutado** en su recorte (alumnos) · **Sin evidencia** (docentes) | La dificultad existe, pero no ahí. Interés en otros departamentos **2,20 / 5**: 13 de 20 responden 2 o menos, **ninguno responde 5**, solo 2 responden 4. Y el dato decisivo: **ningún alumno declara más interés por los eventos de otros departamentos que por los del propio** (0 de 20; 15 lo invierten, 5 empatan). Sobre los eventos propios el problema sí está: interés 3,60, asistencia 1,95, 13 de 20 se perdieron un evento. |
    | **2** | La información está dispersa entre distintos canales. | **Confirmado** | 10 canales en uso, **3,7 por alumno**, 14 de 20 usan 3 o más. 8 de 20 marcan que estaba distribuida y otros 8 que no sabían dónde buscar. **U5**: *"Hay información esparcida por muchos canales diferentes"*. |
    | **3** | Los docentes consideran útil compartir eventos con sus cátedras. | **Sin evidencia** | Grupo secundario, no relevado. Además **el cuestionario no preguntó sobre difundir ni compartir**: no hay dato ni a favor ni en contra. Requiere entrevista. |
    | **4** | El personal administrativo necesita una herramienta centralizada de carga y gestión. | **Sin evidencia** | **Ningún administrativo respondió** y el instrumento no estaba diseñado para ellos. |
    | **5** | La información centralizada aumentaría la participación. | **Sin evidencia** | El supuesto es sobre **participación**, y no se midió antes y después: la comparación que el TP1 planteaba nunca se hizo. El dato cercano —20 de 20 querrían un solo lugar— mide deseo, no conducta, y es una pregunta sin poder discriminante. |
    | **6** | Los alumnos prefieren notificarse por herramientas de la cursada antes que por externas. | **Confirmado** | **16 de 20 aceptarían** ser notificados por MS Teams, que es la plataforma de uso cotidiano durante la cursada. La salvedad: el cuestionario preguntó por Teams por sí o por no, sin ofrecer una alternativa externa contra la cual compararlo, así que lo respaldado es la aceptación y no la preferencia. |

    **4.1. ¿Qué apareció que no habíamos previsto?**

    - **Nadie asiste seguido, ni los más interesados.** La asistencia tiene techo 3: ningún alumno respondió 4 ni 5. Hay una barrera *además* de la información, que ningún supuesto contemplaba.
    - **Superposición horaria con la cursada.** **U12** y **U19** la mencionan sin que se preguntara —2 de las 9 respuestas abiertas—: *"suelen poner los eventos en horarios en los que tengo clase y no puedo asisitir"*. Es una barrera de agenda y **ninguna funcionalidad del brief la resuelve**.
    - **La calidad de la publicación, no solo su llegada** (**U13**, **U22**): el evento puede llegar y aun así no alcanzar para decidir.
    - **Canales informales que la universidad no controla:** WhatsApp (13 de 20) y Discord (5 de 20), ausentes del brief.
    - **Un problema de encuadre:** **U18** marcó *"no sabía que el evento era de mi interés"*. El aviso llegó y no fue reconocido como propio.
    - **Hay rechazo a ser notificado:** 4 de 20 no quieren notificaciones, en tensión con la funcionalidad 3 del brief.

    **4.2. ¿Qué pasó con el supuesto crítico?**

    **Se cayó el recorte, no el problema.** El problema existe y está documentado: 13 de 20 se perdieron eventos que querían ver. Lo que se cayó es *dónde* lo ubicaba el TP1: los eventos de otros departamentos casi no le interesan a nadie —2,20 de promedio, ninguna respuesta en 5, cero alumnos que los prioricen—. **El problema es intradepartamental.** La única voz en contra es un alumno que sí lo reclama: *"hay eventos de otros departamentos que abordan escenarios interesantes de la informática desde sus perspectivas (como IA) pero al no seguir a otros departamentos en Instagram no me entero de ellos"* (**U3**). Es 1 de 20, y no mueve el promedio. Qué implica:

    - **La funcionalidad 4 —compartir a una cátedra de otro departamento— se queda sin sustento.** Se apoyaba en que esos eventos interesaran (refutado) y en que los docentes quisieran difundirlos (sin evidencia).
    - **La funcionalidad 3 —filtro y segmentación— pasa de antisaturación a núcleo:** es lo que hace que llegue lo del propio departamento, que es lo único que este usuario quiere.
    - **La alerta deja de ser una funcionalidad más y pasa a ser el eje.** El brief ya preveía notificación segmentada, pero como una pieza entre cuatro. El problema número uno es *"no vi la publicación"* (15 de 20) y 12 de 20 no buscan: la consulta sigue siendo necesaria, pero **este usuario no llega a ella por iniciativa propia**. Conviene invertir el orden de prioridades del brief. *(El canal concreto de la alerta se analiza en el brief, §4.)*

    Que tres de los seis supuestos hayan quedado sin evidencia y otro refutado no invalida el TP1: se escribieron para ponerlos a prueba, y eso reveló que el producto apuntaba a un problema más chico que el que los usuarios tienen.

    **4.3. ¿El usuario primario sigue siendo el correcto?**

    **Sí, siguen siendo los alumnos**, con dos correcciones y una advertencia.

    - **De alcance.** El brief decía "alumnos de cualquier carrera de grado". Todo lo relevado es de **Ingeniería en Informática del DIIT** y 17 de 20 cursan entre 3.º y 5.º año. Ampliarlo requiere relevar otras carreras.
    - **De descripción.** El brief decía que el alumno "se pierde eventos de su propio departamento y no se entera de actividades de otros departamentos". La primera mitad está confirmada; **la segunda hay que borrarla**.
    - **No es una comparación ganada.** La encuesta no puede decir si otro grupo tiene el problema más fuerte, porque **solo relevó al primario**. Mantener a los alumnos es *consistente* con lo encontrado, no el resultado de haber medido y comparado los tres grupos.

5. Hipótesis de valor

    > **Creemos que** el alumno de Ingeniería en Informática del DIIT que cursa entre 3.º y 5.º año, se informa por el celular y no busca información de eventos por su cuenta,
    >
    > **tiene el problema de** perderse eventos **de su propio departamento** que sí le interesan, porque el aviso no le llega o le llega demasiado cerca de la fecha,
    >
    > **Nuestra solución es** una plataforma que centraliza los eventos y **se los empuja al celular** filtrados por su carrera y año, con antelación suficiente y con la información completa para decidir, dejando la inscripción a un toque desde esa misma alerta.
    >
    > **Sabremos que estamos en lo correcto cuando**, tras un cuatrimestre de uso, los alumnos que reportan *"no vi la publicación"* bajen del **75 % actual a menos del 30 %**, el **80 % de las alertas** se entregue con **7 días o más** de anticipación, y aparezcan las primeras respuestas de asistencia en **4 y 5** de la escala, hoy inexistentes.

    **Trazabilidad.** Cada parte con el dato del relevamiento que la sostiene:

    | Parte | Dato que la sostiene |
    |---|---|
    | **Usuario** | Ing. en Informática del DIIT, 17 de 20 cursan 3.º–5.º.<br>Se informa por celular: 19 de 20.<br>No busca por su cuenta: 12 de 20. |
    | **Problema** | Interés **3,60** contra asistencia **1,95**, sin ninguna respuesta en 4 ni 5.<br>Se perdieron un evento: **13 de 20**.<br>*"No vi la publicación"*: **15 de 20**; *"demasiado cerca de la fecha"*: **11 de 20**.<br>Interés en otros departamentos **2,20**, con cero alumnos que lo prioricen. |
    | **Solución** | Un solo lugar: **20 de 20**.<br>Empujar en vez de esperar la consulta: 12 de 20 no buscan.<br>Filtrar: **3,60** eventos propios contra **2,20** de eventos ajenos. |
    | **Evidencia medible** | Líneas de base de agosto 2026: *"no vi la publicación"* **15 de 20 (75 %)**, antelación **2,05 / 5**, y asistencia sin ninguna respuesta en 4 ni 5.<br>Se remiden con las mismas preguntas, así que la comparación es directa. |

---

Evidencia: https://github.com/gadsii-unlam/gadsii-TicTac/tree/main/docs/evidencia/tp2
