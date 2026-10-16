# 📋 Sistema Gerenciador de Tarefas — API REST

API REST desenvolvida em **C# e ASP.NET Core**, utilizando **Entity Framework Core** e **SQL Server** para gerenciamento de tarefas.

Projeto desenvolvido como parte do desafio prático da **Digital Innovation One (DIO)**, com o objetivo de aplicar conceitos de desenvolvimento Backend, persistência de dados e operações CRUD.

## 🚀 Tecnologias utilizadas

- C# e .NET 6
- ASP.NET Core Web API
- Entity Framework Core
- Microsoft SQL Server
- Swagger / OpenAPI
- Git e GitHub

## ⚙️ Funcionalidades

A aplicação permite:

- Cadastrar novas tarefas.
- Consultar todas as tarefas cadastradas.
- Buscar tarefas pelo identificador.
- Filtrar tarefas por título, data e status.
- Atualizar informações de tarefas existentes.
- Excluir tarefas.

## 🔗 Endpoints da API

| Método | Endpoint | Descrição |
|---|---|---|
| GET | `/Tarefa/{id}` | Buscar tarefa pelo ID |
| GET | `/Tarefa/ObterTodos` | Listar todas as tarefas |
| GET | `/Tarefa/ObterPorTitulo` | Filtrar pelo título |
| GET | `/Tarefa/ObterPorData` | Filtrar pela data |
| GET | `/Tarefa/ObterPorStatus` | Filtrar pelo status |
| POST | `/Tarefa` | Cadastrar uma tarefa |
| PUT | `/Tarefa/{id}` | Atualizar uma tarefa |
| DELETE | `/Tarefa/{id}` | Excluir uma tarefa |

## 🗄️ Banco de dados

A aplicação utiliza **SQL Server** e **Entity Framework Core**, com migrations para gerenciamento da estrutura do banco de dados.

### Configuração local

**Pré-requisitos:**

- SDK do .NET 6
- SQL Server
- Ferramenta `dotnet-ef`

Clone o repositório:

```bash
git clone https://github.com/jose-nt7/trilha-net-api-desafio.git
cd trilha-net-api-desafio
```

Configure a string de conexão `ConexaoPadrao` no arquivo `appsettings.json` de acordo com sua instância local do SQL Server.

Restaure as dependências:

```bash
dotnet restore
```

Aplique as migrations:

```bash
dotnet ef database update
```

Execute a aplicação:

```bash
dotnet run
```

Acesse a documentação interativa do Swagger pelo endereço HTTPS informado no terminal, acrescentando `/swagger`.

## 🧪 Testes realizados

As funcionalidades foram verificadas por meio do Swagger, incluindo cadastro, consulta, filtros, atualização e exclusão de tarefas.

A aplicação foi executada localmente com integração ao SQL Server.

## 📚 Documentação original

O material original disponibilizado pela DIO foi preservado em [docs/README-DIO.md](docs/README-DIO.md).

## 👨‍💻 Autor

**José Ribeiro**

Projeto desenvolvido para fins educacionais e aprimoramento das habilidades em desenvolvimento Backend com C# e .NET.