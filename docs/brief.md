# Brief de Producto — Nodo UNLaM

## Versión 2 — Agosto 2026

> **Registro de cambios.** Esta versión se reescribe con la evidencia del relevamiento del TP2: una encuesta de 22 respuestas —20 de alumnos, el grupo primario— realizada el 30 y 31 de agosto de 2026, documentada en [TP2.md](TP2.md) y versionada en [`docs/evidencia/tp2/`](evidencia/tp2/).
>
> **Qué cambió y por qué.** Cayó el recorte del supuesto crítico: la versión 1 sostenía que el problema era enterarse de los eventos **de otros departamentos**, y el relevamiento mostró que esos eventos casi no le interesan a nadie —2,20 sobre 5, y **ningún alumno los prioriza por encima de los de su propio departamento**—. El problema es intradepartamental. En consecuencia: el **perfil hipotético de alumno fue reemplazado por el perfil real** relevado, la **alerta pasó de ser la funcionalidad 3 a ser el eje del producto** —el motivo más marcado para perderse un evento es "no vi la publicación", 15 de 20, y 12 de 20 no buscan información nunca o casi nunca—, la **segmentación dejó de ser un antisaturación para volverse el núcleo**, y **compartir eventos a cátedras de otros departamentos salió del alcance inicial** por quedarse sin sustento. Se agregaron necesidades, problemas y contexto de uso que antes no existían en el brief, y la hipótesis de valor.
>
> **Qué no cambió y por qué.** El producto, el segmento y la mayoría de las funcionalidades siguen en pie: el problema existe y está documentado —13 de 20 quisieron ir a un evento y no pudieron—, y la dispersión de canales quedó confirmada. Lo que se corrigió es dónde está el problema, no si lo hay.


---

## 1. Segmento elegido

**Segmento:** Personal docente y estudiantil de la UNLaM, pertenecientes únicamente a las carreras de grado.

**Por qué ese segmento:** Porque estudiantes y docentes tienen una participación directa en las actividades académicas de la UNLaM. Los estudiantes son los principales destinatarios de estos eventos y necesitan acceder a información relevante sobre ellos, mientras que los docentes cumplen un rol importante en su difusión dentro de las comisiones.

**Tamaño aproximado:** Entre 78.000 y 79.000 estudiantes y aproximadamente 3.400 docentes.

**Qué los distingue del resto de la comunidad:** Son personas directamente vinculadas con la actividad académica de la universidad, principales participantes e interesados de la comunicación y participación de actividades complementarias a la cursada.

> **Alcance validado (nuevo en v2).** El segmento sigue siendo la aspiración del producto, pero lo único que hoy tiene respaldo empírico es el **DIIT, carrera de Ingeniería en Informática**. Ampliar el segmento con evidencia requiere relevar otras carreras.

---

## 2. Producto

**Nombre:** Nodo UNLaM

**Problema que resuelve (revisado en v2).** Los alumnos se pierden eventos **de su propio departamento** que sí les interesan. El problema tiene tres causas distintas, que el relevamiento permitió separar:

1. **De alcance** — la publicación existe y no llega: *"no vi la publicación"*, **15 de 20**. Es el motivo más frecuente.
2. **De oportunidad** — llega, pero tarde para organizarse: *"apareció demasiado cerca de la fecha"*, **11 de 20**.
3. **De dispersión** — la información está repartida en 10 canales distintos, 3,7 por alumno: **8 de 20** marcan que estaba distribuida y otros **8** que no sabían dónde buscarla.

La versión 1 nombraba solo la tercera. Las dos primeras son más frecuentes y **no se resuelven centralizando**: centralizar no sirve si el usuario nunca entra al lugar donde se centralizó.

**A quién se lo resuelve.** A los alumnos, en primer lugar. Con el agregado —confirmado por el relevamiento— de que la solución tiene que ir a buscarlos a ellos y no al revés: **12 de 20 no buscan información sobre eventos nunca o solo esporádicamente**.

---

## 3. Funcionalidades core

Reordenadas por prioridad según la evidencia. El cambio principal respecto de v1 es que la notificación deja de ser la tercera funcionalidad y pasa a ser el eje.

