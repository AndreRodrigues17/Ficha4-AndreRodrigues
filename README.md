# Ficha4-AndreRodrigues

## Como correr

São precisos dois terminais.

Terminal 1 (server):

    cd server
    npm install
    node --watch server.js

O server fica em http://localhost:3000

Terminal 2 (client):

    cd client
    npm install
    npm run dev

A app React fica em http://localhost:5173

## Pergunta 3

Quem bloqueou foi o browser. O server respondeu normalmente: o endereço abre na barra do browser e o terminal do server não mostra nenhum erro. O browser recebeu a resposta, viu que faltava o header Access-Control-Allow-Origin e não deixou a app React ler os dados. Sei porque o erro "blocked by CORS policy" aparece na consola do browser (F12) e não no terminal do server.