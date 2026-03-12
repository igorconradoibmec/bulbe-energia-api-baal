<div align="center">

# Bulbe Energia API

**Backend do sistema de monitoramento de energia renovavel**
Projeto desenvolvido para a disciplina de Projeto de Desenvolvimento Backend — IBMEC

![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)
![Node.js](https://img.shields.io/badge/Node.js-18%2B-green)
![License](https://img.shields.io/badge/license-MIT-blue)

</div>

---

## Equipe

| Nome Completo | Matricula | GitHub |
|---|---|---|
| Igor Conrado Figueiredo Almeida | 202501008411 | [@igorconradoibmec](https://github.com/igorconradoibmec) |
| Joshua Azze Distel | 202501007181 | [@joshazze](https://github.com/joshazze) |
| Marcelo Benvindo Guimaraes Reis | 202501006361 | [@marceloxreis](https://github.com/marceloxreis) |
| Felipe de Miranda Cota Callado | 202301170711 | [@felipecota04](https://github.com/felipecota04) |

---

## Sobre o Projeto

A Bulbe Energia API e o backend do sistema BulbeShop, uma plataforma de e-commerce voltada para produtos de energia renovavel e dispositivos inteligentes para o lar. Esta API foi projetada para substituir a camada estatica do frontend (que utiliza `localStorage` e arquivos JSON) por uma arquitetura REST robusta, com autenticacao, validacao server-side e persistencia em banco de dados. O projeto foi desenvolvido como parte da disciplina de Projeto de Desenvolvimento Backend no IBMEC.

---

## Arquitetura

> *A ser preenchido na Sprint 2 apos definicao da arquitetura MVC.*

---

## Tecnologias

> *A ser preenchido na Sprint 2.*

---

## Como Executar Localmente

> *A ser preenchido na Sprint 2.*

---

## Endpoints da API (esboco inicial)

> Consulte o arquivo completo em [`docs/requisitos.md`](./docs/requisitos.md).

| Verbo  | Path                                | Descricao                                      |
|--------|-------------------------------------|-------------------------------------------------|
| GET    | /api/products                       | Listar todos os produtos                        |
| GET    | /api/products/{id}                  | Buscar produto por ID                           |
| GET    | /api/products/search?q={termo}      | Buscar produtos por texto                       |
| GET    | /api/products/featured              | Listar produtos em destaque                     |
| GET    | /api/products/black-friday          | Listar produtos Black Friday                    |
| GET    | /api/products/recommendations       | Obter recomendacoes de produtos                 |
| GET    | /api/cart                           | Obter carrinho do usuario                       |
| POST   | /api/cart/items                     | Adicionar item ao carrinho                      |
| PUT    | /api/cart/items/{itemId}            | Atualizar quantidade de item                    |
| DELETE | /api/cart/items/{itemId}            | Remover item do carrinho                        |
| DELETE | /api/cart                           | Limpar carrinho                                 |
| POST   | /api/orders                        | Criar pedido (finalizar compra)                 |
| GET    | /api/customers/{customerId}/orders  | Listar pedidos do usuario                       |
| GET    | /api/orders/{orderId}              | Buscar detalhes de um pedido                    |
| POST   | /api/coupons/validate              | Validar cupom de desconto                       |
| POST   | /api/users                         | Criar ou obter sessao de usuario                |

---

## Documentacao OpenAPI

> Arquivo em [`docs/openapi.yaml`](./docs/openapi.yaml) — a ser preenchido progressivamente.

---

## Estrutura do Repositorio

```
bulbe-energia-api-baal/
├── docs/
│   ├── requisitos.md
│   └── openapi.yaml
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   └── services/
├── tests/
├── .gitignore
├── package.json
└── README.md
```

---

## Sprints

| Sprint | Foco | Status |
|--------|------|--------|
| Kickoff | Apresentacao dos trabalhos do semestre anterior | Concluida |
| Sprint 1 | Setup + Elicitacao de Requisitos | Em andamento |
| Sprint 2 | Modelagem + Arquitetura + CRUD basico | Aguardando |
| Sprint 3 | Banco de Dados + ORM + Testes | Aguardando |
| Sprint 4 | Autenticacao + Documentacao Final | Aguardando |

---

## Referencias

- SOMMERVILLE, I. *Software Engineering*. 10. ed. Pearson, 2015.
- FOWLER, M. *Patterns of Enterprise Application Architecture*. Addison-Wesley, 2002.
- RICHARDSON, L.; RUBY, S. *RESTful Web Services*. O'Reilly, 2007.
- OpenAPI Initiative. *OpenAPI Specification v3.1.0*. Disponivel em: https://spec.openapis.org/oas/v3.1.0

---

## Licenca

Distribuido sob a licenca MIT. Consulte o arquivo [LICENSE](./LICENSE) para mais detalhes.
