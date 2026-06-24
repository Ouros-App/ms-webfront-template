# MS Webfront Template

Template base para frontend web com React, TypeScript, Vite e Tailwind CSS, já organizado para aplicações com consumo de API, autenticação, rotas privadas, hooks reutilizáveis e deploy via Docker.

## Stack

- React 19
- TypeScript
- Vite
- Tailwind CSS
- React Router
- Docker + Nginx

## Estrutura

```text
src/
  components/
  context/
  hooks/
  pages/
  reducers/
  routes/
  services/
  types/
  utils/
```

## Como usar

```bash
npm install
npm run dev
```

Aplicação local padrão:

- Dev: `http://localhost:5173`
- Preview/Docker: `http://localhost:4173` ou porta aleatória exposta pelos scripts

## Variáveis de ambiente

Copie `.env.example` para `.env` e ajuste:

```env
APP_NAME=ms-webfront-template
VITE_APP_TITLE=MS Webfront Template
VITE_API_URL=http://localhost:8000/api
VITE_STORAGE_VERSION=v1
PORT=4173
```

## Docker

Build e execução simples:

```bash
bash ./run.sh
```

Compose com instância incremental:

```bash
bash ./run_compose.sh
```

## Publicação

Atualize este campo com o link final da aplicação publicada:

- Produção: `https://seu-dominio-ou-app-publicado`
