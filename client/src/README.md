# Ficha 4 – Redes de Comunicação

App React que vai buscar as cartas a um server Express, através de uma API em JSON.

## Como correr

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