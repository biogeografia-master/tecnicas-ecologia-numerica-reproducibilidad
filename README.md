Práctica de desarrollo 2. PD02. Técnicas de ecología numérica,
reproducibilidad<small><br>Biogeografía (GEO-131)<br>Universidad
Autónoma de Santo Domingo (UASD)<br>Semestre 2024-02</small>
================
El Tali
2024-10-01

<!-- README.md se genera a partir de README.Rmd. Por favor, edita ese archivo. -->

Versión HTML (quizá más legible),
[aquí](https://biogeografia-master.github.io/tecnicas-ecologia-numerica-reproducibilidad/README.html)

# Fecha/hora de entrega

**8 de octubre de 2024, 11:59 pm.**

# Objetivos

Vamos a “calentar motores”. El objetivo de esta práctica de desarrollo
es que demuestres o mejores lo siguiente: a) Tus capacidades de realizar
análisis cuantaitativos con datos de comunidad y ambientales usando R;
b) Tus capacidades de generar cuadernos reproducibles con RMarkdown; c)
tus capacidades de redacción. Esto te preparará, a futuro, para el
manuscrito.

Esta práctica tratará **sobre técnicas de ecología numérica usando datos
de GBIF (GBIF.org, 2022) y el repositorio de estadística zonal sobre RD
de Martínez-Batlle (2022)**, intentando que sea una investigación
reproducible y bien redactada (nada de alto nivel, sólo estamos
ensayando). Lo ideal es que presentes un un documento que cumpla con
estilos de formato, uso apropiado de figuras, tablas, citas y
referencias.

# Mandato

1.  Elige un número entre el 2 y el 20, y toma la matriz de comunidad y
    la matriz ambiental asociadas a ese número, según la tabla que se
    muestra abajo. Los archivos que usarás se encuentran en el
    directorio [salidas_RDS/](salidas_RDS/), y ocasionalmente podrían
    usarse los de los directorios [salidas_mc/](salidas_mc/) y
    [salidas_ma/](salidas_ma/)que son las matrices de comunidad y
    ambiental pero separadas del resto de objetos. Anuncia en el foro el
    número que elijas.

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

2.  Consulta el [ejemplo de análisis](ejemplo%20de%20análisis.Rmd) que
    realicé con los datos del conjunto 1, familia Acanthaceae .

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
    Teoría sobre los modos Q y R, Orlóci”) en adelante.

4.  Redacta un miniartículo. Para el procesamiento de tu texto y tus
    análisis, usa la plantilla
    `manuscrito-tecnicas-ecologia-numerica-reproducibilidad.Rmd` que se
    encuentra en este mismo repositorio. Para hacerlo, deberás clonar
    este repositorio, yendo al [portal de la
    asignatura](https://github.com/biogeografia-202402), haz clic en el
    enlace de la PD02 y acepta la asignación. Deberás usar estilos de
    formato (los títulos debidamente escritos, el texto normal también,
    siguiendo lo aprendido en la práctica de desarrollo anterior),
    referencias bibliográficas, referencias cruzadas a figuras y tablas
    (es decir, necesitarás que las figuras y tablas tengan título o
    “*caption*”). No podrás desarrollar tu redacción usando listas de
    viñetas ni listas numeradas. Debes usar la plantilla mencionada en
    RStudio, preferiblemente en mi servidor, tal como hiciste en la PD
    anterior. Distribuye tu texto en las siguientes secciones:

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
  [https://github.com/biogeografia-master/tecnicas-ecologia-numerica-reproducibilidad/matrices-de-comunidad-y-ambiental.Rmd](matrices-de-comunidad-y-ambiental.Rmd).
  Debes citar el repo oportunamente. Si hiciste el clonado, dicho
  archivo se encuentra tu repositorio clonado también. Puedes consultar
  las versiones [HTML](matrices-de-comunidad-y-ambiental.html) y
  [Markdown](matrices-de-comunidad-y-ambiental.md) que se encuentran en
  este mismo repositorio.

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

## Referencias

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
