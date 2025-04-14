FROM php:8-apache

# Define o diretório de trabalho
WORKDIR /var/www/html/

# Copia a aplicação para dentro do container
COPY . .

# Expõe a porta 80
EXPOSE 80

# Garante que o servidor web (rodando como www-data) tenha permissão total
# sobre os arquivos da aplicação, evitando erros de permissão em tempo de execução.
RUN chown -R www-data:www-data /var/www
