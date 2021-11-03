# php-api-rest-heroku
Ejemplo api rest heroku usando php

###### DESPLIEGUE EN HEROKU
Necesitaremos 4 archivos

- index.php (código fuente de la api-restful, se aloja en la carpeta public)
- composer.json (permitirá descargar las dependencias necesarias)

- Procfile (despliega un servidor apache apuntando a la carpeta public donde se encuentra el archivo index.php

> web: vendor/bin/heroku-php-apache2 /public


- .htaccess.txt (redirecciona al archivo index.php)

> RewriteEngine on
RewriteCond %{REQUEST_FILENAME} !-d
RewriteCond %{REQUEST_FILENAME} !-f
RewriteRule . index.php [L]