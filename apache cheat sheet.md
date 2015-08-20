# Apache

Enable site:`
sudo a2ensite
`

Disable site:`
sudo a2dissite
`

Enable an apache2 module:`
sudo a2enmod
`

Disable an apache2 module:`
sudo a2dismod
`

Force reload the server:`
sudo /etc/init.d/apache2 force-reload
`

Virtual Host:
```
<VirtualHost *:80>
  DocumentRoot /var/www/site
  ServerName site.example.com
  CustomLog /var/www/logs/site/access.log combined
  ErrorLog /var/www/logs/site/error.log
</VirtualHost>
```