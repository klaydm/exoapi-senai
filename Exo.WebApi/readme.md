# Projeto ExoApi SENAI
API para Gerenciamento de Projetos
Esta API permite gerenciar projetos, incluindo cadastrar, listar, buscar por ID, atualizar e deletar projetos.

## Tecnologias Utilizadas
ASP.NET Core
Entity Framework Core
SQL Server

## Requisitos
Dotnet 6.0 ou superior

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

## Modelo de usuário
O modelo de usuário é simples, com apenas três propriedades:

Id: O ID do usuário no banco de dados.
Email: O endereço de e-mail do usuário.
Senha: A senha do usuário.

## Repositório de usuários
O repositório de usuários fornece as seguintes operações:

Login(): Retorna um usuário se o e-mail e a senha fornecidos corresponderem a um usuário no banco de dados.
Listar(): Retorna uma lista de todos os usuários no banco de dados.
Cadastrar(): Adiciona um novo usuário ao banco de dados.
BuscarPorId(): Retorna um usuário com o ID especificado.
Atualizar(): Atualiza as informações de um usuário no banco de dados.
Deletar(): Remove um usuário do banco de dados.

## Controlador de usuários
O controlador de usuários implementa os endpoints da API para usuários. Os endpoints são os seguintes:

GET /api/usuarios: Lista todos os usuários.
POST /api/usuarios: Cadastra um novo usuário.
GET /api/usuarios/{id}: Busca um usuário específico pelo seu ID.
PUT /api/usuarios/{id}: Atualiza um usuário existente pelo seu ID.
DELETE /api/usuarios/{id}: Deleta um usuário existente pelo seu ID.

## Exemplos de uso
### Cadastrar um novo usuário

POST /api/usuarios
{
  "Email": "meu@email.com",
  "Senha": "minha-senha"
}

### Buscar um usuário específico pelo seu ID

GET /api/usuarios/1

### Atualizar um usuário existente

PUT /api/usuarios/1
{
  "Email": "meu-novo@email.com",
  "Senha": "minha-nova-senha"
}

### Deletar um usuário existente

DELETE /api/usuarios/1

## Observações

O código fornecido é apenas um exemplo. Você pode modificá-lo para atender às suas necessidades específicas.
O código está escrito em C# usando o ASP.NET Core, o Entity Framework Core e o SQL Server.
