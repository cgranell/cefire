# Datos Caso 1 

Los datos a utilizar en el caso 1 se entregan en dos formatos de datos comunes en SIG:
* el formato *shapefile* de ESRI que ha sido por muchos años el formato de intercambio de datos vectoriales en SIG y,
* el formato *GeoJSON* que es un alternativa que almacena los datos en formato de texto para facilitar su intercambio a través de la Web. 

Cualquiera de los dos formatos permiten adelantar las actividades del curso y su uso en otras aplicaciones SIG.

## Límites Administrativos de países, escala 1:50m (1cm = 500km)

El archivo [Limites_administrativos.zip](Limites_administrativos.zip) contiene las geometrías del tipo polígono con los límites administrativos de los países junto a una serie de atributos que los describen. El archivo es una versión simplificada de la fuente original [Límites administratimos de países, escala 1:50m (1cm = 500km)](https://www.naturalearthdata.com/http//www.naturalearthdata.com/download/50m/cultural/ne_50m_admin_0_countries.zip) 

A continuación se presenta una corta descripción de los atributos de interés para las prácticas en el curso.

* **TYPE**: Tipo de territorio de acuerdo con su estado legal a nivel internacional (País, territorio dependiente, territorio en disputa o indeterminado).
* **ABREV**: Nombre abreviado del estado que ejerce soberanía en el territorio.
* **NAME_LONG**: Nombre del estado que ejerce soberanía en el territorio.
* **POSTAL**: Nombre abreviado del estado como código postal.
* **POP_EST**: Población estimada, número de habitantes.
* **GDP_MD_EST**: Producto interno bruto medido en miles de millones de Dólares.
* **ECONOMY**: Clasificación del país de acuerdo a su nivel de desarrollo económico.
* **INCOME_GRP**: Clasificación del país de acuerdo a su nivel de ingresos.
* **CONTINENT**: Nombre del continente en el que se encuentra el país.
* **REGION_UN**: Nobre de la región en el que se encuentra el país de acuerdo a la clasificación de las Naciones Unidas.
* **SUBREGION**: Nobre de la subregión en el que se encuentra el país de acuerdo a la clasificación de las Naciones Unidas.
