FROM python:3

# Atualiza pacotes e instala dependências do sistema (se necessário)
RUN apt-get update -y && \
    apt-get install -y build-essential

# Define o diretório de trabalho
WORKDIR /app

# Copia o requirements.txt primeiro (pra cache funcionar melhor)
COPY requirements.txt .

# Instala as dependências Python
RUN pip install --no-cache-dir -r requirements.txt

# Copia o restante da aplicação
COPY . .

# Expõe a porta usada pelo Flask
EXPOSE 5000

# Comando para rodar a aplicação "python ./app.py"
CMD ["python", "./app.py"]