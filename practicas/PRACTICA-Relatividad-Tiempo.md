# Practica: Relatividad del Tiempo

- [Practica: Relatividad del Tiempo](#practica-relatividad-del-tiempo)
  - [Caso de uso para aprendizaje](#caso-de-uso-para-aprendizaje)
  - [Extraer información de libros y textos](#extraer-información-de-libros-y-textos)
  - [Caso de uso para labores Administrativas](#caso-de-uso-para-labores-administrativas)
  - [Caso de uso para labores creativas](#caso-de-uso-para-labores-creativas)




## Caso de uso para aprendizaje

>Aprendizaje
>
>Usar para aprender sobre alguna temática conocida o desconocida
>
>* Buen punto de partida porque cubre hasta un 80% del conocimiento -> hasta nivel medio
>* Falta fiabilidad de la respuesta
>* Se puede dirigir como una conversación
>* Ayudar a los estudiantes -> preparar exámenes
>* Proporcionar curiosidades o cosas poco conocidas


**Paso 1:** Setearemos la IA para que sea un físico teórico -> Role Prompting

```bash
Actúa como un {rol} {experiencia_rol}. Explícame el estado actual de la física con palabras sencillas.
Parafrasea cuál es tu {rol} para confirmar que lo has entendido

{rol}=físico teórico
{experiencia_rol}=con 20 años de experiencia
```

**Paso 2:** Solicitaremos información general con un poco de contexto

```bash
Dame las 10 áreas más importantes actualmente sobre la física
```

**Paso 3:** Solicitaremos información en detalle sobre algun aspecto mostrado anteriormente

```bash
Me puedes dar más información sobre el punto: {tematica}

{tematica}=Relatividad General
```

**Paso 4:** Extraeremos cierta información del texto anterior

```bash
Considera el texto de la respuesta anterior. Extrae los puntos más relevantes en una lista numerada
```

**Paso 5:** Reformatear la información

```bash
Genera una tabla con los puntos 1 y 2 con dos columnas. Una columna con el texto del punto y la otra con las palabras clave más destacables
```

**Paso 6:** Solicitaremos un ejemplo fácil

```bash
Ponme un ejemplo sencillo sobre: {tematica_con_dudas}

{tematica_con_dudas}=Curvatura del espacio-tiempo
```

**Paso 7:** Solicitaremos una curiosidad

```bash
Explícame una curiosidad poco conocida de {tematica_con_dudas}
```

**Paso 8:** Solicitaremos otro recurso asociado: exámen

```bash
Podrías generar un exámen de 5 preguntas sobre {tematica_con_dudas}
```

**Paso 9:** Solicitaremos otros recursos asociados: listado libros

```bash
Propón 5 libros para empezar a aprender sobre {tematica_con_dudas}
```

**Paso 10:** Solicitaremos otros recursos asociados "listado películas"

```bash
Propón 5 películas actuales (últimos 6 años) sobre {tematica_con_dudas}
```

**Paso 11:** Solicitaremos un recordatorio de las entidades

```bash
Recuerdame que valor contienen las siguientes etiquetas (mantén el formato de llaves e igualdades para responder)

{rol}=
{experiencia_rol}=
{tematica}=
{tematica_con_dudas}=
```





## Extraer información de libros y textos

>Se puede generar un resumen de un libro y/o texto
>
>* Iterar para resolver el problema del contexto
>* Solicitar mejores explicaciones
>* Obtener texto entendible para los mortales


**Paso 1:** Solicitar un resumen de un libro

```bash
Puedes realizar un breve resumen del libro {libro_seleccionado}

{libro_seleccionado}="El Universo en una cáscara de nuez" de Stephen Hawking
```

**Paso 2:** Extraer informacion

```bash
Puedes proporcionar el listado de capítulos del libro {libro_seleccionado}

{libro_seleccionado}="El Universo en una cáscara de nuez" de Stephen Hawking
```

**Paso 2:** Extraer informacion

```bash
Puedes proporcionar el listado de capítulos del libro {libro_seleccionado}
```
pero me ibas a ayudar, me gustaría que me dijeras los titulos

**Paso 3:** Solicitar un resumen especifico

```bash
Puedes generar un resumen de 4 líneas para cada uno de los capítulos del libro {libro_seleccionado}
```

**Paso 3:** Solicitar un resumen general

```bash
Puedes generar un resumen de lo anterior
```

**Paso 4:** Solicitar un resumen general con un reformateo para mejorar la explicación

```bash
Explicame el resumen como si tuviera 10 años y usa analogías
```





## Caso de uso para labores Administrativas

**Paso 1:** Solicitar un resumen general

```bash
Explicame la curvatura espacio temporal con mi edad y con algun ejemplo sencillo
```

```bash
puedes hacer una formula de excel de lo anterior
```





## Caso de uso para labores creativas

>Usar para generar ideas que aplican sobre áreas concretas
>
>* Brainstorming
>* Generación de contenido
>* Copywriting


**Paso 1:** Brainstorming de ideas de empresa

```bash
Genera 10 nombres buenos para una posible nueva empresa que trabaje con la relatividad temporal. Este nombre tiene que estar relacionado de alguna manera con agujeros de gusano
```

```bash
Simplica la lista en los que consideres mejores
```

```bash
Elimina el primero
```

```bash
Puedes internacionalizar los nombres
```

```bash
Me gustan el 1 y el 3 ¿Explicame que pros y contras tiene cada uno?
```






## Caso de la pelicula "Interestellar"

**Paso 1:** Probaremos sobre el conocimiento existente sobre una pelicula que debería haber sido cargada en el dataset de entrenamiento

```bash
Explica sobre la película Interestellar
```

**Paso 2:** Parametrizaremos mediante etiquetas la petición anterior

```bash
Explica sobre la película {pelicula}

{pelicula}=Interestellar
```

**Paso 3:** Solicitaremos un resumen de la pelicula

```bash
Escribe un resumen sobre la película {pelicula}
```

**Paso 4:** Solicitaremos un resumen de la pelicula con un modificador

```bash
Escribe un resumen de 5 lineas sobre la película {pelicula}
```

```bash
Escribe un resumen sobre la película {pelicula} en verso
```

**Paso 5:** Solicitaremos un resumen de la pelicula con un estilo definido

```bash
Escribe un resumen con un estilo de {estilo_escritura} sobre la película {pelicula}

{estilo_escritura}= un mínimo de 5 y máximo de de 8 líneas, escrito por un niño de 9 años con un tono de humor
```

**Paso 6:** Solicitaremos que nos diga la opinión de la pelicula como si fuera alguien

```bash
Escribe la opinión de la pelicula {pelicula} como si fueras Steve Jobs
```

**Paso 7:** Solicitaremos que nos diga la temática de la pelicula en un formato de lista

```bash
Extrae las temáticas principales de la {pelicula} como una lista
```

```bash
Muestra detalles en un parrafo para cada uno elementos de la lista anterior
```

**Paso 8:** Generar un índice para abordar un tema

```bash
Vas a asistir a un debate a nivel mundial,

El asunto del debate es: "La relatividad del tiempo y sus efectos en la experiencia humana"

Tendrás la postura A, que esta en contra de que exista la relatividad del tiempo.

Utiliza un índice jerárquico para mostrar argumentos en contra de que exista y categorizalos en, como mínimo, 5 categorías diferentes con  al menos 3 argumentos por cada categoría
```