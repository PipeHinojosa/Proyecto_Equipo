# Documentación

Para recopilar la base de datos se ocupó  como fuente la página Transfermarkt, sitio alemán que recopila puntuaciones, resultados, noticias de transferencias, calendarios de liga, y valores de jugadores.
Para extraer los datos de la página se hizo web scraping. Programé un bot en python y las librerias Request y BeautifulSoup. Primero se identificaron automáticamente los equipos participantes en cada temporada desde la página oficial de la liga. Luego se accedió al historial de técnicos de cada equipo único. Finalmente se cruzaron las fechas de inicio y fin de cada técnico con el rango de cada temporada (1 de enero al 31 de diciembre) para determinar qué técnicos estuvieron activos en cada año. 
Los datos fueron exportados a Excel usando la librería pandas.

El rango de teimpo (2018-2025) se eligió por una razón en específico. Ese periodo nos permite comparar solo temporadas de torneo largo. Antes del 2018, las temporadas consistían de dos torneos cortos (apertura y clausura), por lo que no se pueden comparar.
Además, el rango nos permite observar un ciclo completo de gestión, desde el año 2018, el estallido social en 2019, la crisis sanitaria de 2020 y la reestructuración económica actual de la liga.
