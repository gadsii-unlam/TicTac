1. Técnica elegida para poder conocer al grupo de usuarios primarios identificado en el TP 1 es **encuesta** o **cuestionario**. Decidimos elegir esta técnica dado que nuestro grupo de usuarios es muy grande y tienen una diversidad académica considerable. Ya que nuestro proyecto se encarga de centralizar los eventos de los distintos departamentos, consideramos que el uso de las encuestas para conocer la satisfacción de muchos de estos nos otorgará información muy precisa con respecto a lo que los usuarios quieren.

2. Instrumento

    Cuestionario autoadministrado de **19 preguntas**, distribuido por formulario web. La guía de preguntas completa y las respuestas crudas están versionadas como evidencia en `docs/evidencia/tp2/` (`guia-de-preguntas.md` y `resultados-encuesta.xlsx`); acá se describe qué se preguntó y con qué intención.

    Las preguntas se agruparon en cuatro bloques, cada uno apuntando a algo que el TP1 había dado por supuesto:

    | Bloque | Preguntas | Qué buscaba medir |
    |---|---|---|
    | **Perfil** | 1–5 | Edad, departamento, carrera, rol y año de cursada. Sirve para saber a quién estábamos escuchando realmente y para poder segmentar después entre alumnos y docentes. |
    | **Interés y conducta** | 6–8 | Escalas 1–5 de interés en los eventos del propio departamento y en los de los demás, más frecuencia de asistencia. El cruce entre las tres es lo que permite ver si hay brecha entre lo que dicen que les interesa y lo que efectivamente hacen. |
    | **Hábitos de información** | 9–13 | Por qué canales se enteran, con qué frecuencia buscan por su cuenta, con cuánta antelación se enteran y en qué dispositivos. Apunta al supuesto de dispersión de canales y al contexto de uso. |
    | **Fricción y expectativa** | 14–19 | Si alguna vez se perdieron un evento y por qué motivo, qué tan eficiente les parece la comunicación actual, una pregunta abierta, y si querrían un único lugar y notificaciones por plataforma académica. |

    Tres decisiones de diseño del cuestionario que conviene dejar registradas, porque condicionan lo que se pudo encontrar:

    - **El interés propio y el ajeno se preguntaron por separado** (6 y 7) en lugar de asumir que eran igual de altos. Es la pregunta que termina refutando el recorte del supuesto crítico (punto 4).
    - **El motivo de perderse un evento se preguntó como multiselección** (15), con opciones que distinguen alcance, oportunidad y dispersión, en vez de forzar una única causa. Sin eso no habríamos podido separar los tres problemas del punto 3.3.
    - **Se incluyó una pregunta abierta opcional** (17). Aportó 9 respuestas y es de donde salen las citas del análisis, incluidas dos condiciones de uso que ningún supuesto había previsto.

