FROM mysql:8.0.33
LABEL "Project"="Vprofile"
LABEL "Author"="arjun"

ENV MYSQL_ROOT_PASSWORD="vprodbpass"
ENV MYSQL_DATABASE="accounts"


ADD db_backup.sql docker-entrypoint-initdb.d/db_backup.sql      

# docker-entrypoint-initdb.d directory is a special directory in the MySQL Docker image.
# SQL files placed in this 'docker-entrypoint-initdb.d' directory are automatically executed when the container is started 
# Adds a (db_backup.sql) SQL script to be executed during the initialization of the MySQL