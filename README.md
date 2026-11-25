# Senai-Relogio-API

API Express + Front-end consumindo a API

## Descrição

Atividade consistente em:
1. **Criar uma API com Express** que possua uma rota para retornar data e hora atuais
2. **Desenvolver uma aplicação Front-end** em repositório separado que consuma a API hospedada e exiba a data e hora na tela

Esta atividade corresponde à **Aula 04 - Atividade 02** da disciplina Frameworks Front-end.

## Tecnologias utilizadas

- **Node.js** — ambiente de execução JavaScript no servidor
- **Express.js** — framework para criação de rotas e servidores web leves
- **CORS** — middleware para controle de acesso entre domínios diferentes
- **HTML5** — estrutura da aplicação front-end
- **JavaScript (Fetch API)** — consumo da API via requisições HTTP assíncronas

## Estrutura do projeto

```
relogio-api/
├── api.js          — servidor Express com rota GET /
├── index.html      — front-end que consome a API via fetch
├── package.json    — dependencias e scripts
└── README.md
```

## Como o protótipo funciona

### Backend (API)
O arquivo `api.js` cria um servidor Express com:
- Middleware `cors()` para permitir acesso de origens diferentes
- Rota `GET /` que retorna um JSON com a data e hora atuais no formato `pt-BR`
- O servidor escuta na porta 3000 (ou na variável de ambiente `PORT`)

Exemplo de resposta da API:
```json
{
  "date": "25/11/2026 20:30:00",
  "status": "API funcionando!"
}
```

### Front-end
O arquivo `index.html` exibe a data e hora atual em um card centralizado. Ao carregar a página e ao clicar no botão "Atualizar", o front-end faz uma requisição `fetch` para a API e exibe o resultado. A URL da API deve ser configurada no script (substitua `SUA-API-ON-RENDER.onrender.com` pela URL real do deploy).

## Conceitos aplicados (Aula 04 - Atividade 02)

- [x] Criação de API com Express.js
- [x] Protocolo HTTP e método GET
- [x] Formato JSON para troca de dados
- [x] CORS (Cross-Origin Resource Sharing)
- [x] Consumo de API com Fetch API no front-end
- [x] Requisições assíncronas (async/await)

## Como executar

### Backend (API)

1. Instale as dependencias:
   ```bash
   npm install
   ```
2. Execute o servidor:
   ```bash
   npm start
   ```
3. Acesse: `http://localhost:3000/`

### Front-end

1. Abra o arquivo `index.html` no navegador
2. Altere a URL da API no script JavaScript para a URL publica do deploy da sua API

## Repositorio principal

[senai-framework-frontend](https://github.com/paulopoppes-hash/senai-framework-frontend)
