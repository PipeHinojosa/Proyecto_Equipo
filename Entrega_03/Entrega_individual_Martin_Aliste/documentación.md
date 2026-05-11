# Documentación

Al momento de visualizar los datos, la prioridad era que estos sean fáciles de entender. En un principio pensé en ocupar un gráfico de dispersión, pero la información no quedaba clara a simple vista. Debido a eso, preferí utilizar un gráfico de barras y agrupar los datos para hacer más fácil su interpretación.

Se separaron los datos en tres grupos: los equipos que no cambiaron de técnico durante la temporada, los que lo hicieron 1 o 2 veces, y los que lo hicieron más de tres. De esta forma se elimina el ruido visual de tener todos los datos dispersos en el gráfico, permitiendo comparar temporada tras temporada la diferencia en el promedio de la posición final entre los equipos más estables y menos estables.

Después de abrir la base de datos en Google Colab e instalar las librerías de Altair, le pedí ayuda a Claude AI para generar un script en base a mis indicaciones para visualizar los datos.

Utilicé la base de datos de los cambios de técnicos por temporada. Lo que hice fue separar en columnas distintas a los DTs de los equipos y agregar la base de datos de las posiciones finales de los equipos para poder cruzar los datos.

## Las preguntas que la visualización puede responder son las siguientes:

¿Existe una correlación entre los equipos más exitosos y los que tienen más estabilidad técnica?

¿Se puede relacionar la rotación de directores técnicos y el porcentaje de puntos obtenidos al finalizar la temporada?

