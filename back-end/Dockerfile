# Use uma imagem base do Node.js com a versão desejada
FROM node:16

# Defina o diretório de trabalho dentro do contêiner
WORKDIR /app

# Copie o arquivo package.json e o arquivo package-lock.json (se existir)
COPY package.json .

# Instale as dependências do projeto
RUN npm install

# Copie o restante dos arquivos da aplicação
COPY . .

# Expõe a porta em que a aplicação irá escutar
EXPOSE 3000

# Comando para iniciar a aplicação
CMD [ "npm", "run", "dev" ]
