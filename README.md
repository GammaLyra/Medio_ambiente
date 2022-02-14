# Medio_ambiente

Hay varios notebook de Python en los que representamos y analizamos diferentes datos relacionados con el medio ambiente.

Notebooks:

<ul>
	<li> <b>Greenhouse_Gases.ipynb</b>: Usamos varias bases de datos obtenidas de NOAA con medidas globales de los gases de efecto invernadero a lo largo del tiempo (hay datos anuales y mensuales). <br>
	* Referencia de los datos: Dr. Pieter Tans, NOAA/GML (gml.noaa.gov/ccgg/trends/) and Dr. Ralph Keeling, Scripps Institution of Oceanography (scrippsco2.ucsd.edu/)<br>  <br>
Gases de los que tenemos datos:
	<ul>
	 	<li>CO2: Tenemos datos desde 01/01/1980 hasta 01/10/2021</li>
	 	<li>N2O: Tenemos datos desde 01/01/2001 hasta 01/09/2021)</li>
	 	<li>CH4: Tenemos datos desde 01/07/1983 hasta 01/09/2021)</li>
	 	<li>SF6: Tenemos datos desde 01/07/1997 hasta 01/09/2021)</li>
	</ul>
Qué es lo que se muestra:
	<ul>
		<li>Estadística de los datos anuales y mensuales</li>
		<li>Los histogramas de los datos mensuales de cada gas</li>
	</ul> 
	</li>
	<li> <b>Temp_Paises.ipynb</b>: Se utiliza una base de datos que contiene información de la temperatura promedio medida a lo largo del tiempo en diferentes países y continentes. En este caso únicamente vamos a usar las medidas obtenidas para cada uno de los continentes (África, Europa, Asia, Norte América, Sud América y Oceanía).<br>
* Base de datos obtenida de Kaggle (https://www.kaggle.com/sachinsarkar/climate-change-global-temperature-data)<br><br>
Qué es lo que se muestra:
	<ul>
		<li>Estadística de los datos</li>
		<li>Los histogramas de la temperatura promedio de cada continente y su error.</li>
		<li>Boxplot de la temperatura medida cada mes (variable categórica) en cada uno de los continentes. Además añadimos cada una de las medidas de la temperatura como scatterplot. Se representan en un color diferentes los datos de los últimos 11 años para ver si se salen de la estadística.</li>
		<li>Distribución (KDE) de la temperatura medida cada mes en los diferentes continentes.</li>
		<li>Representación de la temperatura mínima, máxima y promedio por año en cada continente. Variables calculadas por nosotros</li>
		<li>Representación de las temperaturas medidas mensualmente para cada continente justo con el promedio móvil de la temperatura máxima, mínima y promedio. Usamos el promedio móvil para ver la tendencia a lo largo del tiempo.</li>
	</ul>
	</li>
	<li><b>Temp_Global.ipynb</b>: Usamos una base de datos que contiene datos globales de la temperatura de la Tierra a lo largo de tiempo.  Información: temperatura promedio de la superficie, temperatura máxima de la superficie, temperatura mínima de la superficie y temperatura promedio de la superficie y el océano. <br>
* Base de datos obtenida de Kaggle (https://www.kaggle.com/sachinsarkar/climate-change-global-temperature-data)<br><br>
Qué es lo que se muestra:
	<ul>
		<li>Estadística de los datos</li>
		<li>Los histogramas</li>
	</ul>
	</li>
</ul>