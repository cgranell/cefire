# Caso 3 

## Recuerda: Pasos generales para generar un mapa. 
* **La historia**: ¿qué pregunta o perspectiva quiero contestar o illustrar con un mapa?.
* **Los datos**: ¿qué datos necesito? ¿Dónde encontrarlos?
* **El mapa (en digital)**: ¿Cómo transformo los datos en un mapa?
* **El mapa (en papel)**: ¿Cómo genero un mapa apto para imprimir?
* **El proyecto**: Por si acaso, ¿cómo guardo el mapa para futuros usos? 

### [La historia]: ¿Cómo identificar los efectos que produce un incendio forestal? ¿Cuáles son las tecnologías satelitales que pueden ayudar en la tarea? ¿Cómo era una zona antes de un incendio forestal? ¿Como ha quedado después? ¿Cuáles son los cambios más relevantes? ¿Es posible estimar el área afectada sin hacer una inspección de campo?

* **Los datos**: [Breve descripción y acceso a los datos](Datos/README.md)
* **La representación digital del terreno**: Las imágenes de satélite usan el mismo principio de la fotografía digital y este a su vez es su limitante. Estas imágenes permiten identificar objetos con un diámetro mayor a 10m, son óptimas para estudios de escalas municipales y provinciales.
* **Gestión de archivos**: Las imágenes de satélite contienen grandes cantidades de información y usualmente demandan grandes espacios de almacenamiento. Se pueden comparar los tamaños de los archivos trabajados hasta el momento, su cobertura y nivel de detalle para apreciar las diferencias.

### [La historia]: ¿Cuál es el papel de los sensores en observación satelital? ¿Qué información añaden los sensores de energía en el infrarojo cercano? ¿Cómo usar los colores para interpretar información que no percibe el ojo humano? ¿Cuáles algoritmos permiten manipular la información satelital? ¿Cuáles índices sintetizan las caracterísiticas de la vegetación? 

* [Fórmula de cálculo del índice de vegetación - NDVI](https://es.wikipedia.org/wiki/%C3%8Dndice_de_vegetaci%C3%B3n_de_diferencia_normalizada): Se calcula como la división de i) la diferencia entre los valores del infrarojo cercano y el rojo, entre ii) la suma de los valores del infrarojo cercano y el rojo). NDVI = (IRC - R)/(IRC + R).

* **Interpretación del NDVI**: El índice produce valores entre -1 y 1.
	* Valores cercanos a 1 indican una alta actividad clorofílica, es decir, vegetación vigorosa.
	* Valores cercanos a 0 o negativos indican baja actividad clorofílica usualmente asociada a suelo desnudo, rocas, ciudades, cuerpos de agua o rios.

* **Usando el falso color**: las composiciones de imágenes permiten ver la realidad con colores a los que no estamos acostumbrados para resaltar un fenómeno en particular, en este caso, la actividad clorofílica de la vegegación. (Usar el estilo ajustado para [NDVI](Datos/simbologia_ndvi.qml))
	* Rojo: para valores cercanos a 1 indican una alta actividad clorofílica, es decir, vegetación vigorosa.
	* Azul: para Valores cercanos a 0 o negativos indican baja actividad clorofílica usualmente asociada a suelo desnudo, rocas, ciudades, cuerpos de agua o rios.

## Break

### [La historia]: ¿De que forma se se identifican cambios en el tiempo a partir de índices? ¿Cómo usar colores para resaltar fenómenos particulares en el SIG? 
* **Comparando los índices de vegetación**: La resta aritmética de los índices (NDVI Despues - NDVI Antes) Permite ver los cambios en el índice a través del tiempo. (Usar el estilo ajustado para diferencias [NDVI](Datos/simbologia_diferencia_ndvi.qml))
	* Rojo: para valores negativos, son las zonas con descensos en el índice de vegetación y corresponden en su mayoría a áreas afectadas por el incendio forestal.
	* Amarillos: para valores cercanos a cero, son las zonas sin mayores cambios en el índice.
	* Verde: para valores positivos, son las zonas con aumentos en el índice de vegetación.


### [La historia]: ¿Qué otras opciones de visualización existen para este tipo de fenómenos que se distribuyen en el territorio? ¿Cómo usar la información histórica para extraer patrones de distribución espacial de fenómenos? 
* **Creación de mapas de calor**: La comparación de las ubicaciones relativas (objetos cercanos o agroupados) permite hacer estimaciones matemáticas de su concentración. Una herramienta indicativa de dicha concentración se conoce comunmente como *mapas de calor* (del ingés heatmap). *QGIS* ofrece una herramienta simplificada para generar este tipo de mapas en la sección de simbología, aplica únicamente a capas de tipo punto.
	* Tonalidades intensas: para concentraciones altas, son las zonas en donde existe mayor presencia de objetos (puntos).
	* Tonalidades claras: para concentraciones bajas, son las zonas en donde la presencia de objetos (puntos) es menor.
	* Transparencia: Los mapas de calor se usan en combinación con capas de fondo para facilitar la interpretación.
