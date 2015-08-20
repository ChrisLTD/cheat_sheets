# Apache

Enable site:`
sudo a2ensite
`

Disable site:`
sudo a2dissite
`

List apache modules:`
apache2ctl -M
`

Enable an apache2 module:`
sudo a2enmod
`

Disable an apache2 module:`
sudo a2dismod
`

Reload server:`
service apache2 reload
`

Force reload the server:`
sudo /etc/init.d/apache2 force-reload
`

Apache file permissions:
```
chown -R www-data:www-data /folder/
chmod +r /folder
```

Virtual Host:
```
<VirtualHost *:80>
  DocumentRoot /var/www/site
  ServerName site.example.com
  CustomLog /var/www/logs/site/access.log combined
  ErrorLog /var/www/logs/site/error.log
</VirtualHost>
```