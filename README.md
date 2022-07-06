# IEPC_Memorama

Set this on a NGINX web server

'''
server {
        listen 80 default_server;
        listen [::]:80 default_server;

        root /var/www/html/iepc;

        index index.html index.htm index.nginx-debian.html;

        server_name _;

        location / {
                try_files $uri $uri/ =404;
                autoindex on;
        }
}
'''

## BackEnd Server

On your Linux Server:

            cronrab -e

Then:

            @reboot sudo python3 /var/www/html/iepc/server.py

## Technologies

* HTML
* SCSS
* Vanilla Javascript
* Boostrap 5
* Axios
* Python
* Flask
* Sqlite3