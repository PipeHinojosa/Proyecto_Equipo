# Documentación

## Fuentes de Datos y Justificación
Para recopilar la base de datos se ocupó  como fuente Transfermarkt, sitio web alemán que opera desde el año 2000 y recopila puntuaciones, resultados, noticias de transferencias, calendarios de liga, y valores de jugadores, datos que son indispensables para nuestra investigación.

Para extraer los datos de la página se hizo web scraping. Programé un bot en python y las librerias Request y BeautifulSoup. Primero se identificaron automáticamente los equipos participantes en cada temporada desde la página oficial de la liga, posteriormente, se accedió al historial de técnicos de cada equipo único. Finalmente se cruzaron las fechas de inicio y fin de cada técnico con el rango de cada temporada (1 de enero al 31 de diciembre) para determinar qué técnicos estuvieron activos en cada año. 
Los datos fueron exportados a Excel usando la librería pandas.

La herramientas utilizadas fueron Visual Studio Code, Claude para ayudar a programar y corregir errores y excel para visualizar los datos.

El rango de teimpo (2018-2025) se eligió por una razón en específico. Ese periodo nos permite comparar solo temporadas de torneo largo. Antes del 2018, las temporadas consistían de dos torneos cortos (apertura y clausura), por lo que no se pueden comparar. El 2018 al cambiarse el formato del torneo, fue el primer año que se entregó otro tipo de premio económico al campeón ya que ahora era solo uno anual. Debido a esto, partiremos desde el 2019 porque es el primer premio que se entregó tras un campeonato anual.

## Proceso de Limpieza de Datos
La base de datos en general no tenía información que no sirviera para la investigación, sin embargo, el archivo consideraba datos de la actual temporada 2026, los cuales se eliminaron de la base.

## Preguntas a responder
¿Existe una correlación entre los equipos más exitosos y los que tienen más estabilidad técnica?

¿Se puede relacionar la rotación de directores técnicos y el porcentaje de puntos obtenidos al finalizar la temporada?

¿Realmente los equipos mejoran su rendimiento al cambiar de técnico a mitad de temporada?