1. **Alerta segmentada al celular** *(era la funcionalidad 3; ahora es el núcleo)*. Envío activo de los eventos que corresponden a la carrera y el año del alumno, con antelación suficiente. Sostiene el problema de alcance (15 de 20) y el de oportunidad (11 de 20), y responde a que 19 de 20 se enteran por celular y 8 no usan ningún otro dispositivo. Requiere **frecuencia configurable y baja**: 4 de 20 declaran que no quieren ser notificados.
2. **Ficha de evento completa** *(nueva en v2)*. Fecha, hora, lugar, de qué se trata y qué se necesita para participar. Surge de que la publicación actual no alcanza para decidir: **U22** — *"la información provista en las publicaciones suelen ser escazas o poco claras, y es dificil encontrar detalles adicionales"*; **U13** — *"no profundizan tanto como para generar un interés"*.
3. **Consulta centralizada de eventos**. El único punto donde está todo: **20 de 20** lo querrían. Sigue siendo necesario, pero es el destino de la alerta, no la puerta de entrada.
4. **Inscripción a un evento**, con confirmación y control de cupo. Sin cambios respecto de v1.
5. **Carga y publicación de eventos por departamento** (rol administrativo): título, descripción, fecha/hora, lugar, cupo y departamento/carrera al que se dirige. Sin cambios respecto de v1, pero **sin evidencia**: ningún administrativo fue relevado.

**Fuera del alcance inicial:** *compartir o recomendar un evento a una cátedra de otro departamento* (era la funcionalidad 4 de v1). Se apoyaba en dos cosas que no se sostienen: que los eventos de otros departamentos interesaran —refutado— y que los docentes quisieran difundirlos —sin evidencia—. No debería construirse antes de entrevistar docentes.

---

## 4. Integraciones previstas

- **Intraconsulta UNLaM:** para obtener materias, comisiones y alumnos inscriptos, y así habilitar la segmentación por carrera y año. **Sube de prioridad en v2**: si la segmentación es el núcleo, esta integración es la que la hace posible.
- **Calendario académico institucional:** para contextualizar los eventos con fechas generales del cuatrimestre, como las mesas de examen y verificación de materias.
- **Canal de la alerta — decisión abierta.** La v1 daba por sentado Teams. El relevamiento no lo confirma ni lo descarta, pero lo acota:
  - **16 de 20 aceptarían** ser notificados por Teams, pero solo **3 de 20** lo mencionan como canal actual: hay aceptación declarada, no hábito.
  - **WhatsApp es el canal no institucional más instalado** (13 de 20) y el de menor fricción de adopción.
  - **El correo es la opción más débil: ningún alumno lo menciona** entre los canales por los que hoy se entera de eventos.
  - La decisión entre aplicación móvil con push y aplicación web con WhatsApp o mail **requiere una pregunta comparativa que esta encuesta no hizo**.

---

## 5. Grupos de usuarios

### Grupo primario: Alumnos — perfil real (reemplaza al perfil hipotético de v1)

**Quién es.** Estudiante de **Ingeniería en Informática del DIIT**, de **21 a 27 años** (18 de los 20 relevados; los extremos son 17 y 39), **cursando entre 3.º y 5.º año** (17 de 20).

**Cómo se comporta.** Lo que lo define no es el desinterés sino la brecha entre lo que le interesa y lo que hace: el interés en los eventos de su propio departamento promedia **3,60 sobre 5**, la asistencia **1,95**, y **ningún alumno respondió 4 ni 5 en asistencia**. Ocho de veinte combinan interés alto con asistencia baja.

**Es pasivo en la búsqueda.** 12 de 20 buscan información sobre eventos "Nunca" o solo "Esporádicamente". **U6**: *"los medios de comunicación oficial suelen tener la información, pero es raro que los revise, más que nada porque no voy a estar revisando múltiples medios en busca de que aparezca un evento"*.

**Se informa por canales mayormente informales.** 16 de 20 por Instagram, 16 por algún canal informal —WhatsApp (13), Discord (5) o un compañero (9)—. Tres alumnos no usan **ningún** canal institucional. **U10**: *"si no fuese porque los tengo en instagram, no me enteraría de casi nada"*.

