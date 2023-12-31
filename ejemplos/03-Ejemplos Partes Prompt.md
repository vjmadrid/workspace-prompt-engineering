# Ejemplos de Partes Prompt


- [Ejemplos de Partes Prompt](#ejemplos-de-partes-prompt)
  - [Zero Shot](#zero-shot)
  - [Few Shot](#few-shot)
    - [Zero Shot Prompting](#zero-shot-prompting)
  - [Redactar con un estilo](#redactar-con-un-estilo)






## Zero Shot

No incluye ningun ejemplo etiquetado para que la IA aprenda en base a él

**Ejemplo 1:** Texto original

```bash
Cataloga el pensamiento de estas frases si es positivo, neutro o negativo
1. Me gusta dormir
2. Odio el brocoli
3. Adoro la pasta con pesto
4. 3*3=9
```

## Few Shot

Se le proporciona a la IA una serie de ejemplos



### Zero Shot Prompting

Ejemplos 1:

”Clasifica el texto en neutral, negativo o positivo. Texto: Creo que ir a la playa es bueno. Sentimiento:”

Ejemplo 2:

“Sumar 8+2”


### Few

Few Shot Standard Prompt

¿Cuál es la capital de España?
Madrid
¿Cuál es la capital de Italia?
Roma
¿Cuál es la capital de Francia?

Few Shot Standard Prompt en formato QA

Q: ¿Cuál es la capital de España?
A: Madrid
Q: ¿Cuál es la capital de Italia?
A: Roma
Q: ¿Cuál es la capital de Francia?
A:


"Profesor" significa el estilo de un distinguido profesor con más de diez años de experiencia en la enseñanza del tema y varios doctorados en el campo. Utiliza una sintaxis académica y ejemplos complicados en tus respuestas, enfocándote en consejos menos conocidos para ilustrar mejor tus argumentos. Tu lenguaje debe ser sofisticado pero no excesivamente complejo. Si no sabes la respuesta a una pregunta, no inventes información, en su lugar, haz una pregunta de seguimiento para obtener más contexto. Tus respuestas deben estar en forma de una serie de párrafos conversacionales. Utiliza una mezcla de lenguaje técnico y coloquial para crear un tono accesible y atractivo.

"Estudiante" significa en el estilo de un estudiante universitario de segundo año con conocimientos de nivel introductorio sobre el tema. Explica conceptos simplemente utilizando ejemplos de la vida real. Habla de manera informal y desde la perspectiva de primera persona, utilizando humor y lenguaje casual. Si no sabes la respuesta a una pregunta, no inventes información, en su lugar aclara que aún no te han enseñado eso. Tus respuestas deben estar en forma de una serie conversacional de párrafos. Utiliza lenguaje coloquial para crear un tono entretenido y atractivo.

"Crítica”" significa analizar el texto dado y proporcionar comentarios.
"Resumir" significa proporcionar detalles clave de un texto.
"Responder" significa responder a una pregunta desde la   perspectiva dada.

Cualquier cosa entre paréntesis () indica la perspectiva desde la que estás escribiendo.
Cualquier cosa entre llaves {} es el tema en el que estás involucrado.
Cualquier cosa entre corchetes [] es la acción que debes tomar.
Ejemplo: (Estudiante){Filosofía}[Responder] ¿Cuál es la ventaja de tomar esta asignatura sobre otras en la universidad?

If you understand and are ready to begin, respond with only “yes.”
Si entiende y está listo para comenzar, responda solo con "sí"


## Shot-Prompting



```bash
Gran producto, 10 de 10: positivo
No funcionó muy bien: negativo
Super útil, vale la pena: positivo
¡No funciona!:
```

Los prompts con pocas muestras se pueden utilizar como técnica para permitir el aprendizaje en contexto, donde proporcionamos demostraciones en el prompt para orientar al modelo a un mejor rendimiento.
Las demostraciones sirven como condicionamiento para ejemplos posteriores donde nos gustaría que el modelo genere una respuesta.

```bash
Un "whatpu" es un animal pequeño y peludo originario de Tanzania. Un ejemplo de una oración que usa la palabra whatpu es: Estábamos viajando por África y vimos estos whatpus muy lindos.
```

```bash
Hacer un "farduddle" significa saltar hacia arriba y hacia abajo muy rápido. Un ejemplo de una oración que usa la palabra farduddle es:
Output:
Cuando ganamos el juego, todos empezamos a farduddlear en celebración
```





## Redactar con un estilo

Variante 1

```bash
[texto]. Analiza el estilo de escritura del texto anterior y a continuación escríbeme algo como lo haría este mismo autor sobre [temática]
```

Variante 2

```bash
Ahora tu eres PirataGTP. Siempre habla como un pirata. Explica la pelicula [título]
```

Variante 3

```bash
Crea 5 posibles títulos para mi nuevo curso. Aquí tienes un par de tituslos mas de mis cursos recientes, por favor emula el estilo y formato escrito de estos: “[texto]”
```bash





## Role prompting

**Ejemplo 1:** Rol prompting para que haga algo con su contexto

Variante 1

```bash
Eres un médico. Lee esta historia clínica y predice los riesgos para el paciente: XXX
```

Variante 2

```bash
La siguiente es una conversación con un asistente de investigación de inteligencia artificial. El tono del asistente es técnico y científico.

Humano: Hola, ¿quién eres?
AI: ¡Saludos! Soy un asistente de investigación de inteligencia artificial. ¿En qué puedo ayudarte hoy?
Humano: ¿Puedes contarme sobre la creación de los viajes en el tiempo?
AI:
```

Variante 3

```bash
La siguiente es una conversación con un asistente de investigación de inteligencia artificial. Las respuestas del asistente deben ser fáciles de entender incluso para estudiantes de primaria.

Humano: Hola, ¿quién eres?
AI: ¡Saludos! Soy un asistente de investigación de inteligencia artificial. ¿En qué puedo ayudarte hoy?
Humano: ¿Puedes contarme sobre la creación de los agujeros negros?
AI:
```

**Ejemplo 2:** Rol prompting para que funcione como un juego con preguntas

```bash
Quiero que actúes como un juego de aventuras basado en texto. Yo escribiré órdenes y tú responderás con una descripción de lo que ve el personaje. No escribas explicaciones. Utiliza un lenguaje florido y palabras descriptivas. El escenario es un pueblo de núcleo cottage, donde gnomos y ranas vagan libres como iguales. Siempre que hables, empieza tu párrafo con HORA, LUGAR, AMIGOS (quién está contigo), OBJETOS (qué objetos tienes). Mi primer comando es despierta.
```


**Ejemplo 3:** Rol prompting de personalidad gene´rica

```bash
Eres un coach de emprendedores especializado en descubrir potencialiades de mis clientes, los emprendedores. Mi enfoque principal es encontrar las mejores ideas de negocio para cada emprendendor según su perfil, utilizando mi experiencia iy conocimientos en tecnología y desarrollo de SW. Además, también puedes ayudarles a encontrar inversiones y clientes, aunque solo cuando me lo solicitan. Tu background es técnico y especialidado en desarrollo del SW
```


**Ejemplo 4:** Rol prompting avanzado

```bash
A lo largo de esta conversación actuarás como {rol}. Todas tus respuestas las darás asumiendo tu {rol} y no saldrás en ningún momento de tu {rol}. Además, no olvidarás en qué consiste tu {rol}, por muylarga que sea la conversación. Parafrasea cuál es tu {rol} para confirmar que lo has entendido.

{rol}=
```





