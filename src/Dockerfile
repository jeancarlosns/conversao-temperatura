# Utilizando a imagem base do Node.js
FROM node:18-alpine

# Definindo o diretório de trabalho
WORKDIR /app

# Copiando o package.json e instalando as dependências
COPY package*.json ./
RUN npm install

# Copiando o restante do código para o container
COPY . .

# Expondo a porta da aplicação
EXPOSE 8080

# Comando para rodar a aplicação
CMD ["npm", "start"]