> *Qué decía la v1:* "alumnos activos de cualquier carrera de grado que hoy se enteran de eventos solo si siguen la cuenta de su propio departamento… se pierden sistemáticamente los eventos". La intuición sobre la dependencia de redes sociales resultó correcta; el alcance ("cualquier carrera") y la parte sobre eventos de otros departamentos, no.

### Grupo secundario: Docentes — sin evidencia

Los docentes no fueron objeto del relevamiento. Dos respondieron de manera espontánea, lo que no constituye evidencia sobre el grupo, y el cuestionario **no incluyó ninguna pregunta sobre difundir o compartir eventos**. Todo lo que la v1 afirmaba sobre su rol de difusores sigue siendo una hipótesis sin verificar. Requiere entrevista.

### Grupo secundario: Administrador de eventos por departamento — sin evidencia

**Ningún administrativo respondió.** El instrumento tampoco estaba diseñado para ellos. La descripción de v1 —que hoy cargan el mismo evento en Instagram y por mail, sin sistema único ni visibilidad de inscriptos— se mantiene como supuesto, no como hallazgo. Requiere entrevista y observación del proceso actual.

**Por qué los alumnos siguen siendo el grupo primario.** Son quienes muestran la brecha entre interés y asistencia y quienes reportan haberse perdido eventos (13 de 20). **Con una advertencia honesta:** el relevamiento no puede decir si otro grupo tiene el problema más fuerte, porque solo relevó al grupo primario. Mantenerlos es consistente con lo encontrado, no el resultado de haber comparado los tres grupos.

---

## 6. Necesidades, problemas y contexto de uso (nuevo en v2)

### Necesidades relevadas

1. **Un único lugar donde esté todo** — 20 de 20, la única respuesta unánime.
2. **Que la información los alcance en vez de tener que buscarla** — 12 de 20 casi nunca buscan.
3. **Enterarse con tiempo para poder ir** — antelación percibida 2,05 sobre 5.
4. **Información completa, no solo el aviso** — U13 y U22.
5. **Relevancia filtrada** — interés 3,60 en el propio departamento contra 2,20 en los demás.

### Problemas y frustraciones

**13 de 20 quisieron ir a un evento y no pudieron** porque no se enteraron a tiempo o no encontraron la información. Los motivos: *"no vi la publicación"* (15 de 20), *"apareció demasiado cerca de la fecha"* (11), *"no sabía dónde buscar"* (8) y *"la información estaba distribuida en distintos canales"* (8). La eficiencia percibida de la comunicación de la UNLaM promedia **2,50 sobre 5**, con 10 de 20 puntuándola en 1 o 2.

### Contexto de uso

- **Dispositivo:** celular, 19 de 20; **8 no usan ningún otro**. Computadora 12, tablet 1.
- **Momento:** no hay un momento dedicado. El consumo es incidental, mientras usan el teléfono para otra cosa, entre clases o fuera de la facultad.
- **Condición:** apurados y en modo pasivo. El primer impacto es decisivo: el motivo más marcado es no haber visto la publicación, no que no interesara.
- **Compañía:** la información circula por rebote social — 9 se enteran por un compañero, 8 por un docente, 13 participan de grupos de WhatsApp.
- **Conectividad:** **no relevada.** No se afirma nada sobre uso sin conexión.
- **Barrera no informativa:** dos alumnos señalaron espontáneamente que los eventos **se superponen con su horario de cursada** (U12, U19). Ninguna funcionalidad de este brief la resuelve.

---

## 7. Hipótesis de valor

> **Creemos que** el alumno de Ingeniería en Informática del DIIT que cursa entre 3.º y 5.º año, se informa por el celular y no busca información de eventos por su cuenta,
>
> **tiene el problema de** perderse eventos **de su propio departamento** que sí le interesan, porque el aviso no le llega o le llega demasiado cerca de la fecha,
>
> **Nuestra solución es** una plataforma que centraliza los eventos y **se los empuja al celular** filtrados por su carrera y año, con antelación suficiente y con la información completa para decidir, dejando la inscripción a un toque desde esa misma alerta.
>
> **Sabremos que estamos en lo correcto cuando**, tras un cuatrimestre de uso, los alumnos que reportan *"no vi la publicación"* bajen del **75 % actual a menos del 30 %**, el **80 % de las alertas** se entregue con **7 días o más** de anticipación, y aparezcan las primeras respuestas de asistencia en **4 y 5** de la escala, hoy inexistentes.

