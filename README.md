# Case de Avaliação para Estágio em DevOps

Este projeto integra um backend em Ruby on Rails com um frontend em React/Vite, utilizando Docker e Docker Compose. O backend e o frontend estão configurados para se comunicar corretamente e realizar interações com um banco de dados SQLite.

## Como Rodar os Containers Localmente

### Pré-requisitos
- **Docker** e **Docker Compose** instalados na sua máquina.
  - Se você ainda não tem o Docker, pode instalá-lo a partir do [site oficial](https://www.docker.com/get-started).
  - Docker Compose já vem junto com o Docker a partir da versão 1.27.0.

### Passos para rodar os containers

1. **Clone o repositório** (caso ainda não tenha feito isso):
   ```bash
   git clone https://github.com/EstherMart/devopscaseback
   ```

2. **Subir os Containers com Docker Compose**
Com o Docker e Docker Compose instalados, use o seguinte comando para rodar os containers localmente:

```bash
docker-compose up --build
``` 

Este comando irá:

- Criar e iniciar os containers para o backend, frontend e banco de dados.
- Instalar as dependências do backend e do frontend.
- Criar e migrar o banco de dados para o backend.

3. Acessar a Aplicação
Após a execução do comando, os containers estarão rodando e você pode acessar a aplicação da seguinte forma:

**Frontend**: Acesse a interface do usuário em https://devopscasefront.vercel.app/. no seu navegador.
**Backend (API):** A API estará disponível em http://localhost:3000 e pode ser acessada pelo frontend.
