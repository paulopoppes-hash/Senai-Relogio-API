# Senai-Relogio-API

API Express + Front-end consumindo a API

## Descrição

Atividade consistente em:
1. Criar uma API com Express que retorne data e hora atuais
2. Desenvolver uma aplicação Front-end que consuma a API e exiba a data e hora na tela

## Tecnologias

- Node.js
- Express.js
- CORS
- HTML5
- JavaScript (Fetch API)

## Arquivos

- `api.js` — Servidor Express com rota `GET /` retornando data e hora
- `index.html` — Front-end que consome a API via Fetch

## Como executar

### Backend (API)
1. Instale as dependências: `npm install express cors`
2. Execute o servidor: `node api.js`
3. Acesse: `http://localhost:3000/`

### Front-end
1. Abra o arquivo `index.html` no navegador
2. Altere a URL da API no script para a URL pública do deploy

## Repositório principal

[senai-framework-frontend](https://github.com/paulopoppes-hash/senai-framework-frontend)
