# Caso 2 

## Recuerda: Pasos generales para generar un mapa. 
* **La historia**: ¿qué pregunta o perspectiva quiero contestar o illustrar con un mapa?.
* **Los datos**: ¿qué datos necesito? ¿Dónde encontrarlos?
* **El mapa (en digital)**: ¿Cómo transformo los datos en un mapa?
* **El mapa (en papel)**: ¿Cómo genero un mapa apto para imprimir?
* **El proyecto**: Por si acaso, ¿cómo guardo el mapa para futuros usos? 


### [La historia]: ¿Qué partes/regiones de España concentran la mayor población? ¿Qué municipios son los más poblados? ¿Cuáles los menos poblados? 

* **Los datos**: [Población y desempleo por municipio en España 2017](Datos/README.md)

### [La historia]: ¿Qué regiones y municipios forman la ["España Vacía"](https://elpais.com/cultura/2016/04/19/babelia/1461071676_157409.html)? ¿

* **Los datos**: [Población y desempleo por municipio en España 2017](Datos/README.md)

### [La historia]: Al hilo del artículo en El País sobre ["Las pequeñas ciudades se despueblan: La ciudad mermada que soñó con llegar a 300.000 habitantes"](https://elpais.com/sociedad/2019/02/05/actualidad/1549335210_628003.html), ¿Qué municipios ganan y cuales pierden población?

* **Los datos**: [Población y desempleo por municipio en España 2017](Datos/README.md) y [Población por municipio, padrón municipal 2018](Datos/README.md)

Conceptos:
* ¿los datos de población de 2018 y 2017 están separados? => *joins* o uniones.

### [La historia]: ¿Cómo se distribuye la densidad de población en España? ¿Qué Comunidades/municipios tienen mayor densidad? ¿Cuáles las que menos? 

Conceptos:
* ¿Cómo comparar el número de habitantes entre municipios grandes y pequeños? => La densidad de población usa una unidad de área que permita hacer la comparación, esta puede ser kilómetros cuadrados o hectareas.
	* Densidad por Kilómetro Cuadrado = (Población) / (Área en Kilómetros cuadrados)
* ¿Cómo convertir los valores de área entre metros cuadrados y kilómetros cuadrados? => Para convertir las áreas calculadas por el SIG en metros cuadrados se debe dividir el valor en 1.000.000.
	* 1 Kilómetro cuadrado = 1.000.000 metros cuadrados = 1.000 m x 1.000 m.

## Break

### [La historia]: ¿Cómo se distribuye la población por género, por ejemplo, en que municipios son mayoría las mujeres y en cuales los hombres?

Conceptos:

* ¿Cómo sintetizar la proporción de hombres y mujeres? => se puede hacer una proporcion entre estos dos valores para saber la proporción de hombres por cada mujer.
	* La división o ratio (cantidad de mujeres) / (cantidad de hombres) puede ser interpretada como: Existen *X* cantidad de hombres por cada mujer.
	* Para reducir el número de decimales en una operación se puede usar la función *round* round (valor, decimales).

### [La historia]: ¿Qué municipios tienen mayor desempleo? ¿Existe relación entre la tasa de paro y la densidad de población?

* ¿Cómo encontrar un estimado de la tasa de empleo? => los datos con los que contamos no nos permiten hacer el cálculo preciso de la tasa de desempleo o de paro, para esto sería necesario contar con los datos de la población económicamente activa, en capacidad de trabajar o su equivalente. El cálculo realizado es indicativo y con fines académicos.

### [La historia]: ¿Cuanta población vive en la franja de la costa (a menos de 50km) y cuanta en el interior? ¿Cuánta población habría que evacuar ante una eventual crecida de los oceános? ¿Cuanta población debería ser más sensible al "mar de plástico"?

Conceptos:
* ¿Cómo identificar los objetos que estan dentro de un rango de distancia? => El proceso en el SIG está compuesto por una función de área de influencia y una opcional de intersección. Primero se usa el área de influencia para dibujar una extensión de un objeto haciendo uso de la distancia.
	* Función buffer (objeto, distancia): esta función toma cada uno de los objetos y genera el área de influencia a partir de la distancia indicada.
	* Opción de disolver, se usa cuando se quiere obtener una única área a partir de las áreas que se sobreponen entre sí luego de calcular el área de influencia, esta opción es conveniente y necesaria en este caso.

