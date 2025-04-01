
# 🎉 Agência de Eventos — API + Front-End

Este é um projeto completo de **cadastro de clientes e eventos**, com autenticação de usuários e exibição de estatísticas, desenvolvido como proposta de **trabalho acadêmico** ou aplicação real. A API é construída em **Node.js com Express**, persistência em **PostgreSQL**, e front-end com **HTML + PicoCSS**.

## 📌 Funcionalidades

- ✅ Cadastro de **clientes** e seus dados.
- ✅ Registro de **eventos** associados aos clientes.
- ✅ Sistema de **autenticação** de usuários.
- ✅ Exibição de **estatísticas**: total de clientes, eventos e usuários.
- ✅ Front-end responsivo com Pico CSS.
- ✅ API RESTful com CORS liberado para integração externa.
- ✅ Deploy funcional usando **Vercel (API)** e **Neon (Banco de Dados PostgreSQL)**.

## 🚀 Tecnologias Utilizadas

### 🔧 Back-end (Node.js + Express)

- **Node.js** — Ambiente de execução JavaScript.
- **Express** — Framework web minimalista para criação da API.
- **pg** — Driver para PostgreSQL.
- **dotenv** — Para usar variáveis de ambiente localmente.
- **cors** — Middleware para liberar o acesso da API.

### 🗄 Banco de Dados

- **PostgreSQL** — Banco de dados relacional robusto e open-source.
- **Neon** — Hospedagem gratuita e escalável de bancos PostgreSQL na nuvem.

### 🎨 Front-end

- **HTML5**
- **PicoCSS** — Framework CSS leve, moderno e responsivo, sem necessidade de classes extras.

## 🗂️ Estrutura de Diretórios

```
├── rotas/                # Rotas da API (clientes, eventos, usuários, auth, estatísticas)
├── public/               # HTML + CSS (PicoCSS)
├── db.js                 # Conexão com PostgreSQL (Neon)
├── server.js             # Arquivo principal do servidor
├── modificarDB.js        # Executa init.sql para criar as tabelas
├── init.sql              # SQL de estrutura do banco
├── .env                  # Variáveis de ambiente (usado localmente)
└── package.json
```

## 🌐 Deploy

- **Backend:** Vercel
- **Banco de Dados:** Neon PostgreSQL


## 📃 Endpoints da API

| Método | Rota             | Descrição                          |
|--------|------------------|------------------------------------|
| POST   | `/clientes`      | Cadastrar novo cliente             |
| GET    | `/clientes`      | Listar todos os clientes           |
| GET    | `/clientes/:id`  | Obter cliente por ID               |
| PUT    | `/clientes/:id`  | Atualizar cliente                  |
| DELETE | `/clientes/:id`  | Remover cliente                    |
| POST   | `/eventos`       | Cadastrar novo evento              |
| GET    | `/eventos`       | Listar eventos + nome do cliente   |
| GET    | `/eventos/:id`   | Detalhes de um evento              |
| PUT    | `/eventos/:id`   | Atualizar evento                   |
| DELETE | `/eventos/:id`   | Remover evento                     |
| POST   | `/users`         | Criar usuário                      |
| GET    | `/users`         | Listar usuários                    |
| GET    | `/users/:id`     | Obter usuário por ID               |
| PUT    | `/users/:id`     | Atualizar usuário                  |
| DELETE | `/users/:id`     | Deletar usuário                    |
| POST   | `/login`         | Autenticação                       |
| GET    | `/statistics`    | Total de eventos, clientes, users  |

🧠 O que são as tecnologias usadas no projeto?
🟩 Node.js
É um ambiente de execução JavaScript fora do navegador, usado principalmente no back-end.

👉 Com o Node, conseguimos criar servidores e APIs que interagem com bancos de dados, arquivos, autenticação, etc.

⚙️ Express
É um framework para Node.js que facilita a criação de rotas, middlewares e estruturas de uma API web.

👉 Ele permite que a gente diga: “quando alguém acessar /clientes, execute essa função...”.

🧩 pg
É o driver oficial do PostgreSQL para Node.js. Ele permite que seu código JavaScript se conecte ao banco de dados, envie comandos SQL, receba resultados, etc.

🔐 dotenv
Permite armazenar dados sensíveis (como senhas e conexões) em um arquivo .env, fora do código.

👉 Com isso, o projeto pode ser versionado sem expor dados privados.

🌐 CORS
CORS significa "Cross-Origin Resource Sharing". Esse middleware permite que o front-end (por exemplo, vindo de vercel.app) acesse sua API mesmo que estejam em domínios diferentes.

🧮 PostgreSQL
É um banco de dados relacional poderoso e gratuito, amplamente usado no mercado.

👉 Ele armazena dados em tabelas (clientes, eventos, usuários) e suporta relacionamentos, índices e mais.

☁️ Neon
É uma plataforma que hospeda bancos PostgreSQL na nuvem gratuitamente.

👉 Você pode acessar seu banco de dados a partir de qualquer API, sem precisar instalar nada localmente.

🚀 Vercel
É uma plataforma de deploy que roda seu back-end ou front-end automaticamente a partir do GitHub.

👉 No nosso caso, ela hospeda a API em Node.js de forma gratuita e escalável.

🎨 Pico CSS
É um framework CSS minimalista.

👉 Com ele, os formulários e botões já ficam bonitos e responsivos sem precisar escrever estilos manuais.

