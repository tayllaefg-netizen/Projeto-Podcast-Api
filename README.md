# Podcast API

API desenvolvida no bootcamp da DIO com Node.js e TypeScript para listar e filtrar episódios de podcasts em vídeo. O projeto utiliza o módulo HTTP nativo do Node.js, sem Express, e organiza o código em camadas simples.

## Funcionalidades

- Listar episódios cadastrados.
- Filtrar episódios pelo nome do podcast.
- Retornar dados em formato JSON.
- Ler informações a partir de um arquivo local.

## Tecnologias

- Node.js
- TypeScript
- TSX
- TSUP
- HTTP nativo do Node.js

## Como executar

Instale as dependências:

```bash
npm install
```

Crie ou mantenha um arquivo `.env` na raiz do projeto:

```env
PORT=3333
```

Execute em desenvolvimento:

```bash
npm run start:dev
```

Acesse:

```txt
http://localhost:3333/api/list
```

## Rotas

```http
GET /api/list
```

```http
GET /api/podcasts?p=flow
```

## Estrutura

```txt
src/
  app.ts
  server.ts
  controllers/
  models/
  repositories/
  routes/
  services/
  utils/
```

## Scripts

```json
{
  "start:dev": "tsx --env-file=.env src/server.ts",
  "start:watch": "tsx watch --env-file=.env src/server.ts",
  "dist": "tsup src",
  "start:dist": "npm run dist && node --env-file=.env dist/server.js"
}
```

<a href="https://github.com/tayllaefg-netizen" target="_blank">
  <img src="https://img.shields.io/badge/GitHub-Taylla-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Taylla">
</a>
