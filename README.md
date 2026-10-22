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

## Pergunta 4

Na Ficha 3, ESCREVE AQUI A TUA RESPOSTA 4 DA FICHA 3.
Agora a app React faz 1 request às cartas quando abre (2 em desenvolvimento, por causa do StrictMode) e 0 quando filtro, porque o filtro é feito no browser com os dados que já chegaram. Os dados vivem no server, no array do server.js, e chegam em JSON. O HTML é construído no browser, pelo React, a partir desses dados.