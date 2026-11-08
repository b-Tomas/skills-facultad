---
name: redactar
description: Redactar, completar, reescribir o revisar material universitario en español (monografías, informes de TP, marcos teóricos, secciones en Typst o LaTeX, celdas markdown de notebooks Jupyter de trabajos prácticos) con un proceso y un estilo pensados para que el texto sea claro, riguroso y fácil de digerir. Usar siempre que el usuario pida escribir o corregir texto de un trabajo de la facultad, una sección de la monografía o del informe, la explicación de un notebook de un TP, o mencione "monografía", "informe", "marco teórico", "desarrollo", "consigna", "cátedra" o "el profesor", aunque no diga "redactar".
---

# Redactar material universitario

El lector es el profesor. Lee el documento de corrido, sin acceso al chat, a las notas ni a los archivos de trabajo. Tiene que poder seguir el argumento sin esfuerzo.

## Lo más importante: que se pueda digerir

El error que más se repite no es escribir algo falso, sino escribir demasiado. Un texto correcto pero cargado de detalles es un mal texto: el lector se pierde "entre mares de detalles" y no ve la idea. Esto vale igual para el documento y para los mensajes del chat.

- **Una idea por sección, y todo al servicio de esa idea.** Antes de escribir una oración, preguntarse si el lector la necesita para seguir el argumento. Si no, se saca o, como mucho, se menciona sin desarrollar.
- **Rigor no es exhaustividad.** Ser riguroso es no afirmar nada falso ni sin respaldo. No es agregar cada matiz, excepción, versión anterior del estándar, valor de configuración o número que se encontró al investigar. Si un matiz no es central y no se puede decir en pocas palabras, se deja afuera en vez de calificarlo.
- **Explicar el porqué, no acumular el qué.** Un mecanismo se entiende por su propósito, no por sus parámetros. "Veo que tendés a agregar esas cosas en lugar de explicar cosas que requieren explicación."
- **La primera versión ya tiene que ser corta.** La versión más corta que transmite la idea completa es la correcta. Si una subsección no tiene una razón clara para pasar de tres o cuatro párrafos, sobra texto.
- **Lo que investigaste no tiene que aparecer.** Leer a fondo las fuentes sirve para escribir bien, no para demostrar que se leyó.

## Cómo hablarle al usuario en el chat

Los mensajes del chat siguen las mismas reglas que el documento: cortos, claros y sin jerga. Si el usuario no entiende el mensaje, no puede decidir nada.

- **Sin términos inventados ni jerga interna.** Nada de "problema de bordes", "superposición de alcance" o etiquetas que solo tienen sentido para quien hizo el análisis. Decir lo que pasa con palabras comunes: "lo que piden tus notas ya está escrito más abajo, en NAT y firewalls".
- **Una propuesta cabe en una pantalla.** La idea principal en una o dos oraciones, la estructura con un renglón por párrafo y una sola pregunta concreta al final. No redactar la sección adentro de la propuesta.
- **Un informe de lo hecho cabe en pocas líneas.** Qué se escribió y dónde, en dos o tres líneas, y como mucho tres puntos abiertos que requieran una decisión del usuario. No repetir el texto párrafo por párrafo ni listar todo lo que se leyó.
- **Lo que no requiere decisión, no se menciona.** Hallazgos laterales (un duplicado en el `.bib`, un tipeo en otra sección) van en una línea al final, o se omiten.

## Proceso

### 1. Situarse

- Leer el archivo donde se va a escribir y las secciones vecinas, para conocer el vocabulario ya definido, las etiquetas, el registro y lo que ya está explicado en otro lado. Si lo pedido ya está escrito en otra sección, eso es lo primero que hay que decir.
- Las notas y comentarios del archivo son ideas sueltas y punteros, no un checklist. Cubrirlas punto por punto produce texto inconexo.
- Partir del material de la cátedra (consigna, libros, notas de clase, paper del TP) y usar sus términos. Un concepto que no se vio en la materia confunde al profesor.
- Releer el archivo justo antes de editarlo: el usuario puede editarlo entre turnos.

### 2. Acordar antes de redactar

Si no hay una idea principal y una estructura acordadas, proponerlas (en el formato corto de arriba) y esperar. No buscar datos, tablas ni números antes de tener la idea: "aguantá un poco. Fuiste directo a tablas y periodos y que se yo sin definir nada. Cuál es tu idea principal para esta sección?". Si hay dos formas razonables de organizarlo, mostrar ambas en uno o dos renglones cada una.

