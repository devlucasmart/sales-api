# Sales API

Bem-vindo à **Sales API**, uma API RESTful para gerenciar vendas utilizando Node.js, Express e MongoDB. Esta documentação fornece todas as informações necessárias para configurar, executar e utilizar a API.

## Índice

- [Visão Geral](#visão-geral)
- [Recursos da API](#recursos-da-api)
- [Instalação](#instalação)
- [Configuração](#configuração)
- [Autenticação](#autenticação)
- [Endpoints](#endpoints)
- [Contribuição](#contribuição)
- [Licença](#licença)

---

## Visão Geral

A **Sales API** foi desenvolvida para facilitar a gestão de vendas, permitindo operações CRUD (Criar, Ler, Atualizar, Deletar) em vendas armazenadas em um banco de dados MongoDB.

---

## Recursos da API

- **Gerenciamento de Vendas**: Crie, visualize, atualize e exclua registros de vendas.
- **Relatórios de Vendas**: Obtenha relatórios detalhados sobre vendas.
- **Escalabilidade**: Construída para suportar grandes volumes de dados com MongoDB.

---

## Instalação

Para instalar e configurar a Sales API, siga os passos abaixo:

1. **Clone o repositório:**

    ```bash
    git clone https://github.com/seu-usuario/sales-api.git
    cd sales-api
    ```

2. **Instale as dependências usando Yarn:**

    ```bash
    yarn install
    ```

3. **Configure as variáveis de ambiente:**

    Crie um arquivo `.env` na raiz do projeto e adicione as seguintes variáveis:

    ```
    PORT=3000
    MONGODB_URI=sua-string-de-conexão-com-o-MongoDB
    JWT_SECRET=sua-chave-secreta-para-gerar-o-JWT
    ```

---

## Configuração

1. **Configuração do MongoDB:**

    Certifique-se de ter uma instância do MongoDB rodando localmente ou em um serviço na nuvem. Atualize a variável `MONGODB_URI` no arquivo `.env` com a string de conexão correta.

2. **Configuração do JWT:**

    Defina a variável `JWT_SECRET` no arquivo `.env` com uma chave secreta forte para gerar os tokens JWT utilizados na autenticação.

---

## Autenticação

A autenticação na Sales API é feita usando tokens JWT (JSON Web Tokens). Para obter acesso aos endpoints protegidos, inclua o token JWT na requisição HTTP no cabeçalho de autorização (`Authorization: Bearer <seu-token>`).

---

## Endpoints

A API possui os seguintes endpoints principais:

- `GET /sales`: Retorna todas as vendas.
- `GET /sales/:id`: Retorna uma venda específica pelo ID.
- `POST /sales`: Cria uma nova venda.
- `PUT /sales/:id`: Atualiza uma venda existente pelo ID.
- `DELETE /sales/:id`: Exclui uma venda pelo ID.

Consulte a documentação da API para mais detalhes sobre os parâmetros e respostas esperadas de cada endpoint.

---

## Contribuição

Contribuições são bem-vindas! Para contribuir com a Sales API, siga estas etapas:

1. Faça um fork do repositório.
2. Crie uma branch com o nome da sua feature (`git checkout -b feature/nova-feature`).
3. Commit suas mudanças (`git commit -am 'Adiciona nova feature'`).
4. Faça push para a branch (`git push origin feature/nova-feature`).
5. Abra um Pull Request.

---

## Licença

Este projeto está licenciado sob a Licença MIT - veja o arquivo [LICENSE](./LICENSE) para mais detalhes.
