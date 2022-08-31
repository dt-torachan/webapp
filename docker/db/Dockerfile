FROM mysql:5.7
RUN mysqld --character-set-server=utf8mb4 --collation-server=utf8mb4_unicode_ci
COPY data /var/lib/mysql
COPY my.cnf /etc/mysql/conf.d/my.cnf