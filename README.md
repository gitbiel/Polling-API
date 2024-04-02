# API de Votação em Enquetes
### Descrição
Esta é uma API para criar e gerenciar enquetes online. Ela permite aos usuários criar enquetes, votar em opções e ver os resultados em tempo real. O projeto utiliza Fastify como framework web, Prisma para gerenciamento de banco de dados e Redis para caching.

### Instalação
Clone o repositório:

```bash
 git clone https://github.com/gitbiel/Polling-API.git
```
### Instale as dependências:

```bash
npm install
```

### Uso
Inicie os serviços PostgreSQL e Redis usando o Docker Compose:
```bash
docker-compose up -d
```

### Crie um arquivo .env na raiz do projeto com o seguinte conteúdo:

```bash
DATABASE_URL="postgresql://docker:docker@localhost:5432/polls?schema=public"
```

### Inicie o servidor:

```bash
npm run dev
```
## Endpoints
- POST /polls: Crie uma nova enquete
- GET /polls/:id: Obtenha detalhes de uma enquete específica
- POST /polls/:id/vote: Vote em uma enquete
  
## Dependências
- Fastify
- Prisma
- Redis
- Zod
