# CommerceAPI
Esta é uma API RESTful que gerencia produtos e usuários, utilizando o Slim Framework para a construção de APIs. A API inclui autenticação JWT para autenticação de usuário e o MySQL como banco de dados.

## Funcionalidades

- **Produtos:** Operações CRUD (Criar, Ler, Atualizar, Excluir) para gerenciar informações sobre produtos.
- **Usuários:** Registro de usuários, login e perfis de usuário com autenticação JWT.

## Tecnologias Utilizadas

- **Slim Framework:** Um micro framework PHP para o desenvolvimento de APIs e aplicações web.
- **JWT (JSON Web Tokens):** Para autenticação e autorização segura do usuário.
- **MySQL:** Um banco de dados relacional para armazenamento de dados.
- **PHP:** Linguagem de programação do lado do servidor.

## Estrutura do Projeto

- `app/`: Lógica da aplicação, incluindo rotas, controladores e middleware.
- `public/`: Diretório público acessível para o servidor web.

## Configuração

1. Clone o repositório: `git clone https://github.com/1bertojunior/CommerceAPI.git`.
2. Instale as dependências: `composer install`.

## Uso

1. Inicie o servidor embutido do PHP: `php -S localhost:8000 -t public/`.
2. Acesse as rotas da API utilizando uma ferramenta como [Postman](https://www.postman.com/) ou [cURL](https://curl.se/).

## Autenticação JWT

A autenticação JWT é necessária para acessar algumas rotas da API. Faça uma requisição POST para `/api/login` com as credenciais do usuário para obter o token JWT. Inclua o token nas requisições subsequentes no cabeçalho `Authorization`.

## Estrutura do Slim Framework

O projeto segue a estrutura de diretórios recomendada pelo Slim Framework:

- `src/`: Código-fonte da aplicação, organizado por namespaces.
- `public/`: Raiz do servidor web, contém assets e ponto de entrada para requisições web.
- `templates/`: Arquivos de template para renderização de visualizações.

# API Endpoints

## Produtos

- **Listar Produtos**: `GET /api/v1/produtos/lista`
- **Adicionar Produto**: `POST /api/v1/produtos/adiciona`
- **Recuperar Produto por ID**: `GET /api/v1/produtos/lista/{id}`
- **Atualizar Produto por ID**: `PUT /api/v1/produtos/atualiza/{id}`
- **Remover Produto por ID**: `GET /api/v1/produtos/remove/{id}`

## Usuários (Login)

- **Gerar Token**: `POST /api/token`

### Exemplo de requisição

```json
{
  "email": "seuemail@example.com",
  "senha": "suasenha"
}
```

## Como Contribuir

1. Faça um fork do repositório.
2. Clone o fork para sua máquina local.
3. Faça suas modificações e adições.
4. Envie um pull request para análise.

Obrigado por contribuir para o desenvolvimento da SlimCommerceAPI! Juntos, estamos criando uma API poderosa e segura.

Divirta-se explorando a API!
