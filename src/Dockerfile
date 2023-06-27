FROM node:latest 
#imagem que roda a aplicação
WORKDIR /app
#criação da pasta que vai instalar a aplicação
COPY package*.json ./
#para da instalaçaõ do node com app precisa do package.json
#que ajuda no gerenciamento de pacotes que precisa do npm
RUN npm install
COPY . .
# Esse comando é para fazer a copia de todas a pasta do diretoria que estou querendo
#rodar a aplicação 
EXPOSE 8080
#é a portar que a aplicação server.js estará rodando
CMD ["node", "server.js"]
#o Cmd do node é esse para inicializar a aplicação em node