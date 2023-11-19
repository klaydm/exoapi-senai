# Projeto ExoApi SENAI
API para Gerenciamento de Projetos
Esta API permite gerenciar projetos, incluindo cadastrar, listar, buscar por ID, atualizar e deletar projetos.

## Tecnologias Utilizadas
ASP.NET Core
Entity Framework Core
SQL Server

## Estrutura da API
A API está organizada em três camadas:
Models: Representam os modelos de dados da aplicação.
Repositories: Encapsulam a lógica de acesso aos dados.
Controllers: Implementam os endpoints da API.

## Endpoints Disponíveis
GET /api/projetos: Lista todos os projetos.
POST /api/projetos: Cadastra um novo projeto.
GET /api/projetos/{id}: Busca um projeto específico pelo seu ID.
PUT /api/projetos/{id}: Atualiza um projeto existente.
DELETE /api/projetos/{id}: Deleta um projeto existente.

## Exemplos de Uso
### Cadastrar um novo projeto
JSON
{
  "NomeDoProjeto": "Projeto Novo",
  "Area": "Desenvolvimento Web",
  "Status": true
}

### Buscar um projeto específico pelo seu ID
GET /api/projetos/1
Atualizar um projeto existente
JSON
{
  "Id": 1,
  "NomeDoProjeto": "Projeto Atualizado",
  "Area": "Desenvolvimento Mobile",
  "Status": false
}

### Deletar um projeto existente
DELETE /api/projetos/1
