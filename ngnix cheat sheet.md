# nginx

## [Setting up a virtual host](https://www.digitalocean.com/community/tutorials/how-to-set-up-nginx-virtual-hosts-server-blocks-on-ubuntu-12-04-lts--3)

Enable a site:`
sudo ln -s /etc/nginx/sites-available/SITENAME /etc/nginx/sites-enabled/SITENAME
`

Reload server:`
sudo service nginx restart
`