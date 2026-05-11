# Documentación de Entrega Individual - Patricio Gómez

## 1. Proceso de visualización: Pasos y decisiones
El proceso de construcción de esta visualización se centró en la optimización de los datos para su correcta interpretación gráfica. Las etapas principales fueron:

* **Limpieza de datos:** Se realizó una limpieza profunda del archivo Excel original. La decisión técnica más importante fue eliminar las unidades de texto (como "millones de euros" o "mil euros") para dejar únicamente los valores numéricos. Esto es fundamental para que el software de visualización pueda realizar cálculos y escalas correctamente.
* **Ordenamiento:** Se estructuró la información de manera cronológica y por categorías para asegurar que la visualización sea fluida.

## 2. Base de datos (CSV)
* **Selección:** Se optó por utilizar la base de datos con la que se venía trabajando previamente en el proyecto de equipo, garantizando así la coherencia con el resto del trabajo.
* **Procesamiento:** La base fue filtrada y "limpiada" de caracteres no numéricos en las columnas de valor, transformándola de un formato de lectura humana a un formato de procesamiento de datos (CSV listo para graficar).

## 3. Preguntas que responde esta visualización
Esta visualización permite resolver las siguientes interrogantes:

* **Variación de mercado:** ¿Cómo ha ido variando el precio de los equipos a lo largo de las temporadas?
* **Análisis comparativo:** Permite establecer una relación directa con las bases de datos de mis compañeros.
* **Cruce de datos e hipótesis:** Al integrar esta información con los otros sets de datos del equipo, es posible responder hipótesis más complejas mediante el cruce de variables (por ejemplo, relación entre precio y rendimiento deportivo). Además, permite calcular el valor total del plantel por temporada sumando los valores individuales.

## 4. Ficha técnica de la base de datos
* **Variables incorporadas:**
    * `Temporada`: Año o periodo de la competición.
    * `Equipo`: Club al que pertenece el jugador.
    * `Jugador`: Nombre del deportista.
    * `Posición`: Rol táctico en el campo.
    * `Edad`: Edad del jugador en dicha temporada.
    * `Nacionalidad`: País de origen del jugador.
    * `Valor de mercado`: Precio estimado del jugador por año (dato numérico limpio).
* **Observaciones:** El conjunto de estas variables permite realizar un análisis granular, pasando desde el valor individual del jugador hasta el valor agregado del plantel completo por cada ciclo anual.
