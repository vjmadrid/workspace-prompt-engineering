# Ejemplos de Best Practices


- [Ejemplos de Best Practices](#ejemplos-de-best-practices)
  - [Chain of Thought](#chain-of-thought)
  - [Uso de marcado de lenguajes de programación](#uso-de-marcado-de-lenguajes-de-programación)
  - [Solicitar Feedback](#solicitar-feedback)
  - [Resumir mejor parrafo a parrafo](#resumir-mejor-parrafo-a-parrafo)
  - [Cambiar de conversación](#cambiar-de-conversación)
  - [Solicitar varias acciones en el mismo prompt para optimizar](#solicitar-varias-acciones-en-el-mismo-prompt-para-optimizar)





## Chain of Thought


***Ejemplo 1:*** Detalle explicativo del uso de esta técnica

Texto original

```bash
Vas a la tienda y compras una raqueta de tenis y una pelota. En total, todo cuesta 65 euro. la raqueta cuesta 60 euros más que la pelota
```

Adaptación

```bash
Vas a la tienda y compras una raqueta de tenis y una pelota. En total, todo cuesta 65 euro. la raqueta cuesta 60 euros más que la pelota

Transforma la información anterior en ecuaciones y explicalo paso a paso
```

***Ejemplo 2:*** Detalle explicativo del uso de esta técnica

Texto original

```bash
Fui al mercado y compré 10 manzanas. Regalé 2 manzanas al vecino y 2 al reparador. Luego fui y compré 5 manzanas más y me comí 1. ¿Cuántas manzanas me quedan?
```

Adaptación

```bash
Fui al mercado y compré 10 manzanas. Regalé 2 manzanas al vecino y 2 al reparador. Luego fui y compré 5 manzanas más y me comí 1. ¿Cuántas manzanas me quedan? Pensemos paso a paso.
```

Algunas de los textos que se pueden utilizar para esto son:

* "Pensemos paso a paso"
* "Responde razonando paso a paso"
* "Pensémoslo"
* ...

Además sobre este texto pòdemos añadir modificadores para obtener textos más interesantes

* "<texto CoT> detenidamente"
* "<texto CoT> en profundidad"
* "<texto CoT> desde otra perspectiva"
* "<texto CoT> como lo haría XXX"
* "<texto CoT> como lo harías en la situación YYY





## Uso de marcado de lenguajes de programación

**Ejemplo 1:** Usar etiquetas para estructurar el prompt

Variante 1

```bash
He escrito el siguiente texto: "{texto}"

¿Cómo lo podrías mejorar?

{texto}=XXX
```

Variante 2

```bash
Tengo este parrafo: "{texto}"
Extrae los puntos más relevantes en una lista numerada

{texto}=XXX
```

**Ejemplo 2:** Actualización del valor del texto

```bash
{texto}=YYY
```

**Ejemplo 3:** Usar etiquetas como recordatorio

```bash
Recuerdame que son las siguientes etiquetas (mantén el formato de llaves e igualdades para responder)

{rol}=
{situacion}=
{soluciones}=
```

**Ejemplo 3:** Usar etiquetas basadas en HTML


Texto original

```bash
Escribe un post sobre el amor siguiendo la estructura siguiente:

<h1>{título}</h1>
<h2>¿Qué es el amor?</h2>
<p>El amor es {explicación hormonal}</p>
<p>{el amor entre perros}</p>
```





## Solicitar Feedback

**Ejemplo 1:** Pedir mejoras sobre un texto

Variante 1

```bash
He escrito el siguiente texto: "XXX"

¿Cómo lo podrías mejorar?
```

Variante 2

```bash
He escrito este texto.¿Cómo lo podrías mejorar?

"XXX"
```

Variante 3

```bash
He escrito este texto: "XXX"

¿Cómo lo mejorarías?
```





## Resumir mejor parrafo a parrafo

**Ejemplo 1:** Pedir mejoras

```bash
Resume los siguientes textos (60 palabras para cada resumen)

1. "XXX"
2. "YYY"
3. "ZZZ"
```





## Cambiar de conversación

No requiere tener que reiniciar la conversación

**Ejemplo 1:** Reiniciar una conversación

```bash
Bueno, vamos a cambiar de tema. ¿Quiero crear una idea para una película de dinosaurios?
```

**Ejemplo 2:** Reiniciar una conversación reduciendo la contaminación

Variante 1

```bash
Ignora todas las instrucciones anteriores. Vamos a cambiar de tema y no vamos a reutilizar nada de los anterior ¿Esta claro?
```

Variante 2

```bash
Ignora todas las instrucciones anteriores. Cambiaremos de tema de forma radical. No quiero que las respuestas anteriores condiciones las próximas respuestas ¿Esta claro?
```





## Confirmar que algo se ha entendido

**Ejemplo 1:** Confirmación

Variante 1: Puede contestar sí sin saber que esta pasando

```bash
Si lo has entendido, contesta con un "Sí"
```

Variante 2: Puede contestar sí sin saber que esta pasando

```bash
Parafrasea cual es tu XXX para confirmar que lo has entendido
```




## Solicitar varias acciones en el mismo prompt para optimizar

**Ejemplo 1:** Variaciones del mismo texto

Variante 1

```bash
Traduce el siguiente texto [texto acción]: 1. Inglés, 2. Frances, 3. Italiano
```

Variante 2

```bash
Traduce el siguiente texto [texto acción] al ingles pero con las siguientes variantes: 1. Técnico, 2. Formal, 3. Popiular
```

**Ejemplo 3:** Pedir variaciones con diferentes funcionalidad

Variantes 1

```bash
Se quiere reescribir un [texto utilizado] para las diferentes redes sociales, cada una con el TONO que se suele utilizar  (más cachondo para Twitter, más serio para LinkedIn, más inspirador para Instagram, etc).
```

Se supone que que el texto es un PÁRRAFO de 80 tokens