3. Análisis de los resultados

    **Ficha del relevamiento.** Encuesta autoadministrada por formulario web, respondida entre el 30 y el 31 de agosto de 2026. Se recibieron **22 respuestas**: **20 de alumnos** —el grupo primario, al que estaba dirigido el relevamiento— y 2 de docentes, que llegaron de manera espontánea.

    **El análisis se hace sobre las 20 respuestas de alumnos.** Los docentes son un grupo secundario que no fue objeto de este relevamiento: dos respuestas incidentales no constituyen evidencia sobre ese grupo, y por eso no se usan para sostener ni para refutar ningún supuesto que los involucre (ver punto 4). Donde se los menciona es de manera descriptiva y está señalado. Cada respondente se identifica como **U1** a **U22** según su número en la planilla de resultados; el análisis no consigna nombres ni direcciones de correo.

    **Limitaciones de la muestra, declaradas por adelantado:**

    - Las 20 respuestas de alumnos provienen del **Departamento de Ingeniería e Investigaciones Tecnológicas**, y todas de la carrera de **Ingeniería en Informática**. No hay una sola respuesta de otro departamento ni de otra carrera. Nada de lo que sigue puede extrapolarse al resto de la universidad.
    - **No respondió ningún administrativo**, que es uno de los tres grupos de usuarios definidos en el brief.
    - **5 de los respondentes son integrantes de este equipo**, lo que introduce un sesgo de proximidad al problema que ya teníamos identificado antes de preguntar.

    ---

    **3.1. Perfil del usuario**

    El usuario que efectivamente relevamos es un **estudiante de Ingeniería en Informática del DIIT, de entre 21 y 27 años** (18 de los 20 caen en esa franja; los extremos son 17 y 39), **cursando entre 3.º y 5.º año** (17 de 20).

    El rasgo que lo define no es el desinterés, sino la **distancia entre lo que le interesa y lo que hace**:

    - Le interesan los eventos de su propio departamento: promedio **3,60 sobre 5**, con 12 de 20 respondiendo 4 o 5.
    - Pero casi no asiste: promedio **1,95 sobre 5**. El valor más alto que eligió alguien es 3. **Ningún alumno respondió 4 ni 5.**
    - **8 de 20 combinan interés alto (4–5) con asistencia baja (1–2)**: es el núcleo del problema, gente que quiere ir y no va.

    Y es un usuario **pasivo en la búsqueda**: 12 de los 20 declaran que buscan información sobre eventos "Nunca" o solo "Esporádicamente". No es alguien que vaya a entrar a un portal a ver qué hay. Se entera si la información lo alcanza, y si no, no se entera. **U6** lo dice sin rodeos: *"los medios de comunicación oficial suelen tener la información, pero es raro que los revise, más que nada porque no voy a estar revisando múltiples medios en busca de que aparezca un evento"*.

    Su dieta informativa es **mayoritariamente informal**: 16 de 20 se enteran por Instagram (oficial o no oficial) y otros 16 por algún canal informal —grupos de WhatsApp, servidores de Discord o un compañero—. **3 alumnos no usan ningún canal institucional**: para ellos, MIeL, la web de la universidad y Teams sencillamente no existen como fuente de eventos.

    ---

    **3.2. Necesidades reales**

    Qué necesitan que hoy no tienen, o que tienen de forma deficiente:

    1. **Un único lugar donde esté todo.** Es la única respuesta unánime de la encuesta: **20 de 20** responden que sí. Hoy la información existe, pero repartida en 10 canales distintos, con un promedio de 3,7 canales por alumno y 14 de 20 usando 3 o más.
    2. **Que la información los alcance, en vez de tener que ir a buscarla.** Es la necesidad que el perfil vuelve inevitable: con 12 de 20 que casi nunca buscan, cualquier solución que dependa de que el usuario entre a consultar reproduce el problema actual. Necesitan entrega activa, no un repositorio.
    3. **Enterarse con tiempo suficiente para poder ir.** La antelación percibida promedia **2,05 sobre 5**, y "la publicación apareció demasiado cerca de la fecha" es el segundo motivo más marcado (**11 de 20**). Enterarse tarde equivale a no enterarse.
    4. **Información completa, no solo el aviso.** Aparece en las respuestas abiertas: **U22** señala que *"la información provista en las publicaciones suelen ser escazas o poco claras, y es dificil encontrar detalles adicionales"*, y **U13** que *"la comunicación es muy vaga, si bien lo suelen difundir por redes, no profundizan tanto como para generar un interés"*. No basta con que el evento llegue: tiene que llegar con lo necesario para decidir si vale la pena ir.
    5. **Relevancia filtrada.** El interés está fuertemente concentrado en el propio departamento (3,60) frente a los demás (2,20). Necesitan que lo que les llegue sea de lo suyo, no un caño de todo lo que pasa en la universidad.

    ---

    **3.3. Problemas y frustraciones concretas**

    **El dato de cabecera: 13 de 20 quisieron ir a un evento y no pudieron** porque no se enteraron a tiempo o no encontraron la información. No es un problema hipotético: ya les pasó.

    Los motivos que marcaron no son un solo problema, sino **tres problemas distintos** que conviene no mezclar, porque no se resuelven con la misma funcionalidad:

    | Problema | Motivo marcado | Frecuencia | Qué falla realmente |
    |---|---|---|---|
    | **Alcance** | "No vi la publicación." | **15 / 20** | La publicación existió y no llegó. Es el motivo más frecuente y **no es un problema de centralización**: centralizar no sirve si el usuario nunca mira el lugar donde se centralizó. |
    | **Oportunidad** | "La publicación apareció demasiado cerca de la fecha." | **11 / 20** | Llegó, pero tarde para poder organizarse. |
    | **Dispersión — hallazgo** | "No sabía dónde buscar la información." | **8 / 20** | No hay un lugar canónico identificable. |
    | **Dispersión — fragmentación** | "La información estaba distribuida en distintos canales." | **8 / 20** | Está repartida y hay que reconstruirla juntando pedazos. |

    Las respuestas abiertas ponen palabras a la fragmentación: *"Hay información esparcida por muchos canales diferentes"* (**U5**); *"Hay muchos medios de comunicación posibles, y uno se pierde al buscar la información"* (**U22**); *"A veces están tan distrubuidos que no llego a enterarme"* (**U3**).

    La dependencia de un canal ajeno a la universidad queda expuesta en el comentario de **U10**: *"si no fuese porque los tengo en instagram, no me enteraría de casi nada"*. La difusión funciona hoy porque el estudiante, por su cuenta, decidió seguir una cuenta de Instagram. Quien no lo hizo, queda afuera.

    Y hay un problema de **puntería**, no de volumen, señalado por **U14**: *"se comunican de forma correcta pero falta que la informacion comunicada llegue mas frecuentemente al publico objetivo correcto"*.

    Todo esto se refleja en la evaluación general: la eficiencia de la comunicación de eventos de la UNLaM promedia **2,50 sobre 5**, con **10 de 20 puntuándola en 1 o 2** y un solo alumno por encima de 3.

    ---

    **3.4. Contexto de uso**

    - **Dispositivo: el celular, de manera abrumadora.** 19 de 20 se enteran por celular, y **8 lo usan como único dispositivo**. 12 mencionan también la computadora y 1 la tablet. Cualquier diseño que asuma pantalla grande deja afuera a casi la mitad de los relevados.
    - **Momento: sin momento.** No hay una instancia dedicada a informarse. Con 12 de 20 que buscan "Nunca" o "Esporádicamente", el consumo ocurre de manera incidental —mientras usan el teléfono para otra cosa—, entre clases, viajando o fuera de la facultad. El producto no compite por un rato reservado: tiene que aparecer dentro del uso que el estudiante ya hace del celular.
    - **Condición: apurados y en modo pasivo.** El usuario no llega con tiempo ni con intención de explorar. Esto vuelve decisivo el primer impacto: si el aviso no se entiende en una lectura rápida, se pierde. Lo respalda que el motivo más marcado sea "no vi la publicación" (15 de 20) y no "no me interesó".
    - **Compañía: la información circula por rebote social.** 8 se enteran por un docente y 9 por un compañero de la carrera; 13 participan de grupos de WhatsApp y 5 de servidores de Discord. La difusión efectiva hoy pasa tanto por la red de pares como por el canal oficial.
    - **Sobre la conectividad:** la encuesta **no relevó** condiciones de conectividad. No tenemos evidencia para afirmar nada sobre uso sin conexión, y no lo damos por supuesto.
    - **Una condición de contexto que no es de información:** dos respuestas (**U12** y **U19**) señalan que los eventos **se superponen con su horario de cursada** —*"suelen poner los eventos en horarios en los que tengo clase y no puedo asisitir"*—. Enterarse a tiempo no alcanza si el evento cae cuando el estudiante está en el aula. Se retoma en el punto 4.

