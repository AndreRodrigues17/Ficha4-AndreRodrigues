Ficha 4 – Redes de Comunicação

App React que vai buscar as cartas a um server Express, através de uma API em JSON.

Como correr

São precisos dois terminais.

Terminal 1 (server):

em bash
cd server
npm install
node --watch server.js


O server fica em http://localhost:3000

Terminal 2 (client):

em bash
cd client
npm install
npm run dev


A app fica em http://localhost:5173

A API está em http://localhost:3000/api/cartas

Pergunta 3

Quem bloqueou foi o browser, não o server. O server recebeu o pedido e respondeu com o JSON normalmente (no Network tab o request aparece com o estado 200 e o terminal do server não mostra nenhum erro). Foi o browser que, ao ver que faltava o header Access-Control-Allow-Origin, não deixou o código React ler a resposta e mostrou o erro de CORS na consola. Escrever o endereço na barra funciona porque aí não há CORS, só se aplica a pedidos feitos por código de outra origem.
