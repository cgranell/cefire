# Datos Caso 2 

Los datos a utilizar en el caso 1 se entregan en dos formatos de datos comunes en SIG. Formato Shapefile de ESRI que ha sido por muchos años el formato de intercambio de datos vectoriales en SIG y Formato GeoJSON que es un alternativa que almacena los datos en formato de texto para facilitar su intercambio a través de la Web. Cualquiera de los dos formatos permiten adelantar las actividades del curso y su uso en otras aplicaciones SIG.

## Datos de población y desempleo por municipio en España 2017

Este archivo (Poblacion_paro_municipio.zip) contiene las geometrías del tipo polígono con los límites administrativos de los municipios de España junto a una serie de de población y desempleo. El archivo es una versión simplificada de la compilación de datos abiertos ofrecida por [Esri España](http://opendata.esri.es) 

A continuación se presenta una corta descripción de los atributos de interés para las prácticas en el curso.

* **Cod_CCAA**: Código de identificación de la comunidad autónoma.
* **cod_mpio**: Código de identificación del municipio.
* **nom_mpio**: Nombre del municipio.
* **Cod_Prov**: Código de la provincia en la que se ubica el municipio.
* **Cod_CCAA**: Código de la comunidad autónoma en la que se ubica el municipio.
* **total_paro**: Código de la provincia en la que se ubica el municipio.
* **poblacion**: Código de la provincia en la que se ubica el municipio.

## Límite de línea costera natural y artificial. Línea de pleamar y bajamar.

Este archivo (Linea_costera.zip) contiene las geometrías del tipo línea con los límites costeros de España clasificados de acuerdo a su origen y naturaleza. El archivo es una versión compilada e integrada de la cartografía báse del Instituto Geográfico Nacional disponibles en el [Centro Nacional de Información Geográfica](http://centrodedescargas.cnig.es/CentroDescargas)

A continuación se presenta la descripción de los atributos de interés para las prácticas en el curso.

* **CATEGORIA**: Descripción corta de las categorías de líneas costeras.

## Población por municipio, padrón municipal.

Este archivo (PoblacionMunicipal2018.csv) contiene los datos del padrón municipal de población España a corte del 01/01/2018. El archivo es una versión ajustada para la lectura en software SIG en formato de texto del [Instituto Nacional de estadística](https://www.ine.es/dyngs/INEbase/es/operacion.htm?c=Estadistica_C&cid=1254736177011&menu=resultados&idp=1254734710990)

A continuación se presenta la descripción de los atributos de interés para las prácticas en el curso.

* **CODIGO**: Código integrado del municipio que permite vincularlo con la capa de municipios.
* **POB18**: Población total del municipio a corte del 01/01/2018.
* **HOMBRES**: Población de hombres del municipio a corte del 01/01/2018.
* **MUJERES**: Población mujeres del municipio a corte del 01/01/2018.