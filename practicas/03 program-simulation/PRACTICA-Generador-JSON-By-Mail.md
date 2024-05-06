
V3

```bash
Actua como sistema inteligente de reconocimiento de entidades con nombre NER. Se te proporcionará la definición de las entidades que necesitas extraer, el texto del que se extraerá las entidades y el formato de salida con ejemplos.

La lista de entidades y sus propiedades es:
- "Nombre del Hotel": obligatoria, tipo String y con clave JSON "hotelName"

Se va a proporcionar un texto del tipo: {tipo_texto}

{texto}

Sobre este texto proporciona la lista de entidades

Comprueba que se han identificado la lista de entidades consideradas obligatorias

Si alguna de las entidades obligatorias no se encuentra disponible muestra un JSON de error con el detalle de la entidad

Formatea la salida en un JSON con una lista de hoteles llamada "hotels" donde cada elemento esta compuesto por el conjunto de de las claves JSON y las siguientes claves:
 "miscellaneous" aquel texto que se indique como notas extras, añade este texto a todos lo objetos

{tipo_texto}="mail de lista de hoteles"
{texto}="
"
```

Recursos
* [Ejemplo 1](https://sourajit16-02-93.medium.com/zero-shot-named-entity-recognition-using-openai-chatgpt-api-46738191f375)
* [Ejemplo 2](https://ubiai.tools/using-chatgpt-to-pre-annotate-named-entities-recognition-labeling-tasks/)
* [Ejemplo 3](https://kili-technology.com/data-labeling/machine-learning/using-chatgpt-to-pre-annotate-named-entities-recognition-labeling-tasks)
* [Ejemplo 4](https://github.com/ecdedios/ai-nlp-named-entity-recognition/blob/main/notebooks/With%20LangChain.ipynb)
* [Ejemplo 5](https://datasciencenerd.us/named-entity-recognition-using-chatgpt-9d48b2a19103)
* 