# Datos Caso 3 

Los datos a utilizar en el caso 3 se entregan en el formato de datos común en información de sensores remotos, imágenes y SIG. El formato *TIFF* o *GeoTIFF* es una de las múltiples alternativas para almacenar datos del tipo raster. Al hablar de raster se usa una retícula o matriz de elementos en donde cada elemento almacena información (valor numérico) de un área específica del territorio (resolución espacial) la conjunción de estos dos conceptos definen el elemento pictórico contraído en ingles como *Pixel*. Pese a q estas imágenes pueden verse en múltiples programas de imágenes, tienen una particularidad al almacenar los datos de coordenadas de su ubicación sobre la superficie terrestre, la cual le permite a los programas de SIG sobreponerlos sobre la información vectorial o en general sobre la superficie de referencia de la aplicaciones y herramientas SIG.

Las imágenes usadas en este caso provienen del programa satelital de la agencia espacial Europea [Sentinel](https://sentinel.esa.int/web/sentinel/home) y son apenas una selección dentro de los productos de información satelital que ofrece esta misión.

## Vista del municipio de Culla en la Comunidad Valenciana del 27 de diciembre de 2017 (Antes del incendio)

La vista esta compuesta por tres archivos con diferentes mediciones características. El primer archivo ([antes_colorverdadero_20171227.tif](antes_colorverdadero_20171227.tif) es una composición en color verdadero, es decir, una composición de colores similares a las que detecta el ojo humano. El segundo archivo ([antes_rojo_20171227.tif](antes_rojo_20171227.tif) corresponde a una sección correspondiente al color rojo, es decir, la medición de energia en el color rojo detectada por el ojo humano. Finalmente, el tercer archivo ([antes_infrarojo_20171227.tif](antes_infrarojo_20171227.tif) corresponde a una sección correspodiente al infrarojo cercano, esta es la muestra de cómo los sensores remotos complementan la visión humana mediante mediciones de energia que no puede ser dectectada por el ojo humano.

## Vista del municipio de Culla en la Comunidad Valenciana del 15 de enero de 2018 (Despues del incendio)

La vista esta compuesta por tres archivos con diferentes mediciones características. El primer archivo ([antes_colorverdadero_20180116.tif](antes_colorverdadero_20180116.tif) es una composición en color verdadero, es decir, una composición de colores similares a las que detecta el ojo humano. El segundo archivo ([antes_rojo_20180116.tif](antes_rojo_20180116.tif) corresponde a una sección correspondiente al color rojo, es decir, la medición de energia en el color rojo detectada por el ojo humano. Finalmente, el tercer archivo ([antes_infrarojo_20180116.tif](antes_infrarojo_20180116.tif) corresponde a una sección correspodiente al infrarojo cercano, esta es la muestra de cómo los sensores remotos complementan la visión humana mediante mediciones de energia que no puede ser dectectada por el ojo humano.

## Índice de diferencia normalizada de vegetación (NDVI)

El índice es un método que usa la aritmética entre mediciones de energia entre el color rojo y el infrarojo para identificar las características de la vegetación de acuerdo a su vigorosidad. El primer archivo ([antes_ndvi_20171227.tif](antes_ndvi_20171227.tif) es el resultado de estimar el índice vegetación de diferencia normalizada. Para mejorar la visibilidad e interpretación se debe usar la simbología en el  estilo ajustado para [NDVI](simbologia_ndvi.qml).

## Simbología

Las aplicaciones SIG permiten generar archivos de simbología para facilitar la visualización de datos. Los archios de simbología permiten por un lado ver la representación del índice de vegetación usando una combinación artificial de colores conocida normalmente como falso color, Archivo [simbologia_ndvi.qml](simbologia_ndvi.qml). Por otro lado permiten ver las diferencias entre índices de vegetación de forma más clara que con la escala de grises por defecto [simbologia_diferencia_ndvi.qml](simbologia_diferencia_ndvi.qml).

## Inventario de incendios forestales de la Comunidad Valenciana (1993-2015)

El Archivo [Incendios_forestales_1993_2015.zip](Incendios_forestales_1993_2015.zip) contiene la información cartográfica de los incendios forestales reportados en la Cumunidad Valenciana entre los años 1993 y 2015. El archivo contiene capas con representaciones en puntos y polígonos.