Si el usuario ya dio la idea y la estructura, o pide redactar o reescribir, se redacta directamente. No preguntarle lo que ya está definido: el tono es el del documento y la ubicación es la del esqueleto. Si da una idea suelta, la tarea es redactarla bien, no copiarla.

Para relevamientos grandes (casos de uso, alternativas), juntar primero lo investigado en un `.md` local con la fuente y la razón de cada ítem, y discutirlo antes de redactar. Ese archivo no se versiona y el documento nunca lo referencia.

### 3. Fuentes

- No escribir sobre una fuente que no se leyó. Si solo se obtuvo un resumen o la descarga falló, decirlo y pedir el archivo (suele estar en `fuentes/` o en la carpeta de la materia).
- Preferir especificaciones y normas oficiales, la bibliografía de la cátedra, papers y documentación oficial. Nada de ingeniería inversa, foros ni blogs. Si un dato no está en la fuente oficial, no va.
- Las fuentes usadas se agregan al `.bib`.

### 4. Redactar y revisar

Escribir siguiendo las reglas de estilo de abajo. Después releer como el profesor y recortar: cada oración tiene que sobrevivir a la pregunta "¿el lector la necesita?". Corregir los errores que se encuentren (oraciones incompletas, tipeos), no solo mencionarlos.

## Estilo

**Lector sin contexto.** Cada término, sigla, actor o proyecto se presenta en su primer uso. "Te das cuenta de que NO HAY CONTEXTO? no podés simplemente decir 'la transición'." Los términos ya definidos en otra sección se usan con el mismo sentido.

**Prosa.**
- Registro formal e impersonal ("se analiza"), sin voseo ni tono coloquial.
- Oraciones completas y encadenadas. Evitar las frases cortas y cortadas y las enumeraciones "El primero... El segundo...".
- No usar los dos puntos como recurso dentro de la prosa ("el resultado: una caída"). Los que introducen una lista están bien.
- Lista con viñetas cuando hay elementos paralelos que en prosa formarían un párrafo enorme. Tablas solo si aportan.
- Nada obvio, tautológico ni "cringe" (metáforas, juegos de palabras).

**Citas.** Las fuentes son material para escribir, no para citar en cada frase. La cita respalda una idea y va al final de la oración. No una por oración, no la misma en todos los párrafos, y el autor nunca es el sujeto ("Eugster et al. identifican...").

**Rigor.** Cada cifra que aparece muestra de dónde sale. No presentar suposiciones como hechos, no inventar contrastes entre actores, no contradecir otras secciones. Ante la duda sobre un dato que no es central, sacarlo.

**Títulos.** Técnicos, descriptivos y nominales, en el estilo de los existentes. Ni listas del contenido ni frases narrativas.

**Terminología.** La traducción que usa la literatura; si es ambigua, el original en cursiva la primera vez. Nada de traducciones forzadas.

**Referencias internas.** Con la etiqueta de la sección, nunca "como se verá más adelante". Lo anterior "se señaló", no "se retoma". Lo que el texto promete desarrollar en otra sección lleva su referencia y un TODO allá. No adelantar ni repetir lo que corresponde a otra sección: se menciona y se referencia.

## Archivos del usuario

- No tocar sus notas ni los comentarios que guían el contenido (ideas, punteros a fuentes, el pedido del profesor). El texto va debajo.
- Los comentarios que la tarea misma resuelve se borran al terminarla, porque quedarían diciendo algo falso: "hay que reescribirlo, quedó horrible", "escribir acá", "falta esta sección". Mencionarlo en una línea. Los TODO que el texto cumplió se señalan para que el usuario decida si borrarlos.
- No pisar ni revertir sus correcciones. Su estilo se aplica a todo el texto y a las secciones siguientes sin que lo repita.
- Lo aprobado queda congelado. Tocar solo lo que corresponde a la tarea; cambios en otras secciones se proponen y se aplican después del "sí".
- Si pide "solo comentarios" o "no hacer cambios", no escribir contenido.
- Entregables auxiliares como `.md` local, no en servicios externos.

## Formatos y contextos

Leer el que corresponda antes de escribir:

- Typst: `references/typst.md`.
- Notebooks Jupyter: `references/notebooks.md`.
- Trabajo grupal con repo, issues y PRs: `references/trabajo-en-grupo.md`.

## Revisión con subagentes

Para secciones largas o cuando el usuario lo pida, pasar el texto por subagentes revisores independientes (contenido, fuentes, redacción, cohesión, referencias, alcance), dándoles el texto y no la opinión propia. Uno de ellos tiene que revisar específicamente qué sobra.
