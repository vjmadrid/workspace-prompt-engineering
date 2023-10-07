# Ejemplos

- [Generación de texto](#generación-de-texto)
- [Clasificar información](#clasificar-información)
- [Resumen de un texto](#resumen-de-un-texto)





## Generación de texto

Realmente lo que hace es completar texto





## Clasificar información

```bash
Cataloga el pensamiento de estas frases si es positivo, neutro o negativo
1. Me gusta dormir
2. Odio el brocoli
3. Adoro la pasta con pesto
4. 3*3=9
```



## Resumen de un texto

```bash
XXX

Resume este párrafo en una sola oración:
```


## Reescritura de texto

```bash
XXX

Reescribe el texto anterior. Cambia el formato
```



## Extraer informacion


### Preguntas y respuestas

Con un poco de context learning lo hace

```bash
¿Cuando se descubrio la bombilla?
```


Si no ha sido entrenado con esa informacion
```bash
¿Cuanto mide el mueble Logorjander de Ikea?
```

Pero si le damos la informacion entonces si
```bash
El mueble de salón Logorjander...

¿Cuanto mide el mueble Logorjander de Ikea?
```



## Resolución de problemas matemáticos

```bash
¿Cuánto es 985*650?
```

A veces se responde incorrectamente

GPT-3 (text-davinci-003)

```bash
¿Cuánto es 985*650?
Asegúrese de que su respuesta es exactamente correcta.
```

### Entender temas complejos

```bash
Explícame la teoría de la relatividad en términos sencillos. Explícamelo como si tuviera 11 años.
```

### Redactar con un estilo

```bash
Bla, bla, bla”. Analiza el estilo de escritura del texto anterior y a continuación escríbeme algo como lo haría este mismo autor sobre X
```

### Consultar a gente importante

```bash
Te voy a dar un argumento u opinión mía. Quiero que lo critiques como si fueras Steve Jobs
```

### Reemplazar texto por otra cosa

```bash
Lea el siguiente correo electrónico de xxx.
Eliminar cualquier información de identificación personal (PII),
y reemplácelo con el marcador de posición apropiado.
Por ejemplo, reemplace el nombre "Victor xxx"
con "[NOMBRE]"

XXX
```


## Cloze Prompt o Completar

```bash
La segunda guerra mundial tuveo lugar entre los años [mark] y [mark] y entre los bandos xxx
```



### Ejemplo de Chainb of Thought

```bash
Vas a la tienda y compras una raqueta de tenis y una pelota. En total, todo cuesta 65 euro. la raqueta cuesta 60 euros más que la pelota
```



```bash
Vas a la tienda y compras una raqueta de tenis y una pelota. En total, todo cuesta 65 euro. la raqueta cuesta 60 euros más que la pelota

Transforma la información anterior en ecuaciones y explicalo paso a paso
```



Crear un artículo de 400 palabras sobre XXX
Resumen de la respuesta anterior
Alguna pregunta sobre ese nombre
Pedir una traducción del
Generacion del código

Por ejemplo:
Prompt:
### Instrucción ### Traduce el texto a continuación al español: Texto: "Hello!"
Resultado:
¡Hola!


Ejemplo 
Prompt:
Extrae los nombres de lugares del siguiente texto. Formato deseado: Lugar: <lista_separada_por_comas_de_nombres_de_empresa> Input: "Aunque estos avances son alentadores para los investigadores, aún hay mucho misterio. 'A menudo tenemos una caja negra entre el cerebro y el efecto que vemos en la periferia', dice Henrique Veiga-Fernandes, un neuroinmunólogo en el Centro Champalimaud para lo Desconocido en Lisboa. 'Si queremos usarlo en el contexto terapéutico, necesitamos entender el mecanismo'.
Resultado:
Place: Centro Champalimaud para lo Desconocido, Lisboa

Por ejemplo, podrías estar interesado en aprender el concepto de ingeniería de prompts. Podrías intentar algo como:
Explica el concepto de ingeniería de promoción. Mantén la explicación corta, solo unas pocas frases y no seas demasiado descriptivo.
No está claro en la instrucción anterior cuántas oraciones utilizar y qué estilo. Es posible que puedas obtener respuestas aceptables con el prompt anterior, pero un prompt que sea muy específico, conciso y directo sería mejor. Algo como:
Usa 2-3 oraciones para explicar el concepto de ingeniería de prompt a un estudiante de secundaria.


## Role prompting

Eres un médico. Lee esta historia clínica y predice los riesgos para el paciente:


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


## Creación de texto


```bash
Mi Nombre: Mario
Nombre del Jefe: John

Escribe un correo electrónico a mi jefe diciendo que estaré fuera de la oficina hoy ya que estoy enfermo.
```