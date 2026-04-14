# 3. Ficha técnica y diccionario de datos

## Fuente de los datos

La información utilizada en la construcción de la base de datos fue obtenida desde el sitio web Transfermarkt, plataforma especializada en estadísticas y valores de mercado de jugadores y equipos de fútbol a nivel internacional.

## Metodología de construcción de la base

La base de datos fue construida a partir de la recopilación manual de información disponible en Transfermarkt para los planteles de la Primera División del fútbol chileno entre las temporadas 2019 y 2026.

Posteriormente, se realizó un proceso de limpieza y tratamiento de los datos que incluyó:
- Corrección de la variable temporal, ajustando un desfase detectado en los años de registro.
- Eliminación de registros duplicados.
- Estandarización de nombres de equipos y jugadores para asegurar consistencia en el análisis.
- Exclusión de jugadores sin participación en la temporada (sin minutaje registrado), con el fin de considerar únicamente aquellos futbolistas con incidencia deportiva real en los planteles.

## Alcance de los datos

La base de datos presenta el siguiente alcance:
- **Temporal:** comprende las temporadas desde 2019 hasta 2026.
- **Geográfico:** se limita a equipos pertenecientes a la Primera División del fútbol chileno.
- **Unidad de análisis:** jugadores registrados en los planteles de cada equipo por temporada.

## Características de los datos

La base está compuesta por datos de carácter individual (nivel jugador), e incluye tanto variables cuantitativas como categóricas:
- **Variables cuantitativas:** edad y valor de mercado.
- **Variables categóricas:** equipo, nacionalidad, posición y temporada.
Los datos permiten realizar análisis comparativos entre equipos y temporadas en función de características deportivas y económicas.

## Otras observaciones
- El valor de mercado de los jugadores corresponde a estimaciones realizadas por Transfermarkt, por lo que no necesariamente refleja montos reales de transferencias.
- Se identificó inicialmente un desfase en la variable de temporada, el cual fue corregido durante el proceso de limpieza.
- La exclusión de jugadores sin minutaje puede generar una leve subrepresentación de futbolistas juveniles o de baja participación, aunque permite enfocar el análisis en jugadores con impacto efectivo en el rendimiento deportivo.

## Diccionario de datos

- **temporada:** corresponde al año de la temporada en la que se registra el jugador. Es una variable de tipo numérico y toma valores entre 2019 y 2026. Este dato fue corregido debido a un desfase en la base original.
- **equipo:** indica el club al que pertenece el jugador en la temporada correspondiente. Es una variable categórica que incluye a los equipos de la Primera División del fútbol chileno. Los nombres fueron estandarizados durante el proceso de limpieza.
- **jugador:** nombre completo del futbolista registrado en la base de datos. Es una variable de tipo texto.
- **posición:** corresponde a la posición en la que juega el futbolista dentro del campo. Es una variable categórica que puede incluir valores como defensa, mediocampista, delantero, entre otros.
- **edad:** edad del jugador durante la temporada correspondiente. Es una variable numérica, generalmente en un rango aproximado entre 15 y 40 años.
- **nacionalidad:** país de origen del jugador. Es una variable categórica que incluye distintas nacionalidades, como Chile, Argentina, Brasil, entre otras.
- **valor_mercado:** valor estimado del jugador en el mercado de transferencias. Es una variable numérica con valores iguales o superiores a 0. Este dato corresponde a una estimación y no necesariamente refleja el valor real de una transferencia.
