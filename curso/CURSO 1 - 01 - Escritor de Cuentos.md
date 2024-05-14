# Curso 1: Escritor de Cuentos

- [Curso 1: Escritor de Cuentos](#curso-1-escritor-de-cuentos)
  - [Parte Creativa](#parte-creativa)
    - [Generar Ideas](#generar-ideas)
      - [Prompts "Ad-hoc"](#prompts-ad-hoc)
      - [Role prompting](#role-prompting)
      - [Ajuste de Ideas](#ajuste-de-ideas)
    - [Seleccionar Título](#seleccionar-título)
      - [Crear un título](#crear-un-título)
      - [Ajustar el titulo](#ajustar-el-titulo)
  - [Parte de Escritura](#parte-de-escritura)
    - [Resumir la idea](#resumir-la-idea)
    - [Trabajar en escenarios y ambientaciones](#trabajar-en-escenarios-y-ambientaciones)
    - [Creación de personales](#creación-de-personales)
    - [Escritura de Capitulos](#escritura-de-capitulos)
  - [Rol prompting](#rol-prompting)



## Parte Creativa

### Generar Ideas

Facilita encontrar ideas originales que puedan servir como argumento y así ayudar a potener la imaginación humana

#### Prompts "Ad-hoc"

```bash
Genera ideas para crear un cuento sobre un grupo de amigos basado en una experiencia personal de superación
```

Templetiza tu prompt

```bash
Genera {numero} ideas para crear un cuento sobre {tematica} {contexto}

{numero}=10
{tematica}=un grupo de amigos
{contexto}=una experiencia personal de superación
```

Mejora sobre el prompt

```bash
Genera {numero} ideas para crear un cuento sobre {tematica} {contexto} dirigido a {publico}

{numero}=10
{tematica}=un grupo de amigos
{contexto}=una experiencia personal de superación
{publico}=niños de entre 5 y 9 años
```

#### Role prompting

```bash
Actua como una IA especializada en la generación de ideas creativas para la escritura de cuentos. Escribe {numero} ideas para crear un cuento sobre {tematica} {contexto}

{numero}=10
{tematica}=un grupo de amigos
{contexto}=una experiencia personal de superación
```




#### Ajuste de Ideas

Puede ser interesante realizar una serie de acciones sobre las propuestas con el objetivo de afinar mucho mejor la idea

```bash
Simplifica la lista con las que consideres mejores
```

```bash
Elimina el primero
```

```bash
Me gustan el 1 y el 3 ¿Explicame que pros y contras tiene cada uno?
```

```bash
Si solo pudieras elegir uno, ¿Cuál sería?
```

```bash
¿Cómo lo mejorarías?
```




### Seleccionar Título

La clave del exito del cuento puede estar en el titulo, lo tanto puede ser interesante trabajar en ellos


#### Crear un título

```bash
Escribe un título original y llamativo para el cuento anterior
```

```bash
Escribe un título original y llamativo para un cuento que habla sobre {tema}

{tema}=
```

```bash
Puedes hacer que los titulos sean más infantiles
```

#### Ajustar el titulo

```bash
Modifica y acorta el título de este cuento sea más divertido
```


## Parte de Escritura

### Resumir la idea

```bash
Genera un breve resumen del cuento
```

### Trabajar en escenarios y ambientaciones

El trabajo sobre el ambiente del libro

```bash
Desarrolla una descripción sobre el ambiente {lugar} en un bosque de Alemania. Utiliza {herramientas}.

{lugar}=campamento de verano
{herramientas}=los 5 sentidos para crear una experiencia sensorial
```

```bash
Desarrolla una descripción en el que se refleje el tono y estado de animo de {situacion} y que {contexto}

{situacion}=un niño que ha perdido recientemente a su perro
{contexto}=se encuentra asistiendo al campamento obligado por sus padres
```


### Creación de personales

```bash
Escribiendo un cuento sobre amistad. Describe la relacion entre dos personas que son enemigos pero que están condenados a entenderse. La primera persona es un niño con gafas, alergias y muy malo en los deportes. La segunda persona es un niño más mayor que es el malote de la clase
```

```bash
Actua como un escritor experto en el desarrollo de personajes. Crea un perfil detallado para {ambiente} de un personaje de un cuento. {características}

{ambiente}=
{características}=
```



### Escritura de Capitulos

```bash
Escribe la introducción para un libro de no ficción titulado {titulo} sobre {contexto}. Debe tener alrededor de {num_palabras} e incluir una descripción general del libro así como los principales temas e ideas que se abordarán.

{titulo}=El Mapa de la Amistad
{contexto}=
{num_palabras}=200
```


## Rol prompting

```bash
Actua comoun experimentado escritor de cuentos con un profundo entendimiento de las emociones humanas y una habilidad especial para tejer historias conmovedoras. Utiliza tus habilidades para escribir un cuento corto basado en una experiencia personal que haya marcado tu vida significativamente. Asegúrate de que tu historia transmita no solo los eventos, sino también las emociones y reflexiones íntimas que estos generaron. Incorpora detalles vívidos para hacer que la narración sea más envolvente y utiliza diálogos realistas para dar voz a los personajes involucrados. Finalmente, añade una moraleja o enseñanza que refleje el impacto y la importancia de esta experiencia en tu desarrollo personal y emocional. Tu objetivo es crear un relato que no solo entretenga, sino que también ofrezca una perspectiva profunda y genuina sobre la vida y sus desafíos.
```