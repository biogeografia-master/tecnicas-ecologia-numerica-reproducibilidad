Práctica de desarrollo 2. PD02. Técnicas de ecología numérica,
reproducibilidad<small><br>Biogeografía (GEO-131)<br>Universidad
Autónoma de Santo Domingo (UASD)<br>Semestre 2024-02</small>
================
El Tali
2024-10-02

<!-- README.md se genera a partir de README.Rmd. Por favor, edita ese archivo. -->

Versión HTML (quizá más legible),
[aquí](https://biogeografia-master.github.io/tecnicas-ecologia-numerica-reproducibilidad/README.html)

# Fecha/hora de entrega

**8 de octubre de 2024, 11:59 pm.**

# Objetivos

Vamos a “calentar motores”. El objetivo de esta práctica de desarrollo
es que demuestres o mejores lo siguiente:

1.  Tus capacidades de realizar análisis cuantaitativos con datos de
    comunidad y ambientales usando R.

2.  Tus capacidades de generar cuadernos reproducibles con RMarkdown.

3.  Tus capacidades de redacción. Esto te preparará, a futuro, para el
    manuscrito.

Esta práctica tratará **sobre técnicas de ecología numérica usando datos
de GBIF (GBIF.org, 2022) y el repositorio de estadística zonal sobre RD
de Martínez-Batlle (2022)**, intentando que sea una investigación
reproducible y bien redactada (nada de alto nivel, sólo estamos
ensayando, pues el objetivo es aprender, no elevar el *H-index*). Lo
ideal es que presentes un un documento que cumpla con estilos de
formato, uso apropiado de figuras, tablas, citas y referencias, pero
usando datos reales aplicados a RD.

# Mandato

1.  Elige un número entre el 2 y el 20, el cual representará tu familia
    elegida según la tabla que se muestra abajo. Anuncia en el foro el
    número que elijas. Normalmente, usarás la matriz de comunidad y la
    matriz ambiental asociadas a dicha familia. Los archivos fuente de
    donde obtendras dichas matrices se encuentran en el directorio
    `salidas_RDS/`. En el referido directorio hay muchos archivos, pero
    el que te interesa más es el que comienza por
    todos_los_objetos_NOMBREDEFAMILIA.RDS. Dichos archivos contienen
    todos los subproductos generados para la familia en cuestión, usando
    los datos de GBIF y del repositorio de estadística zonal sobre la
    familia elegida. El script con el que se generaron todos los
    subproductos se llama
    [matrices-de-comunidad-y-ambiental.html](https://biogeografia-master.github.io/tecnicas-ecologia-numerica-reproducibilidad/matrices-de-comunidad-y-ambiental.html)
    (tiene versión Markdown también). Ocasionalmente podrían usarse los
    archivos de los directorios `salidas_mc/` y `salidas_ma/`, que son
    también las matrices de comunidad y ambiental, respectivamente, pero
    separadas del resto de objetos.

| estudiante | familia             |
|-----------:|:--------------------|
|          1 | Acanthaceae         |
|          2 | Solanaceae          |
|          3 | Asteraceae          |
|          4 | Phyllostomidae      |
|          5 | Fabaceae            |
|          6 | Tyrannidae          |
|          7 | Euphorbiaceae       |
|          8 | Cactaceae           |
|          9 | Orchidaceae         |
|         10 | Bromeliaceae        |
|         11 | Rubiaceae           |
|         12 | Eleutherodactylidae |
|         13 | Nymphalidae         |
|         14 | Melastomataceae     |
|         15 | Myrtaceae           |
|         16 | Trochilidae         |
|         17 | Orthoptera          |
|         18 | Thraupidae          |
|         19 | Piperaceae          |
|         20 | Poaceae             |

2.  Consulta el [ejemplo de
    análisis](https://biogeografia-master.github.io/tecnicas-ecologia-numerica-reproducibilidad/ejemplo-de-analisis.html)
    que realicé con los datos del conjunto 1, familia Acanthaceae. Te
    recomiendo que veas el código de R también, abriendo el documento
    `ejemplo-de-análisis.Rmd` que se encuentra en este mismo repo o en
    el enlace
    [ejemplo-de-análisis.Rmd](https://github.com/biogeografia-master/tecnicas-ecologia-numerica-reproducibilidad/blob/main/ejemplo-de-analisis.Rmd);
    no te quedes sólo en el documento HTML, pues es más fácil usar el
    .Rmd para ejecutar, bloque a bloque, el código de R (recuerda
    desactivar el traductor para el servidor si aún lo tienes activado).
    Tal como lo lees, es importante ejecutar bloque a bloque, o línea a
    línea, para ver qué cosas producen las maravillosas líneas de R.
    Intentar comprenderlas también es importante, pero puede resultar
    abrumador. Lo más importante es que adaptes el código de dicho
    cuaderno a tu familia elegida, editando las líneas allí donde tengas
    que hacerlo (no son muchos lugares realmente que necesitas
    personalizar) sobre él propio cuaderno. Recuerda que el código en
    dicho cuaderno sigue una lógica secuencial, por lo que los bloques
    posteriores ocasionalmente podrían depender de los anteriores.

En los vídeos a continuación muestro qué extraer de los análisis que
ejecuta el código de ejemplo. Los vídeos muestran datos ficticios o
referidos a otros subconjuntos de semestres anteriores, pero la
explicación sobre los patrones potencialmente aprovechables es
igualmente válida.

- [20240307-20240314-video-1-tutoriales-practica-3-tecnicas-de-ecologia-numerica-reproducibilidad-redaccion-estilos-citas-referencias.mp4.
  **Del minuto 10 al
  15**](https://drive.google.com/file/d/1LZeTjMnM5PFzG3zhLOC3Jaf22k1pnxlU/view?usp=sharing)

- [Práctica 4. Metodología y resultados de ecología numérica. Intro,
  análisis exploratorio de
  datos](https://www.youtube.com/watch?v=2E5G3eC3E_Y)

- [Práctica 4. Metodología y resultados de ecología numérica. Análisis
  de agrupamiento](https://www.youtube.com/watch?v=eJ8bMHDAyvE)

- [Práctica 4. Metodología y resultados de ecología numérica. Técnicas
  de ordenación](https://www.youtube.com/watch?v=YeZU9iZhvNg)

- [Práctica 4. Metodología y resultados de ecología numérica. Análisis
  de diversidad](https://www.youtube.com/watch?v=U5eImkQfwKk)

3.  Desarrolla análisis aplicando **todas las técnicas de ecología
    numérica posibles** (el ejemplo es una buena base, pero puedes
    incluir otras técnicas). Al hacerlo, obtendrás un conjunto de
    resultados. Usa todos los apoyos que necesites, desde el libro de
    Borcard et al. (2018), hasta inteligencia artificial (IA). Si usas
    IA, no le pidas que te resuelva el mandato tal cual y luego
    copiando\>pegando textos o código. Más bien, pídele que te explique
    cómo resolverlo y hazlo por tu cuenta (modo tutor). Revisa
    demostraciones y aplicaciones en Borcard et al. (2018), así como la
    lista de reproducción [Ecología numérica con
    R](https://www.youtube.com/playlist?list=PLDcT2n8UzsCRDqjqSeqHI1wsiNOqpYmsJ),
    desde el vídeo número 10 (“ma_1: Medición de asociación, parte 1.
    Teoría sobre los modos Q y R, Orlóci”) en adelante (esta lista usaba
    datos de la isla Barro Colorado, Panamá).

4.  Redacta un manuscrito. Para el procesamiento de tu texto y la
    redacción de tus análisis, usa la plantilla
    `manuscrito-tecnicas-ecologia-numerica-reproducibilidad.Rmd` que se
    encuentra en este mismo repositorio. Con esta plantilla generarás un
    PDF que tejeras a usando RStudio. Para hacerlo, deberás clonar este
    repositorio, yendo al [portal de la
    asignatura](https://github.com/biogeografia-202402), haz clic en el
    enlace de la PD02 y acepta la asignación. Deberás usar estilos de
    formato (los títulos debidamente escritos, el texto normal también,
    siguiendo lo aprendido en la práctica de desarrollo anterior),
    referencias bibliográficas, referencias cruzadas a figuras y tablas
    (es decir, necesitarás que las figuras y tablas tengan título o
    “*caption*”). No podrás desarrollar tu redacción usando listas de
    viñetas ni listas numeradas. Debes usar la plantilla mencionada en
    RStudio, preferiblemente en mi servidor, tal como hiciste en la PD
    anterior. Cuando termines tu manuscrito con tus análisis
    reproducibles, y lo tejas a PDF, no olvides hacer commit\>push de
    todos tus cambios para subirlos a GitHub.

Distribuye tu texto en las siguientes secciones:

- **Introducción** (tamaño recomendado: 3 párrafos). Desde lo amplio,
  puedes comenzar escribiendo sobre GBIF y su potencial, el repositorio
  de estadística zonal de RD (Martínez-Batlle, 2022), así como sobre la
  familia elegida y su importancia en RD. A continuación, explica en qué
  consisten las técnicas de ecología numérica que aplicarás, su
  importancia, por qué son útiles. Plantea tu o tus objetivos, que en
  este caso están algo acotados. Cierra con la importancia que reviste
  técnicas de ecología numérica a la familia que has elegido respecto
  del conjunto de la ciencia.

  - Dentro de esta sección, debes incluir al menos cinco citas. Los
    conceptos y afirmaciones ajenas, deben citarse bibliográficamente, y
    nunca deberás usar cita textual, pues se considera plagio. Las citas
    bibliográficas que incluyas, deberán estar respaldadas por su
    correspondiente lista referencias, que deberá aparecer en la sección
    final (Referencias), la cual el propio tejido de RMarkdown debería
    generar por ti, siempre que sigas las instrucciones correspondientes
    (vuelve al vídeo de la PD01 para refrescar). Las citas y la lista de
    referencias, deberán seguir el estándar APA 7ma edición (APA7), que
    es el que la propia plantilla tiene configurado por defecto; en
    principio, no tendrás que ocuparte de todos los detalles de sintaxis
    del formato APA7, pero no debes confiar ciegamente en lo que hace
    RMarkdown.

- **Materiales y métodos** (tamaño recomendado: cinco párrafos). Explica
  cómo obtuviste los datos que usaste, y documenta en qué consiste la
  fuente. Los datos de este ejercicio se generaron con el cuaderno
  `matrices-de-comunidad-y-ambiental.Rmd` que se encuentra en este mismo
  repo o que puedes leer en el enlace
  [matrices-de-comunidad-y-ambiental.Rmd](https://github.com/biogeografia-master/tecnicas-ecologia-numerica-reproducibilidad/blob/main/matrices-de-comunidad-y-ambiental.Rmd).
  Debes citar el repo oportunamente. Si hiciste el clonado, dicho
  archivo se encuentra tu repositorio clonado también. Puedes consultar
  las versiones
  [HTML](https://biogeografia-master.github.io/tecnicas-ecologia-numerica-reproducibilidad/matrices-de-comunidad-y-ambiental.html)
  y [Markdown](matrices-de-comunidad-y-ambiental.md) que se encuentran
  en este mismo repositorio.

Debes igualmente citar el software y hardware usado, y las referencias
sobre la técnica o algoritmo empleados. Si incluyes un diagrama de flujo
metodológico (“metodología gráfica”), te resultará más fácil explicar tu
metodología. **No adelantes resultados, sólo escribe que fuentes y
herramientas usaste (materiales) y qué técnicas concretas o algoritmos
utilizaste (métodos)**. Toda figura y tabla que insertes debe citarse
con referencia cruzada, que básicamente se construyen con (más
instrucciones en el aula, por vídeos o por el foro). En el caso de los
cuadernos RMarkdown, las figuras normalmente

- **Resultados** (tamaño recomendado: 4 párrafo). El parámetro o
  variable morfométrica que obtuviste, presentándolo en sus respectivas
  componentes. No hagas valoraciones en esta sección, simplemente
  incluye el resultado obtenido.

- **Discusión** (tamaño recomendado: 4 párrafos). Abre la discusión
  indicando si alcanzaste tus objetivos. Describe por qué era importante
  alcanzarlos. Comenta sobre las limitaciones, de cualquier tipo, ya sea
  las limitaciones de los datos, de la técnicas, de los objetivos de
  aprendizaje. Cierra indicando qué desafíos futuros quedan abiertos
  tras este trabajo.

- **Referencias**. Las referencias que hayas citado en el texto, se
  incluirán automáticamente en la sección “Referencias”. No obstante,
  debes verificar la integridad de las mismas.

> **RECUADRO: recomendaciones básicas de redacción**
>
> Usa una voz (activa o pasiva) de forma consistente, pero sólo ten
> presente que la redacción de manuscritos científicos a menudo se
> utilizan ambas voces, dependiendo del contexto y el mensaje que el/la
> autor/a quiera transmitir. Veamos algunos ejemplos:
>
> **Voz activa en manuscrito científicos:**
>
> - **Analicé** los datos utilizando el software R.
>
> - El experimento **mostró** que la temperatura afecta directamente la
>   tasa de reacción.
>
> - Los investigadores **encontraron** una correlación significativa
>   entre las dos variables.
>
> La voz activa puede hacer que la redacción parezca más directa y
> clara, y es especialmente útil cuando el/la autor/a quiere enfatizar
> quién llevó a cabo una acción o cuándo se desea hacer una afirmación
> fuerte.
>
> **Voz pasiva en artículos científicos:**
>
> - Los datos **fueron analizados** utilizando el software R.
>
> - **Se observó** que la temperatura afecta directamente la tasa de
>   reacción.
>
> - Una correlación significativa **fue encontrada** entre las dos
>   variables.
>
> La voz pasiva es común en la redacción científica porque a menudo se
> prefiere un tono más impersonal, enfocando la atención en los
> resultados y procedimientos en lugar de en quienes llevaron a cabo la
> investigación. También puede ser útil cuando no se quiere o no es
> relevante especificar quién realizó la acción.
>
> **En todas mis prácticas, está completamente permitido usar IA
> (e.g. chatGPT), pero te recomiendo que la uses más como tutor que como
> redactor**. Tal como te sugerí arriba, no le pidas que te resuelva los
> problemas del mandato. Pídele que te dé ideas, y que luego tú las
> mejores o las descartes. No abuses tampoco del texto, pues mucha
> redacción no siempre es mejor; en redacción de ensayos “menos es más”.
> Cruza las redacciones que te ofrezca con tu conocimiento, y revisa si
> los términos o conceptos usados son descabellados (toda IA se inventa
> cosas, cuidate de no caer en esa trampa). Nunca le pidas referencias
> bibliográficas, porque se va equivocar.

# Referencias

<div id="refs" class="references csl-bib-body hanging-indent"
entry-spacing="0" line-spacing="2">

<div id="ref-borcard2018numerical" class="csl-entry">

Borcard, D., Gillet, F. y Legendre, P. (2018). *Numerical ecology with
R*. Springer.

</div>

<div id="ref-gbiforg2022what" class="csl-entry">

GBIF.org. (2022). *What is GBIF?* <https://www.gbif.org/what-is-gbif>

</div>

<div id="ref-jose_ramon_martinez_batlle_2022_7367180" class="csl-entry">

Martínez-Batlle, J. R. (2022). *geofis/zonal-statistics: Let there be
environmental variables* (Versión v0.0.0.9000). Zenodo.
<https://doi.org/10.5281/zenodo.7367256>

</div>

</div>
