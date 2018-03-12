FROM mysql:latest
MAINTAINER karaga <mohamedkaraga75@gmail.com>

# ROOT PASSWORD
ENV MYSQL_ROOT_PASSWORD=mypassword

COPY doc.sql /docker-entrypoint-initdb.d/

RUN /etc/init.d/mysql start ; mysql -u root -p$MYSQL_ROOT_PASSWORD < /docker-entrypoint-initdb.d/doc.sql
