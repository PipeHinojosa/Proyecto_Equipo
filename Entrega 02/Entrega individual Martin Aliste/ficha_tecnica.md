# Ficha técnica y diccionario de datos

## Fuente de los datos: 
La información fue obtenida de la página Transfermarkt

## Metodología de la construcción de la base:
La base de datos se obtuvo mediante la técnica de web scraping. Se programó un bot que mediante Python y las librerías Request y BeautifulSoup pudiera acceder a toda la información de la página, logrando obtener información detallada sobre los técnicos de cada equipo y ser traspasada a una planilla de excel mediante Pandas.

## Alcance de los datos:
La base incluye solo a los equipos que participaron en cada temporada de la primera división del fútbol chileno entre el 2018 y 2025. No incluye otro tipo de torneos nacionales.

## Característica de los datos:
Los datos tienen frecuencia anual y están organizados a nivel de equipo por temporada. Cada fila representa la combinación de un equipo y un año, indicando cuántos técnicos distintos lo dirigieron durante ese período y la fecha de inicio y término. La variable principal de análisis es el número de cambios de técnico por temporada. Los nombres de los técnicos se incluyen en formato de texto separado por comas.

## Otras observaciones que tengan sobre la base:
La base no distingue entre técnico titular y técnico interino, lo que puede inflar el conteo de cambios en casos donde un ayudante asumió de forma provisional por pocos partidos.

## Diccionario de datos: tabla con el nombre de cada variable, su descripción, tipo de dato, valores posibles y observaciones editoriales (si aplica):

| Variable  |                           Descripción                            |      Tipo       |             Valores posibles             |                                                 Observación                                                 |
|:---------:|:----------------------------------------------------------------:|:---------------:|:----------------------------------------:|:-----------------------------------------------------------------------------------------------------------:|
| Temporada | Año calendario del torneo                                        | Numérico        | 2018 -2025                               | Corresponde al año de campeonato                                                                            |
| Equipo    | Nombre                                                           | texto           | 25 equipos                               | incluye equipos que no jugaron en primera durante todo el periodo                                           |
| Técnicos  | Nombres de los técnicos                                          | texto           | uno o más nombres separados por una coma | Puede estar incompleto si Transfermarkt no tiene el registro                                                |
| Cantidad  | Número de técnicos distintos que dirigieron al equipo en ese año | Numérico entero | 0 en adelante                            | El valor 0 indica ausencia de registro, no necesariamente ausencia de técnico                               |
| Cambios   | Número de cambios realizados durante la temporada                | Numérico entero | 0 en adelante                            | Se calcula como cantidad de técnicos menos 1. Un valor de 0 indica que el mismo técnico dirigió todo el año |
