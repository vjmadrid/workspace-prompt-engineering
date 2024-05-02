# Generar Datos Sintéticos


## Generación de un fichero JSON


**Ejemplo 1: Crear un ejemplo**

```bash
Necesito que generes un archivo JSON con 2 de las ciudades más populares de la UE.

JSON debe tener las siguientes variables: ciudad, país, código de país y número de teléfono correcto de acuerdo a la ciudad.
```

**Ejemplo 2: Crear datos adicionales**

```bash
Basado en el JSON anterior, puedes generar {num_casos} casos extra

{num_casos}=5
```





## Generación de un fichero YAML

```bash
Necesito que generes un fichero YAML con {num_productos} productos aleatorios en su interior.
Puede agregar tanta complejidad como sea posible

{tipo_fichero}=YAML
{num_productos}=6
```

## SQL Data Generation

**Ejemplo 1**

```bash
Necesito que genere un script SQL donde ponga algunos datos a la tabla {nombre_tabla}.
Tiene nombre de usuario, número de pedido, precio del pedido y hora actual.

{nombre_tabla}=CustomOrder
```

**Ejemplo 2**

```bash
Necesito que genere un script SQL donde ponga algunos datos a la tabla {nombre_tabla}.
Tiene nombre de usuario, número de pedido, precio del pedido y hora actual.
La segunda tabla con nombre {nombre_tabla_2} debe tener id, nombre de usuario, número de teléfono y dirección. 
Quiero tener la consulta join que relaciona las dos tablas y que me escriba el resultado.

{nombre_tabla}=CustomOrder
{nombre_tabla_2}=CustomUser


```


```bash
Crear una lista seleccionada de casos de uso para ChatGPT, cada uno cuidadosamente diseñado para alinearse con {detalle_trabajo}. Esta lista me servirá de guía personalizada, permitiéndome aprovechar las capacidades de ChatGPT en varios aspectos sobre lo anterior. Organiza esta lista en {num_secciones} secciones distintas ordenadas por su relevancia para mi ocupación. En cada sección, construye una tabla con columnas para "Caso de uso" y "Ejemplo de solicitud". Cada sección contendrá {num_ejemplos} ejemplos de casos de uso. El "Ejemplo de solicitud" se redactará en forma de solicitud directa a ChatGPT. Comienza preguntándome por mi ocupación, y en base a ella rellena los intereses, objetivos, retos a los que me enfrento.

{detalle_trabajo}=el trabajo de probar aplicaciones
{num_secciones}=10
{num_ejemplos}=5
```