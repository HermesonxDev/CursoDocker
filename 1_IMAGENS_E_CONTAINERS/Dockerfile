FROM node

# Define o diretório de trabalho
WORKDIR /src

# Copia os arquivos package primeiro (pra cache funcionar melhor)
COPY package*.json .

# Instala as dependências do Node
RUN npm install

# Copia o restante da aplicação
COPY . .

# Expõe a porta 3000
EXPOSE 3000

# Comando para rodar a aplicação "node app.js"
CMD ["node", "app.js"]