# ElectroThings_MongoDB
* Base de Datos acerca de componentes electrónicos generales desarrollado con MongoDB
* Solamente se aplica una Collección, la db es completamente escalable según el propósito del Proyecto que se llevo a cabo.
* Recomiendo generar un .csv y un .json por collection para modularizar y versionar la db

</br>

#### Tabla Colección  `productos`

![Index app](https://github.com/andresWeitzel/db_microelectronica_Oracle/blob/master/doc/db_microelectronica_DER.png)





<hr>

## Más Información

</br>


| **Tecnologías Empleadas** | **Versión** | **Finalidad** |               
| ------------- | ------------- | ------------- |
| MongoDB | 5.0  | DB  |
| MongoDB Compass | 1.31.2  | Gestor de MongoDB | 
| Git Bash | 2.29.1  | Control de Versiones |
| CMD | 10 | Manipular los Servicios de Postgres mediante linea de comandos | 

</br>


## Descarga y Documentacion de las Tecnologías Empleadas:

</br>

| **Tecnologías** | **Descarga** | **Documentación** |               
| ------------- | ------------- | ------------- |
| Git Bash |  https://git-scm.com/downloads |   https://git-scm.com/docs |
| MongoDB |  https://www.mongodb.com/try/download/community  | https://www.mongodb.com/try/download/community |
| MongoDB Compass | https://www.mongodb.com/try/download/compass  | https://www.mongodb.com/try/download/compass | 

</br>

## Bibliografía Oficial Recomendada
* doc oficial : https://www.mongodb.com/docs/manual/tutorial/getting-started/




<hr>

## Creación de Documentos/Base de Datos y Colección

* Podemos usar MongoSHELL, pero es poco eficiente y legible la inseción de datos por shell, usaremos Compass (https://www.mongodb.com/products/compass) como interfaz gráfica y editor
* Ademas vamos a crear nuestra db en formato csv para agilizar tiempo y repetición de palabras. Agregamos 10 registros

### Pasos mongo

#### Creamos nuestra db
* Database Name : db_electro_things
* Collection Name : productos

#### Agregamos registros desde archivo CSV
* Seleccionamos nuestra db, seleccionamos la colección productos
* ADD DATA
* import file
* select file
* linkeas el doc csv de este repo
* import
* Si aparecen los registros se ha importado correctamente
</br>

####  Colección  `productos.csv`

![Index app](https://github.com/andresWeitzel/db_microelectronica_Oracle/blob/master/doc/db_microelectronica_DER.png)
 

#### Agregamos registros desde archivo Json
* En mi caso use un convertidor de documentos online, pase el archivo CSV a JSON. 

####  Colección  `productos.json`

![Index app](https://github.com/andresWeitzel/db_microelectronica_Oracle/blob/master/doc/db_microelectronica_DER.png)
 
