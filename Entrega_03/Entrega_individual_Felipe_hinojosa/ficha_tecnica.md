ficha


| Variable  |                           Descripción                            |      Tipo       |             Valores posibles             |                                                 Observación                                                 |
|:---------:|:----------------------------------------------------------------:|:---------------:|:----------------------------------------:|:-----------------------------------------------------------------------------------------------------------:|
| Temporada | Año calendario del torneo                                        | Numérico        | 2018 -2025                               | Corresponde al año de campeonato                                                                            |
| Equipo    | Nombre                                                           | texto           | 25 equipos                               | incluye equipos que no jugaron en primera durante todo el periodo                                           |
| Técnicos  | Nombres de los técnicos                                          | texto           | uno o más nombres separados por una coma | Puede estar incompleto si Transfermarkt no tiene el registro                                                |
| Cantidad  | Número de técnicos distintos que dirigieron al equipo en ese año | Numérico entero | 0 en adelante                            | El valor 0 indica ausencia de registro, no necesariamente ausencia de técnico                               |
| Cambios   | Número de cambios realizados durante la temporada                | Numérico entero | 0 en adelante                            | Se calcula como cantidad de técnicos menos 1. Un valor de 0 indica que el mismo técnico dirigió todo el año |
