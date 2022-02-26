# Medio ambiente

Hay varios notebook de Python en los que representamos y analizamos diferentes datos relacionados con el medio ambiente.

Notebooks:

<ul>
	<li> <b>Temp_Paises.ipynb</b>: Se utiliza una base de datos que contiene información de la temperatura promedio medida a lo largo del tiempo en diferentes países y continentes. En este caso únicamente vamos a usar las medidas obtenidas para cada uno de los continentes (África, Europa, Asia, Norte América, Sud América y Oceanía).<br><br>
* Base de datos obtenida de Kaggle (https://www.kaggle.com/sachinsarkar/climate-change-global-temperature-data)<br><br>
Qué es lo que se muestra:
	<ul>
		<li>Estadística de los datos:</li>
			<ul>
			<li>Resumen estadístico de los datos: Media, desviación estándar, valor máxima/mínima y cuartiles.</li>
			<li>Los histogramas de la temperatura promedio de cada continente y su error.</li>
			</ul>
		<li>Distribución de los datos por meses:</li>
		<ul>
			<li>Boxplot de la temperatura medida cada mes (variable categórica) en cada uno de los continentes. Además añadimos cada una de las medidas de la temperatura como scatterplot. Se representan en un color diferentes los datos de los últimos 11 años para ver si se salen de la estadística.</li>
			<li>Distribución (KDE) de la temperatura medida cada mes en los diferentes continentes.</li>
		</ul>
		<li>Representación de los datos:</li>
		<ul>
			<li>Representación de las temperaturas medidas mensualmente para cada continente justo la temperatura máxima, mínima y promedio calculados para cada año de cada continente.</li>
			<li>Representación de la temperatura mínima, máxima y promedio por año en cada continente. </li>
		</ul>
		<li>Estudio de la estacionaridad:</li>
		<ul>
			<li>Representación de los datos junto con las estadísticas móviles (promedio y desviación estándar). Para ver visualmente sí son constantes con el tiempo.</li>
			<li>Test de Dickey-Fuller. Para ver con que nivel de confianza podemos rechazar la hipótesis nula.</li>
		</ul>
	</ul>
	</li>
	<br><br>
	<li> <b>Greenhouse_Gases.ipynb</b>: Usamos varias bases de datos obtenidas de NOAA con medidas globales de los gases de efecto invernadero a lo largo del tiempo (hay datos anuales y mensuales). <br>
	* Referencia de los datos: Dr. Pieter Tans, NOAA/GML (gml.noaa.gov/ccgg/trends/) and Dr. Ralph Keeling, Scripps Institution of Oceanography (scrippsco2.ucsd.edu/) -> (https://gml.noaa.gov/ccgg/trends/)
	<br> <br>
Gases de los que tenemos datos:
	<ul>
	 	<li>CO2: Tenemos datos desde 01/01/1980 hasta 01/10/2021</li>
	 	<li>N2O: Tenemos datos desde 01/01/2001 hasta 01/09/2021)</li>
	 	<li>CH4: Tenemos datos desde 01/07/1983 hasta 01/09/2021)</li>
	 	<li>SF6: Tenemos datos desde 01/07/1997 hasta 01/09/2021)</li>
	</ul>
Qué es lo que se muestra:
	<ul>
		<li>Información estadística:</li>
		<ul> 
			<li>Resumen estadístico de los datos: Media, desviación estándar, valor máxima/mínima y cuartiles de los datos anuales y mensuales</li>
			<li>Los histogramas de los datos mensuales de cada gas</li>
		</ul>
		<li>Representación de los datos:</li>
		<ul>
			<li>Representación lineal de los datos medidos anualmente y mensualmente.</li>
		</ul>
		<li>Distribución de los datos:</li>
		<ul>
			<li>Boxplot de los datos mensuales para cada gas junto con los datos medidos en forma de scatter.</li>
			<li>Distribución KDE de los gases medidos mensualmente para cada año.</li>
		</ul>
		<li>Estudio de la estacionaridad:</li>
		<ul>
			<li>Representación de los datos junto con las estadísticas móviles (promedio y desviación estándar). Para ver visualmente sí son constantes con el tiempo.</li>
			<li>Test de Dickey-Fuller. Para ver con que nivel de confianza podemos rechazar la hipótesis nula.</li>
		</ul>
		<li>Forecasting usando el modelo ARIMA:</li>
		<ul>
			<li>Separamos la serie temporal en dos partes, unos que utilizaremos para el entrenamiento del modelo (train) y otro que utilizaremos para testear el modelo (test).</li>
			<li>Conversión de los datos usando una transformación logarítmica y el método de differencing. Tras la conversión de los datos volvemos a aplicar el estudio de estacionaridad para ver si los datos ya son estacionarios.</li>
			<li>Usamos la función de autocorrelación (ACF) y la función de autocorrelación parcial (PACF) para determinar los mejores parámetros "p, d y q" para el modelo ARIMA. El parámetro "d" es el valor del shift usado para el differencing, por lo tanto para determinar cual es el mejor usamos también el test de Dickey-Fuller. </li>
			<li>Aplicamos el modelo ARIMA con los parámetros que acabamos de determinar</li>
			<li>Representamos los residuos y la distribución kde de los residuos para ver la calidad de los modelos</li>
			<li>Utilizamos los datos test para testar la calidad de los datos</li>
			<li>Sobre los datos predichos por el modelo, invertimos la transformación que habíamos hecho para convertir los datos en estacionarios. Para invertir el differing de los datos logarítmicos, lo primero que hacemos es determinar la suma acumulada en el índice y luego agregarle el número base.</li>			
		</ul>
	</ul> 
	</li>
	<br><br>
	<li><b>Temp_Global.ipynb</b>: Usamos una base de datos que contiene datos globales de la temperatura de la Tierra a lo largo de tiempo.  Información: temperatura promedio de la superficie, temperatura máxima de la superficie, temperatura mínima de la superficie y temperatura promedio de la superficie y el océano. <br>
* Base de datos obtenida de Kaggle (https://www.kaggle.com/sachinsarkar/climate-change-global-temperature-data)<br><br>
Qué es lo que se muestra:
	<ul>
		<li>Estadística de los datos</li>
		<li>Los histogramas</li>
	</ul>
	</li>
</ul>