La trazabilidad de cada parte a los datos del relevamiento está en el [punto 5 del TP2](TP2.md).

---

## 8. Estado de los supuestos

### Supuestos de la versión 1

| # | Supuesto | Estado | Evidencia |
|---|---|---|---|
| **1** *(crítico)* | Estudiantes y docentes tienen dificultades para enterarse de los eventos **de otros departamentos**. | **Refutado** en su recorte (alumnos) · **Sin evidencia** (docentes) | La dificultad existe, pero no ahí. Interés en otros departamentos **2,20 / 5**, 13 de 20 responden 2 o menos, ninguno responde 5, y **cero alumnos los priorizan por encima de los propios**. El problema está en los eventos propios: interés 3,60, asistencia 1,95, 13 de 20 se perdieron un evento. |
| **2** | La información está dispersa entre distintos canales. | **Confirmado** | 10 canales en uso, 3,7 por alumno, 14 de 20 usan 3 o más. 8 de 20 marcan que estaba distribuida. **U5**: *"Hay información esparcida por muchos canales diferentes"*. |
| **3** | Los docentes consideran útil compartir eventos con sus cátedras. | **Sin evidencia** | Grupo secundario, no relevado. Además el cuestionario no preguntó sobre difundir ni compartir. |
| **4** | El personal administrativo necesita una herramienta centralizada de carga y gestión. | **Sin evidencia** | Ningún administrativo respondió. |
| **5** | La información centralizada aumentaría la participación. | **Sin evidencia** | La participación no se midió antes y después. El único dato cercano —20 de 20 querrían un solo lugar— mide deseo, no conducta, y es una pregunta sin poder discriminante. |
| **6** | Los alumnos prefieren notificarse por herramientas de uso cotidiano de la cursada antes que por externas. | **Parcialmente confirmado** | 16 de 20 aceptarían Teams. Pero la **preferencia comparada nunca se preguntó**, y la premisa se cae: Teams es canal actual de 3 de 20 y MIeL de 6, frente a Instagram 16 y WhatsApp 13. |

### Supuestos nuevos, surgidos del relevamiento

Todos **sin evidencia**: aparecieron en los datos pero el instrumento no estaba diseñado para medirlos. Son los candidatos a verificar en la próxima ronda.

| # | Supuesto nuevo | De dónde sale | Cómo verificarlo |
|---|---|---|---|
| **7** | Existe una barrera de **agenda**, no de información: los eventos se superponen con el horario de cursada. | U12 y U19 lo mencionaron espontáneamente, sin que se preguntara — 2 de las 9 respuestas abiertas. Además la asistencia tiene techo 3 incluso entre quienes declaran interés máximo. | Preguntar directamente por motivos de no asistencia distintos de la información. Cruzar horarios de eventos con horarios de cursada. |
| **8** | La **calidad de la publicación** es una barrera de decisión, no solo su llegada. | U13 y U22: la información es *"vaga"*, *"escaza o poco clara"* y faltan detalles. | Testear dos formatos de ficha de evento y medir cuál genera más inscripciones. |
| **9** | El **canal más efectivo para la alerta** es el celular por una vía que el alumno ya usa, no una plataforma académica. | Teams: 16 de 20 lo aceptan pero solo 3 lo usan. WhatsApp: 13 de 20 ya lo usan. Correo: 0 alumnos. | Pregunta comparativa entre push, WhatsApp, Teams y mail. |
| **10** | Una parte del público **rechaza ser notificado**, y la notificación mal calibrada expulsa usuarios. | 4 de 20 responden que no quieren notificaciones por plataforma académica. | Medir la tasa de baja y silenciamiento una vez en funcionamiento. |
