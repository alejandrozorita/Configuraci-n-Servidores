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

## Servidor
### Activar compresión
Activar el módulo mod_deflate para comprimir la respuesta del servidor
- https://support.plesk.com/hc/en-us/articles/115000716649-How-to-enable-gzip-compression-in-Apache-on-Plesk-server-
- https://www.techrepublic.com/article/how-to-configure-apache-moddeflate-to-enhance-web-server-performance/
- https://www.techrepublic.com/article/how-to-configure-apache-moddeflate-to-enhance-web-server-performance/
- https://developers.google.com/speed/webp/


<IfModule mod_deflate.c>
  # Compress HTML, CSS, JavaScript, Text, XML and fonts
  AddOutputFilterByType DEFLATE application/javascript
  AddOutputFilterByType DEFLATE application/rss+xml
  AddOutputFilterByType DEFLATE application/vnd.ms-fontobject
  AddOutputFilterByType DEFLATE application/x-font
  AddOutputFilterByType DEFLATE application/x-font-opentype
  AddOutputFilterByType DEFLATE application/x-font-otf
  AddOutputFilterByType DEFLATE application/x-font-truetype
  AddOutputFilterByType DEFLATE application/x-font-ttf
  AddOutputFilterByType DEFLATE application/x-javascript
  AddOutputFilterByType DEFLATE application/xhtml+xml
  AddOutputFilterByType DEFLATE application/xml
  AddOutputFilterByType DEFLATE font/opentype
  AddOutputFilterByType DEFLATE font/otf
  AddOutputFilterByType DEFLATE font/ttf
  AddOutputFilterByType DEFLATE image/svg+xml
  AddOutputFilterByType DEFLATE image/x-icon
  AddOutputFilterByType DEFLATE text/css
  AddOutputFilterByType DEFLATE text/html
  AddOutputFilterByType DEFLATE text/javascript
  AddOutputFilterByType DEFLATE text/plain
  AddOutputFilterByType DEFLATE text/xml

  # Remove browser bugs (only needed for really old browsers)
  BrowserMatch ^Mozilla/4 gzip-only-text/html
  BrowserMatch ^Mozilla/4\.0[678] no-gzip
  BrowserMatch \bMSIE !no-gzip !gzip-only-text/html
  Header append Vary User-Agent
</IfModule>
