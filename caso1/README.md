# Caso 1 

Interactuar desde el primer minuto con la herramienta QGIS para crear mapas, y al mismo tiempo, incluir breves explicaciones teóricas sobre alguno de los conceptos que aparecen durante la realización de los casos prácticos, como la escala, leyenda, *features*, *layer*, etc.

## Interfaz de usuario de QGIS
Barra de menus, panel izquierda (fuentes de datos y capas), panel derecho (previsualización mapas)
Concepto: Capa o *layer*

## Pasos generales para generar un mapa. 
* **La historia**: ¿qué pregunta o perspectiva quiero contestar o illustrar con un mapa?.
* **Los datos**: ¿qué datos necesito? ¿Dónde encontrarlos?
* **El mapa (en digital)**: ¿Cómo transformo los datos en un mapa?
* **El mapa (en papel)**: ¿Cómo genero un mapa apto para imprimir?
* **El proyecto**: Por si acaso, ¿cómo guardo el mapa para futuros usos? 

### [La historia]: Mapamundi político con color uniforme.
* **Los datos**: [Límites administratimos de países, escala 1:50m (1cm = 500km)](https://www.naturalearthdata.com/http//www.naturalearthdata.com/download/50m/cultural/ne_50m_admin_0_countries.zip) 
* **El mapa (en digital)**: 
  * Localizar los datos en QGIS
  * Visualizar una capa en QGIS
* **El mapa (en papel)**: 
  * Crear un mapa (con leyenda, escala, titulo, anotaciones, etc) en formato PDF
* **El proyecto**:  
  * Salva en un fichero (QGIS) el mapa y los datos asociados. 

### [La historia]: Mapamundi político (coloreado) por continentes/países/etc.

Conceptos: 
* ¿Por qué los datos *espaciales* son *especiales*? => Tabla de atributos. 
* ¿Colorear (*categorizar*) por continente? => Categorizar datos por atributo alfanumérico/categóricos (texto)

### [La historia]: Mapamundi político según el PIB por país.

Conceptos: 
* ¿Colorear (*clasificar*) según su PIB por país? => Clasificar datos por atributo numérico
* Mostrar solo los países del grupo de mayor PIB => *Clases* de la *capa* 
* Duplicar *capas* => El orden de las *capas* importa. 

### [La historia]: Mapamundi político según la población por país.

### [La historia]: Mapamundi político según el PIB per cápita por país.

Conceptos: 
* ¿Cuales son los países ricos y cuales los pobres? Necesito el PIB per cápita => Crear nuevos atributos (expresiones) en base a otros ya existentes.  


### [La historia]: Mapamundi político de países en vías de desarrollo con población mayor de 10 millones.

Conceptos: 
* ¿Mostrar (*filtrar*) solo los países con cierta población? => Filtrar datos mediante expresiones que operan/combinan atributos
* ¿Mostrar el nombre del país? => Etiquetas asociadas a atributos


## Break

## Ejemplo a escala nacional y Comunidad Valenciana

## Servicios y visores disponibles 
