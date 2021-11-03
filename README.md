# php-api-rest-heroku
Ejemplo api rest heroku usando php

###### DESPLIEGUE EN HEROKU

- index.php (código fuente de la api-restful, se aloja en la carpeta public)
- composer.json (permitirá descargar las dependencias necesarias)
- composer.lock

- Procfile (despliega un servidor apache apuntando a la carpeta public donde se encuentra el archivo index.php

> web: vendor/bin/heroku-php-apache2 /public
