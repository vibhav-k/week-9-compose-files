#Dockerfile

FROM mysql

WORKDIR /var/lib/mysql
ADD ./data/files/mydb.sql /docker-entrypoint-initdb.d

EXPOSE 3306