4. Confrontación de los supuestos del TP1

    **Criterio de clasificación.** El relevamiento se dirigió al **grupo primario (alumnos)**. Los supuestos que aplican a grupos que no fueron objeto del relevamiento —docentes, que son grupo secundario, y personal administrativo, que directamente no respondió— se clasifican **Sin evidencia**, aun cuando dos docentes hayan respondido de manera espontánea: dos respuestas incidentales de un grupo que no se relevó no constituyen evidencia sobre ese grupo. Cuando un supuesto abarca a los dos grupos a la vez, se indica qué parte quedó respaldada y qué parte quedó sin evidencia.

    | # | Supuesto del TP1 | ¿Se confirmó? | Evidencia que lo sostiene o lo refuta |
    |---|---|---|---|
    | **1** *(crítico)* | Los estudiantes y docentes tienen dificultades para enterarse de los eventos académicos **de otros departamentos**. | **Refutado** en su recorte, para alumnos. **Sin evidencia** para docentes. | La dificultad existe, pero no está donde el supuesto la ubicaba. El interés en los eventos de otros departamentos promedia **2,20 sobre 5**; 13 de 20 responden 2 o menos, **ningún alumno responde 5** y solo 2 responden 4. Y el dato que cierra la discusión: **ningún alumno declara más interés por los eventos de otros departamentos que por los del propio** (0 de 20; 15 lo invierten y 5 empatan). En cambio, sobre los eventos propios el problema sí está: interés **3,60**, asistencia **1,95**, **13 de 20 se perdieron un evento** y el motivo más marcado es *"no vi la publicación"* (15 de 20). |
    | **2** | La información de los eventos está dispersa entre distintos canales. | **Confirmado** | 10 canales distintos en uso, **3,7 por alumno**, y 14 de 20 usan 3 o más. 8 de 20 marcan *"la información estaba distribuida en distintos canales"* y otros 8 *"no sabía dónde buscar la información"*. **U5**: *"Hay información esparcida por muchos canales diferentes"*. **U22**: *"Hay muchos medios de comunicación posibles, y uno se pierde al buscar la información"*. |
    | **3** | Los docentes consideran útil compartir eventos relevantes con los alumnos de sus cátedras. | **Sin evidencia** | Los docentes son grupo secundario y no fueron objeto del relevamiento. A eso se suma que **el cuestionario no incluyó ninguna pregunta sobre difundir o compartir**: no hay dato ni a favor ni en contra. Requiere una entrevista específica a docentes. |
    | **4** | El personal administrativo necesita una herramienta centralizada para cargar y gestionar los eventos de su departamento. | **Sin evidencia** | **Ningún administrativo respondió la encuesta.** El grupo no fue relevado y el instrumento tampoco estaba diseñado para él. |
    | **5** | Contar con información centralizada aumentaría la participación de estudiantes y docentes en los eventos. | **Sin evidencia** | El supuesto es sobre **participación**, y la participación no se midió antes y después de nada: la comparación que el propio TP1 planteaba como evidencia nunca se hizo. El único dato cercano es que **20 de 20 querrían tener todo en un solo lugar**, pero eso mide *deseo*, no conducta, y es una pregunta sin poder discriminante —nadie iba a responder que no—. Para docentes, además, sin evidencia por grupo secundario. |
    | **6** | Los alumnos prefieren notificarse por herramientas de uso cotidiano durante la cursada antes que por herramientas externas. | **Parcialmente confirmado** | **16 de 20 aceptarían** ser notificados por MS Teams: eso sí está respaldado. Pero la **preferencia comparada nunca se preguntó** —el cuestionario ofrecía Teams por sí o por no, nunca contra una alternativa—, así que el "antes que" queda sin evidencia. Y la premisa de que las plataformas académicas sean las herramientas cotidianas **se cae**: Teams es canal actual de solo 3 de 20 y MIeL de 6, frente a Instagram con 16 y WhatsApp con 13. |

    ---

    **4.1. ¿Qué apareció que no habíamos previsto?**

    - **Nadie asiste seguido, ni siquiera los más interesados.** La asistencia tiene techo 3: **ningún alumno respondió 4 ni 5**. Y 8 de 20 combinan interés alto con asistencia baja. Ningún supuesto del TP1 contemplaba que pudiera haber una barrera *además* de la información, pero los datos dicen que la hay.
    - **Superposición horaria con la cursada.** **U12** y **U19** lo mencionan espontáneamente en la pregunta abierta —2 de las 9 que la respondieron—: *"suelen poner los eventos en horarios en los que tengo clase y no puedo asisitir"*. Es una barrera de agenda, no de información, y **ninguna de las cuatro funcionalidades del brief la resuelve**.
    - **La calidad de la publicación, no solo su llegada.** **U13**: *"la comunicación es muy vaga… no profundizan tanto como para generar un interés"*. **U22**: *"la información provista en las publicaciones suelen ser escazas o poco claras"*. El evento puede llegar y aun así no alcanzar para decidir si vale la pena ir.
    - **Canales informales que la universidad no controla.** WhatsApp (13 de 20) y Discord (5 de 20) son parte central de la difusión real. El brief nombraba sitio web, calendario, redes oficiales, centros de estudiantes y docentes; no contemplaba que buena parte de lo que funciona hoy pase por canales ajenos a la institución.
    - **Un problema de encuadre, no de difusión.** **U18** marcó *"no sabía que el evento era de mi interés"*: el aviso llegó y no fue reconocido como propio. Es un modo de fallar distinto a no enterarse.
    - **Hay rechazo a ser notificado.** 4 de 20 alumnos responden que **no** quieren notificaciones por plataforma académica. Es minoría, pero está en tensión directa con la funcionalidad 3 del brief, que da por sentado que la notificación es bienvenida mientras esté segmentada.

    ---

    **4.2. ¿Qué pasó con el supuesto crítico?**

    **Se cayó el recorte, no el problema.** Hay un problema real y está documentado: 13 de 20 se perdieron eventos que querían ver. Lo que se cayó es *dónde* el TP1 lo ubicaba. El supuesto decía que la dificultad estaba en enterarse de los eventos **de otros departamentos**, y el relevamiento muestra que esos eventos casi no le interesan a nadie: 2,20 de promedio, ninguna respuesta en 5, y cero alumnos que los prioricen por encima de los propios. **El problema es intradepartamental.**

    Qué implica para el producto:

    - **La funcionalidad 4 —compartir un evento a una cátedra de otro departamento— se queda sin sustento.** Se apoyaba en dos cosas: que los eventos de otros departamentos interesaran (refutado) y que los docentes quisieran difundirlos (sin evidencia). Hoy es la funcionalidad más débil del brief y no debería construirse antes de relevar docentes.
    - **La funcionalidad 3 —filtro y segmentación— cambia de papel.** En el brief era un antisaturación: evitar que un alumno de Ingeniería reciba lo de Humanidades. Con estos datos deja de ser una salvaguarda y pasa a ser **el core**: la segmentación es lo que hace que llegue lo del propio departamento, que es lo único que este usuario quiere.
    - **La alerta deja de ser una funcionalidad más y pasa a ser el eje del producto.** El brief ya preveía notificación segmentada (funcionalidad 3) y el envío por Teams, pero como una pieza entre cuatro. La evidencia la asciende a mecanismo central: el problema número uno es *"no vi la publicación"* (15 de 20) y 12 de 20 no buscan nunca o casi nunca. La parte de consulta —ver el listado, abrir la ficha, inscribirse— sigue siendo necesaria, pero **este usuario no va a llegar a ella por iniciativa propia**: la alerta es lo que lo trae, y la centralización es lo que hace que la alerta tenga algo completo para traer. Conviene invertir el orden de prioridades del brief.

    **Sobre el canal de la alerta.** La decisión entre aplicación móvil (notificación push) y aplicación web (notificación por mail o WhatsApp) sigue abierta. El cuestionario no preguntó por canal salvo Teams, así que no la resuelve, pero la acota bastante:

    - **Tiene que llegar al celular.** 19 de 20 se enteran de eventos ahí y **8 no usan ningún otro dispositivo**. Una alerta que dependa de estar frente a la computadora deja afuera a casi la mitad del público.
    - **WhatsApp es el canal no institucional más instalado**: 13 de 20 ya reciben información de eventos por grupos. Es la opción con menor fricción de adopción, porque no exige instalar ni revisar nada nuevo.
    - **El mail es la más débil de las tres opciones.** **Ningún alumno menciona el correo** entre los canales por los que hoy se entera de eventos; la única mención en todo el relevamiento es de un docente, y los docentes no cuentan como evidencia. Elegir mail sería apostar a un canal que este usuario hoy no usa para esto.
    - **Teams tiene aceptación declarada, no hábito.** 16 de 20 dirían que sí, pero solo 3 lo mencionan como canal actual. Que lo acepten no significa que lo miren.
    - **Cualquiera sea el canal, hace falta control.** 4 de 20 no quieren ser notificados. La alerta necesita frecuencia configurable y posibilidad de baja, o el producto va a molestar a una quinta parte de su propio público.

    Que tres de seis supuestos hayan quedado sin evidencia y uno refutado no invalida el TP1: los supuestos se escribieron para ponerlos a prueba, y ponerlos a prueba es lo que reveló que el producto estaba orientado hacia un problema —la dispersión entre departamentos— más chico que el que los usuarios efectivamente tienen.

    ---

    **4.3. ¿El usuario primario elegido en el TP1 sigue siendo el correcto?**

    **Sí, siguen siendo los alumnos**, con dos correcciones de definición y una advertencia metodológica.

    - **Corrección de alcance.** El brief decía "alumnos activos de cualquier carrera de grado de la UNLaM". Todo lo relevado proviene de **Ingeniería en Informática del DIIT**, y 17 de 20 cursan entre 3.º y 5.º año. El usuario primario que podemos sostener con evidencia es ese, no el general. Ampliarlo requiere relevar otras carreras.
    - **Corrección de descripción.** El brief caracterizaba al alumno como alguien que "se pierde eventos de su propio departamento y no se entera de actividades de otros departamentos que pueden ser complementarias a su formación". La primera mitad está confirmada; **la segunda hay que borrarla**.
    - **Advertencia: esto no es una comparación ganada.** La encuesta no puede decir si otro grupo tiene el problema más fuerte, porque **solo relevó al grupo primario**. No hay administrativos y los docentes son secundarios. Mantener a los alumnos como primario es *consistente* con lo que encontramos —son quienes muestran la brecha entre interés y asistencia, y quienes reportan haberse perdido eventos—, pero no salió de haber medido a los tres grupos y comparado.

    Sobre el grupo secundario: la funcionalidad 4 del brief depende de que los docentes quieran difundir eventos a sus cátedras, y eso está **sin evidencia**. Antes de diseñar esa parte del producto lo mejor sería entrevistarlos. Lo mismo vale para los administrativos y la funcionalidad 1.

