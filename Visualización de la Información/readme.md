

### UNaB: Universidad Nacional Guillermo Brown
#### 188 - Visualización de la Información

## Prof: Virginia Guerrero
# Alumnos : Euler, Diego - González, Lucas León - Herrera, Marcos Elías.

-----

# Trabajo Práctico Integrador
-----
## Instrucciones

Por favor, utiliza la plantilla RMarkdown provista para completar tu informe. El resultado del documento RMarkdown (en formato HTML) y el archivo RMarkdown sin procesar (como .Rmd) deben ser subidos al campus antes de las 21 hs del martes 19 de noviembre para la comisión 1 y del jueves 21 de noviembre para la comisión 2. Estos dos documentos se calificarán en conjunto, por lo que deben ser coherentes (es decir, no cambies el archivo RMarkdown sin actualizar también el documento HTML).

Todos los resultados presentados deben tener su código correspondiente. Cualquier respuesta/resultado presentado sin el correspondiente código R que generó el resultado no se considerará. Para ser claros: si haces los cálculos a mano en lugar de usar R y luego reportas los resultados de los cálculos, no recibirás puntos por esos cálculos. Todo el código reportado en el documento final del proyecto debe correr sin errores. Por favor, no incluyas ningún código extraño o que produzca mensajes de error (el código que produce advertencias es aceptable, siempre y cuando entiendas lo que significan las advertencias). Por favor, no incluyas instalación de paquetes.

Para este informe, utilizarás la base de datos de meteoritos que contiene información de impactos de meteoritos y su fuente es la NASA. Incluye información sobre más de 45,000 meteoritos, incluyendo su nombre, ubicación, masa y año de impacto.

### Diccionario de Datos

| Variable      | Clase     | Descripción                                                                         |
|---------------|-----------|-------------------------------------------------------------------------------------|
| name          | character | Nombre del meteorito                                                                |
| id            | double    | ID numérico del meteorito                                                           |
| name_type     | character | Tipo de nombre, valid (válido) o relict (un meteorito que no puede ser asignado fácilmente a una clase) |
| class         | character | Clase del meteorito, más detalles en Wikipedia                                       |
| mass          | double    | Masa en gramos                                                                      |
| fall          | character | Fell (alguien vio caer el meteorito) o Found (alguien lo encontró)                   |
| year          | integer   | Año                                                                                 |
| lat           | double    | Latitud                                                                             |
| long          | double    | Longitud                                                                            |
| geolocation   | character | Geolocalización                                                                     |

## Estructura del Informe

Este informe constará de dos partes. Cada parte debe estar estructurada de la siguiente manera:

- **Introducción** (1-2 párrafos)
- **Enfoque** (1-2 párrafos)
- **Análisis** (2-3 bloques de código, 2 figuras, comentarios de texto/código según sea necesario)
- **Discusión** (1-3 párrafos)

Les recomendamos que sean concisos. Un párrafo no debería tener más de 5-6 frases.

No están obligados a realizar ninguna prueba estadística en este proyecto o manipulación de datos complicada, pueden hacerlo si les resulta útil para responder a su pregunta.

### Instrucciones para la Parte 1

En la Parte 1, le proporcionamos una pregunta específica para responder e instrucciones específicas sobre cómo responder a la pregunta.

#### Introducción

En esta sección, escribí una breve introducción al conjunto de datos, la pregunta y qué partes del conjunto de datos son necesarias para responder a la pregunta. Podés repetir parte de la información sobre el conjunto de datos proporcionada anteriormente, parafraseando en tus propios términos y entendiendo con otros detalles. Es importante que te tomes tiempo para entender de qué se trata la base de datos y busques información extra si fuera necesario. Imaginá que tu informe es un documento independiente y que la persona que califica no tiene conocimiento previo del conjunto de datos.

#### Enfoque

Describí los tipos de gráficos que vas a realizar para responder a la pregunta. Para cada gráfico, explicá claramente por qué este gráfico (por ejemplo, diagrama de caja, diagrama de barras, histograma, etc.) es el mejor para proporcionar la información sobre la que se pregunta. Los dos gráficos deben ser de diferentes tipos y al menos uno de ellos debe mapear datos al color o la forma o utilizar facetas (paneles).

#### Análisis

Incluí el código que genera tus gráficos. Utilizá las funciones necesarias para agregar etiquetas de ejes y guías agradables. Podés utilizar funciones de tema para personalizar la apariencia de tu gráfico, pero no es obligatorio hacerlo. Todos los gráficos deben hacerse con ggplot2.

#### Discusión

Interpretá los resultados del análisis. Identificá cualquier tendencia, patrón o relación revelada (o no revelada) por los gráficos. Especulá acerca de por qué los datos tienen el comportamiento que tienen.

### Instrucciones para la Parte 2

En la Parte 2, deberás responder a una segunda pregunta (utilizando el mismo conjunto de datos) y el enfoque, la misma será asignada a cada grupo. Para su resolución, avanzarán de la misma manera que en la parte 1, pero sin repetir el análisis ni las gráficas ya utilizadas.

Para la Introducción, no es necesario que repitas toda la descripción del conjunto de datos de la Parte 1, pero sí que describas las columnas necesarias para responder a tu pregunta.

Respondé a tu pregunta interpretando tus gráficos e identificando las tendencias que revelan o no revelan, según sea el caso.
