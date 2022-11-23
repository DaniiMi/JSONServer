# JSONServer

1- Acessei o site https://www.npmjs.com/package/json-server para obtenção dos códigos

2- Criei uma pasta

3- No terminal executei o comando para instalar o Servidor:
npm install -g json-server

4- Criei um arquivo na Pasta Server Teste: db.json
 Dentro do banco, foi criada rotas personalizadas
 
5- No terminal foi executado o comando para start do banco de dados:
npx json-server --watch db.json

6- ciado um arquivo: server.js
- inserido o js da documentação no server.js:
// server.js
const jsonServer = require('json-server')
const server = jsonServer.create()
const router = jsonServer.router('db.json')
const middlewares = jsonServer.defaults()
server.use(middlewares)
server.use(router)
server.listen(3000, () => {
console.log('JSON Server is running')
})

7 - No Terminal, foi inserido o comando da documentação para executar o JS acima:
npm install json-server --save-dev //Instalação do servidor local

8 - Executar o comando para execução do node:
node server.js
