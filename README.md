# Configuracion-Servidores
Tips de configuración de Servidor


## Sitemap
Generación

## Robots
Añadir el Site map Sitemap: 'https://medssocial.com/sitemap.xml'

## Schema
Generar https://technicalseo.com/seo-tools/schema-markup-generator/

## Cache Servidor
<IfModule mod_expires.c>
  ExpiresActive On
  ExpiresByType image/jpg "access 1 year"
  ExpiresByType image/jpeg "access 1 year"
  ExpiresByType image/gif "access 1 year"
  ExpiresByType image/png "access 1 year"
  ExpiresByType text/css "access 1 month"
  ExpiresByType text/html "access 1 month"
  ExpiresByType application/pdf "access 1 month"
  ExpiresByType text/x-javascript "access 1 month"
  ExpiresByType application/x-shockwave-flash "access 1 month"
  ExpiresByType image/x-icon "access 1 year"
  ExpiresDefault "access plus 1 month"
</IfModule>

## Direción IP Servidor
La dirección IP del servidor, o apunta al dominio del servidor o a ningún lado.

## Headers
Elimianr Powered by" de Plesk y de la versión PHP
