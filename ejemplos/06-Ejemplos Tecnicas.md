# Ejemplos de Técnicas

- [Ejemplos de Técnicas](#ejemplos-de-técnicas)
  - [Razonamiento análogico](#razonamiento-análogico)
  - [Chain of Thought (CoT)](#chain-of-thought-cot)
  - [Prompt Chaining](#prompt-chaining)
  - [Automatic Chain of Thought (Auto-CoT)](#automatic-chain-of-thought-auto-cot)





## Razonamiento análogico

Se solicita realizar un paralelismo entre conceptos

Facilita encontrar similitudes entre dominios, para una comprensión más profunda y con una resolución mas innovadora.

Ventajas:

* Simplificar ideas complejas o abstractas
* Generar metáforas y analogías
* Resolución creativa de problemas

***Ejemplo 1:*** Texto original

```bash
Explain the concept of a computer network using the analogy of a city's transportation system.
```





## Chain of Thought (CoT)

Enfoque de técnica de prompting donde:

Se solicita a la IA que exponga su proceso de razonamiento lógico paso a paso y de forma coherente. Así se puede ver como llega a esa conclusión. Facilita el entender el "por qué" y por lo tanto proporciona muy buenos resultados al dar una respuesta precisa

Algunas de los textos que se pueden utilizar para esto son:

* "Pensemos paso a paso"
* "Responde razonando paso a paso"
* "Pensémoslo"
* ...

Se puede combinar con Few Shot

Además sobre este texto pòdemos añadir modificadores para obtener textos más interesantes

* "<texto CoT> detenidamente"
* "<texto CoT> en profundidad"
* "<texto CoT> desde otra perspectiva"
* "<texto CoT> como lo haría XXX"
* "<texto CoT> como lo harías en la situación YYY


Ventajas:

* Se utiliza para explicar conceptos complejos, resolver problemas matemáticos, procesos de toma de decisiones con su justificación, etc.

Ejemplo:

```bash
Identifica un problema técnico acuciante en tu comunidad y propón una solución global para mitigar su impacto
```




***Ejemplo 1:*** Detalle explicativo del uso de esta técnica

Texto original

```bash
Q: How do you solve 5x + 3 = 23?
A: First, subtract 3 from both sides to get 5x = 20. Then, divide both sides by 5 to find x = 4.
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




## Prompt Chaining

Enfoque de técnica de prompting donde:

Se divide una acción en una secuencia de acciones donde cada una de ellas se basa en la anterior

Ventajas:

* Exploración detallada de temas complejos
* Aprendizaje o instrucción secuencial
* Situaciones en las que una sola indicación no capta todo el alcance de una tarea

***Ejemplo 1:***

```bash
1. List the ingredients needed to bake a cake.
2. Based on the ingredients listed, what are the steps to bake the cake?
```




## Automatic Chain of Thought (Auto-CoT)

Enfoque de técnica de prompting donde:

Facilita el enseñar al LLM el CoT de forma automatica. Para ello realiza un muestreo de diferentes preguntas, la generación de multiples cadenas de razonamiento para cada una de llas.

Se minimizan los errores
