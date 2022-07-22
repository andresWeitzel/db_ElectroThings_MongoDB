# ElectroThings_MongoDB
* Base de Datos acerca de componentes electrónicos generales desarrollado con MongoDB
* La db consta de Cuatro Colecciones, una de Productos Electrónicos y el resto acerca de Usuarios con su autenticación (Usuarios, Roles, Usuarios-Roles).
* Esta Arquitectura es completamente escalable según el propósito del Proyecto que se lleve a cabo. El enfoque es la Modularización de Colecciones por archivos.
* Se generó un .csv y un .json por cada Coleccion, además de la doc gráfica.

</br>

#### Colecciones de la base de datos

![Index app](https://github.com/andresWeitzel/db_ElectroThings_MongoDB/blob/master/doc/collections.png)


#### Colección  `productos`

![Index app](https://github.com/andresWeitzel/db_ElectroThings_MongoDB/blob/master/doc/collection_productos/collection.table.png)


#### Colección  `usuarios`

![Index app](https://github.com/andresWeitzel/db_ElectroThings_MongoDB/blob/master/doc/usuarios.png)


#### Colección  `roles`

![Index app](https://github.com/andresWeitzel/db_ElectroThings_MongoDB/blob/master/doc/roles.png)


#### Colección  `usuarios_roles`

![Index app](https://github.com/andresWeitzel/db_ElectroThings_MongoDB/blob/master/doc/usuarios_roles.png)





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

## Bibliografía Oficial y No Oficial Recomendada
* Doc oficial : https://www.mongodb.com/docs/manual/tutorial/getting-started/
* Convertidor de texto plano a texto cifrado(Bcrypt) : https://www.browserling.com/tools/bcrypt
* Convertidor CSV a Json : https://www.convertcsv.com/csv-to-json.htm




<hr>

## Creación de Documentos/Base de Datos y Colección

* Podemos usar MongoSHELL, pero es poco eficiente y legible la inseción de datos por shell, usaremos Compass (https://www.mongodb.com/products/compass) como interfaz gráfica y editor
* Ademas vamos a crear nuestra db en formato csv para agilizar tiempo y repetición de campos. Agregamos 20 registros

### Pasos MongoDB

#### Creamos nuestra db
* Database Name : db_electro_things
* Collection Name : productos

#### Agregamos registros desde archivo CSV
* Seleccionamos nuestra db, seleccionamos la colección productos
* ADD DATA
* import file
* select file
* linkeas el doc csv desde el filesystem de este repo
* import
* Si aparecen los registros se ha importado correctamente
</br>

####  Colección ejemplar  `productos.csv`
![Index app](https://github.com/andresWeitzel/db_ElectroThings_MongoDB/blob/master/doc/collection_productos/collection.csv.png)



#### Agregamos registros desde archivo Json
* En mi caso use un convertidor de documentos online, pase el archivo CSV a JSON. 

####  Colección ejemplar  `productos.json`

![Index app](https://github.com/andresWeitzel/db_ElectroThings_MongoDB/blob/master/doc/collection_productos/collection.json.png)



</br>


##  Uso y Manejo de Git.

</br>

###  Descarga y Configuración de Git

####  Descarga de Git
* Nos dirigimos a https://git-scm.com/downloads y descargamos el versionador
* Como toda aplicacion siguiente.... siguiente....
* IMPORTANTE:NO TENER DBEAVER ABIERTO DURANTE LA INSTALACION, SINO NO RECONOCE EL PATH

####  Abrir una Consola de Git (Git Bash) desde Windows
* --> Escribimos Git Bash desde el Buscador de Windows
* --> Desde la consola escribimos el comando cd seguidamente de la ruta del proyecto
* --> Tenemos que tener la ruta del Proyecto y pegarla en el Git Bash
* --> Una vez dentro del Proyecto podremos hacer uso de Git

</br>

###  Subir el proyecto al repositorio de github desde la consola de git 

#### Creamos un nuevo repositorio en GitHub.

#### Inicializamos nuestro repositorio local .git desde la terminal.
* git init

#### Agregamos lo desarrollado a nuestro repo local desde la terminal.
* git add *

#### Agregamos lo que tenemos en nuestro repo local al área de Trabajo desde la terminal.
* git commit -m "agrega un comentario entre comillas"

#### Le indicamos a git donde se va a almacenar nuestro proyecto(fijate en tu repositorio de github cual es el enlace de tu proyecto(esta en code)).
* git remote add origin https://github.com/andresWeitzel/db_ElectroThings_MongoDB

#### Subimos nuestro proyecto.
* git push -u origin master


</br>


### Actualización del repositorio del proyecto desde la consola de GIT

#### Visualizamos las modificaciones realizadas en local
* git status

#### Agregamos lo modificado al área de trabajo
* git add *

#### Confirmamos las modificaciones realizadas
* git commit -m "tu commit entre comillas"

#### Sincronizamos y traemos todos los cambios del repositorio remoto a la rama en la que estemos trabajando actualmente.
##### (SOLO SI SE REALIZARON CAMBIOS DESDE OTRA LADO, ej: en github u/o/y un equipo de trabajo)
* git pull https://github.com/andresWeitzel/db_ElectroThings_MongoDB

#### Enviamos todos los cambios locales al repo en github
* git push https://github.com/andresWeitzel/db_ElectroThings_MongoDB

#### En casos extremos pisamos todo el repositorio
* git push -f --set-upstream origin master


</br>

