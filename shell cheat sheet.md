# Shell Cheat Sheet

## File & Folder Operations

Delete a directory:`
rm -r directory
`

Delete file:`
rm FILETODELETE
`

New directory:`
mkdir FOLDERNAME
`

Copy file:`
cp SOURCE DEST
`

Copy folder:`
cp -avr SOURCE DEST
`

Watch file:`
less +F YOUR.LOG
`

## CURL

Download file:`
curl -O URLHERE
`

## Zipping & Uzipping

Unzip:`
unzip FILENAME.ZIP
`

Untar & Gzip:`
tar -xzf FILENAME.TAR.GZ
`

Zip folder:`
zip -er DESTINATION.ZIP FOLDER
`

## Apache

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

## Processes

Kill process:`
kill -9 PROCESSID
`

Find process:`
ps -ef | grep PROCESS NAME
`

Root process list:`
ps -u root
`