5. Hipótesis de valor

    > **Creemos que** el alumno de Ingeniería en Informática del DIIT que cursa entre 3.º y 5.º año, se informa por el celular y no busca información de eventos por su cuenta,
    >
    > **tiene el problema de** perderse eventos **de su propio departamento** que sí le interesan, porque el aviso no le llega o le llega demasiado cerca de la fecha,
    >
    > **Nuestra solución es** una plataforma que centraliza los eventos y **se los empuja al celular** filtrados por su carrera y año, con antelación suficiente y con la información completa para decidir, dejando la inscripción a un toque desde esa misma alerta.
    >
    > **Sabremos que estamos en lo correcto cuando**, tras un cuatrimestre de uso, los alumnos que reportan *"no vi la publicación"* bajen del **75 % actual a menos del 30 %**, el **80 % de las alertas** se entregue con **7 días o más** de anticipación, y aparezcan las primeras respuestas de asistencia en **4 y 5** de la escala, hoy inexistentes.

    ---

    **Trazabilidad.** Cada parte de la hipótesis con el dato del relevamiento que la sostiene:

    | Parte | Qué afirma | Dato que lo sostiene |
    |---|---|---|
    | **Usuario** | Alumno de Ing. en Informática del DIIT, 3.º a 5.º año | Las 20 respuestas del grupo primario son de esa carrera y ese departamento; 17 de 20 cursan entre 3.º y 5.º (punto 3.1). |
    | **Usuario** | Se informa por celular | 19 de 20 se enteran de eventos por celular; **8 no usan ningún otro dispositivo** (punto 3.4). |
    | **Usuario** | No busca por su cuenta | 12 de 20 buscan información sobre eventos "Nunca" o solo "Esporádicamente". **U6**: *"no voy a estar revisando múltiples medios en busca de que aparezca un evento"* (punto 3.1). |
    | **Problema** | Le interesan y no va | Interés en eventos del propio departamento **3,60 / 5**, asistencia **1,95 / 5**, con **ningún alumno respondiendo 4 ni 5** en asistencia. 8 de 20 combinan interés alto con asistencia baja (punto 3.1). |
    | **Problema** | Se los pierde de hecho | **13 de 20** quisieron ir a un evento y no pudieron por no enterarse a tiempo o no encontrar la información (punto 3.3). |
    | **Problema** | El aviso no llega | *"No vi la publicación"* es el motivo más marcado: **15 de 20** (punto 3.3). |
    | **Problema** | O llega tarde | *"La publicación apareció demasiado cerca de la fecha"*: **11 de 20**. Antelación percibida **2,05 / 5** (punto 3.3). |
    | **Problema** | Del propio departamento, no de otros | Interés en otros departamentos **2,20 / 5**, ninguna respuesta en 5, y **cero alumnos que los prioricen por encima de los propios** (punto 4, supuesto 1). |
    | **Solución** | Centralizar | **20 de 20** querrían tener todo en un solo lugar; hoy la información está repartida en 10 canales, 3,7 por alumno (punto 3.2). |
    | **Solución** | Empujar al celular, no esperar la consulta | Se deriva de que 12 de 20 no buscan y de que el motivo principal sea no haber visto la publicación: un lugar donde consultar no alcanza (punto 4.2). |
    | **Solución** | Filtrar por carrera y año | El interés está concentrado en el propio departamento (3,60 contra 2,20); y 4 de 20 ya rechazan ser notificados, así que el volumen importa (puntos 3.2 y 4.1). |
    | **Solución** | Con información completa | **U22**: *"la información provista en las publicaciones suelen ser escazas o poco claras"*. **U13**: *"no profundizan tanto como para generar un interés"* (punto 3.2). |

    ---

    **Cómo se mide.** Los umbrales se fijan contra la línea de base que dejó esta misma encuesta, de modo que la remedición sea una comparación real y no una impresión:

    | Indicador | Cómo se mide | Línea de base (agosto 2026) | Umbral para considerarla confirmada |
    |---|---|---|---|
    | **Alcance del aviso** | Se repregunta el motivo de perderse un evento a los mismos alumnos, tras un cuatrimestre de uso | *"No vi la publicación"*: **15 de 20 (75 %)** | Por debajo del **30 %** |
    | **Eventos perdidos** | Se repregunta si quiso ir a un evento y no pudo por no enterarse | **13 de 20 (65 %)** | Por debajo del **30 %** |
    | **Antelación** | Porcentaje de alertas entregadas con 7 días o más de anticipación, medido en el propio producto | Antelación percibida **2,05 / 5**; *"demasiado cerca de la fecha"* **11 de 20** | **80 %** de las alertas con 7 días o más, y percepción por encima de **3,5 / 5** |
    | **Participación declarada** | Se repregunta la frecuencia de asistencia | **1,95 / 5**, con techo en 3: **nadie respondió 4 ni 5** | Que **aparezcan respuestas en 4 y 5**, hoy inexistentes |
    | **Conducta real** | Inscripciones efectivas por alumno y por cuatrimestre, medidas en el producto | No existe: hoy no hay mecanismo de inscripción | Que crezca entre cuatrimestres, no un valor absoluto en la primera medición |
    | **Rechazo** | Porcentaje de usuarios que silencia o da de baja las notificaciones | 4 de 20 (**20 %**) declaran de entrada que no quieren ser notificados | Que la baja efectiva **no supere ese 20 %** |


