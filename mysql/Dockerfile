FROM mysql:8.0
ENV MY_SQL_ROOT_PASSWORD="Roboshop@1"
COPY db/ /docker-entrypoint-initdb.d.
-e MYSQL_ROOT_PASSWORD=roboshop \
-e MYSQL_DATABASE=catalogue \
-e MYSQL_USER=roboshop \
-e MYSQL_PASSWORD=roboshop

