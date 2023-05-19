# Use a imagem base do Node.js
FROM node:14-alpine

# Defina o diretório de trabalho dentro do contêiner
WORKDIR /app

# Copie o arquivo package.json e o package-lock.json para o diretório de trabalho
COPY package*.json ./

# Instale as dependências do projeto
RUN npm install

# Copie o código fonte para o diretório de trabalho
COPY . .

# Exponha a porta do servidor da aplicação
EXPOSE 3000

# Inicie o servidor da aplicação
CMD ["npm", "start"]
