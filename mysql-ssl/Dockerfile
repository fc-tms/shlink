FROM mysql:8.0

COPY --chmod=600 --chown=mysql:mysql ca.pem server-cert.pem server-key.pem /etc/certs/
COPY ssl.cnf /etc/mysql/conf.d
COPY *.sql.* /docker-entrypoint-initdb.d
