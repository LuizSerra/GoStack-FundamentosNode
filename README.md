
<img alt="GoStack" src="https://storage.googleapis.com/golden-wind/bootcamp-gostack/header-desafios.png" />

<h3 align="center">
  Desafio 05: Primeiro projeto Node.js
</h3>

<blockquote align="center">“Para quem fica melhor a cada dia, ficar pronto é utopia”!</blockquote>

<p align="center">
  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/rocketseat/bootcamp-gostack-desafios?color=%2304D361">

  <a href="https://rocketseat.com.br">
    <img alt="Made by Rocketseat" src="https://img.shields.io/badge/made%20by-Rocketseat-%2304D361">
  </a>

  <img alt="License" src="https://img.shields.io/badge/license-MIT-%2304D361">

  <a href="https://github.com/Rocketseat/bootcamp-gostack-desafios/stargazers">
    <img alt="Stargazers" src="https://img.shields.io/github/stars/rocketseat/bootcamp-gostack-desafios?style=social">
  </a>
</p>

<p align="center">
  <a href="#rocket-sobre-o-desafio">Sobre o desafio</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#memo-licença">Licença</a>
</p>

## :rocket: Sobre o desafio

Nesse desafio, você deve criar uma aplicação para continuar treinando o que você aprendeu até agora no Node.js junto ao TypeScript, utilizando o conceito de models, repositories e services!

Essa será uma aplicação para armazenar transações financeiras de entrada e saída, que deve permitir o cadastro e a listagem dessas transações.

## :hammer: Tecnologias

 - [NodeJS](https://nodejs.org/)
 - [TypeScript](https://www.typescriptlang.org/)
 - [Express](https://expressjs.com/)
 - [TypeORM](https://typeorm.io/)
 - [uuidv4](https://www.npmjs.com/package/uuidv4)
 
## :key: Como rodar esse projeto.

### :sheep: Clonando o repositório.
```
# Clone este repositório
$ git clone https://github.com/LuizSerra/GoStack-FundamentosNode.git

# Acesse a pasta do projeto no terminal/cmd
$ cd gostack-fundamentos-node
```
### :computer: Rodando a aplicação.

```
# Instale as dependências
$ yarn

# Execute a Aplicação
$ yarn dev:server

# Execute o teste da Aplicação
$ yarn test

# O servidor inciará na porta:3333 - acesse http://localhost:3333
```

## :twisted_rightwards_arrows: Rotas da aplicação.

- **`POST /transactions`**: A rota deve receber `title`, `value` e `type` dentro do corpo da requisição, sendo `type` o tipo da transação, que deve ser `income` para entradas (depósitos) e `outcome` para saídas (retiradas). Ao cadastrar uma nova transação, ela deve ser armazenada dentro de um objeto com o seguinte formato :

```json
{
  "id": "uuid",
  "title": "Salário",
  "value": 3000,
  "type": "income"
}
```

- **`GET /transactions`**: Essa rota deve retornar uma listagem com todas as transações que você cadastrou até agora, junto com o valor de soma de entradas, retiradas e total de crédito. Essa rota deve retornar um objeto com o formato a seguir:

```json
{
  "transactions": [
    {
      "id": "uuid",
      "title": "Salário",
      "value": 4000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Freela",
      "value": 2000,
      "type": "income"
    },
    {
      "id": "uuid",
      "title": "Pagamento da fatura",
      "value": 4000,
      "type": "outcome"
    },
    {
      "id": "uuid",
      "title": "Cadeira Gamer",
      "value": 1200,
      "type": "outcome"
    }
  ],
  "balance": {
    "income": 6000,
    "outcome": 5200,
    "total": 800
  }
}
```
## :computer: Quer contribuir com o Projeto? Saiba como:

-   Faça um  **fork**  do projeto;
-   Crie uma nova branch com as suas alterações:  `git checkout -b my-feature`
-   Salve as alterações e crie uma mensagem de commit contando o que você fez:`git commit -m "feature: My new feature"`
-   Envie as suas alterações:  `git push origin my-feature`

> Caso tenha alguma dúvida confira este [guia de como contribuir no GitHub](https://github.com/firstcontributions/first-contributions)


## :memo: Licença

Esse projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

Feito com dedicação por Luiz Serra 👋🏽 [Entre em contato](https://www.linkedin.com/in/luizserra)!

