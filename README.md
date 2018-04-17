# Udacity-AnimeCatalog
Repo for udacity assignment # 3 

Server IP: 35.154.103.81

Server access port : 2200

Application URL: http://35.154.103.81.xip.io/

## Software installed: 
Nginx

uwsgi server

Pip packages: slqalchemy, flask , psycopg2, oauth2client

## Configuration changes:
1. Added the recommended user with proper privileges.
2. All ports blocked except the required(+port 22 , somehow still needed for AWS services even after default port changed).
3. uwsgi configured to serve animeCatalog with 5 worker threads.
4. nginx configured to access uwsgi through Unix Socket.

## Also setup a DigitalOcean server
For running other projects in together and a central directory for all my applications
[http://apps.achopra.me]

## Resources used:
https://www.digitalocean.com/community/tutorials/how-to-serve-flask-applications-with-uwsgi-and-nginx-on-ubuntu-14-04

https://stackoverflow.com/questions/9353822/connecting-postgresql-with-sqlalchemy

https://stackoverflow.com/questions/23839656/sqlalchemy-no-password-supplied-error

https://stackoverflow.com/questions/13485030/strange-postgresql-value-too-long-for-type-character-varying500
