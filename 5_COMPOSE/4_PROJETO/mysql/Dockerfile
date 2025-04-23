FROM mysql:5.7

# Copia o arquivo que vai criar o banco
COPY schema.sql /docker-entrypoint-initdb.d/

# Expõe a porta usada pelo MySQL
EXPOSE 3306