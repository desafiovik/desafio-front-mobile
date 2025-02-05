# Desafio Frontend / Mobile

## **Sobre a VIK**

Somos um programa de saúde inovador voltado para empresas que veio para transformar o mundo corporativo. Com a utilização de gamificação e estímulos diários, a VIK traz uma abordagem envolvente que faz das atividades físicas uma parte divertida e natural do dia a dia.

https://vik.app

## **Problema:**

Desenvolver uma aplicação em Flutter consumindo dois CRUDs da nossa API.

No e-mail que recebeu do desafio enviamos um token para consumir nossa API juntamente com a URL da API.



---

## Sumário

- [Introdução](#introdução)
- [Funcionalidades](#funcionalidades)
- [Requisitos do Projeto](#requisitos-do-projeto)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Rotas da API](#rotas-da-api)
- [Entrega](#entrega)

---

## Introdução


Este projeto é um aplicativo Flutter que tem como objetivo gerenciar empresas e convites. Nele, você encontrará:

- **Autenticação por token:** Acesso seguro ao sistema.
- **Tela de Empresas:** Listagem, cadastro, edição e ativação/desativação de empresas.
- **Tela de Convites:** Listagem, cadastro, edição e ativação/desativação de convites.
- **Gerenciamento de Estado:** Utilização de Provider, Riverpod ou outra solução para manter a consistência dos dados.
- **Organização em Camadas:** Separação clara entre UI, lógica de negócios e API.
- **Layout Responsivo:** Interface adaptável a diferentes tamanhos de tela.

---

## Funcionalidades

### Autenticação
- **Login:** Permite que o usuário realize o login utilizando autenticação baseada em token.

### Empresas
- **Listagem:** Exibe todas as empresas associadas ao cliente.
- **Cadastro:** Formulário para inclusão de nova empresa com campos para nome, endereço e site.
- **Edição:** Permite alterar os dados de uma empresa existente.
- **Ativação/Desativação:** Alterna o status de uma empresa.

### Convites
- **Listagem:** Exibe convites associados a uma empresa.
- **Cadastro:** Permite a criação de convites com a escolha do tipo (e-mail, CPF ou código).
- **Edição:** Permite modificar os dados de um convite existente.
- **Ativação/Desativação:** Alterna o status de um convite.

---

## Requisitos do Projeto

- **Autenticação com Token:** Implementar autenticação simples para acesso ao aplicativo.
- **Gerenciamento de Estado:** Utilizar um gerenciador de estado (Provider, Riverpod ou similar) para atualizar a interface conforme os dados.
- **Organização em Camadas:**
  - **UI:** Widgets e componentes de interface.
  - **Lógica de Negócios:** Regras e fluxos da aplicação.
  - **API:** Comunicação com o backend para autenticação e CRUD.
- **Responsividade:** Layout adaptável a diferentes dispositivos.
- **Boas Práticas:** Código limpo, modular e aderente aos princípios SOLID.

---

## Tecnologias Utilizadas

- **Flutter** e **Dart**
- **Gerenciamento de Estado:** Provider, Riverpod ou outra opção similar
- **HTTP/REST API:** Para autenticação e operações CRUD
- **Pacotes Adicionais:** 
  - `flutter_secure_storage` – Armazenamento seguro do token
  - `http` ou `dio` – Requisições à API

---

## Rotas da API

### Autenticação
- **Login**
  - **Método:** POST  
  - **Endpoint:** `/api/v1/login`  
  - **Descrição:** Autentica o usuário e retorna um token.

### Empresas
- **Listagem:**  
  - **Método:** GET  
  - **Endpoint:** `/api/v1/companies`  
  - **Descrição:** Retorna todas as empresas associadas ao cliente.
- **Cadastro:**  
  - **Método:** POST  
  - **Endpoint:** `/api/v1/companies`  
  - **Parâmetros:** `nome` (string), `endereco` (string), `site` (string)  
  - **Descrição:** Cria uma nova empresa.
- **Detalhes:**  
  - **Método:** GET  
  - **Endpoint:** `/api/v1/companies/:id`  
  - **Descrição:** Exibe detalhes de uma empresa específica.
- **Atualização:**  
  - **Método:** PUT/PATCH  
  - **Endpoint:** `/api/v1/companies/:id`  
  - **Descrição:** Atualiza os dados de uma empresa.
- **Exclusão:**  
  - **Método:** DELETE  
  - **Endpoint:** `/api/v1/companies/:id`  
  - **Descrição:** Remove uma empresa.

### Convites
- **Listagem:**  
  - **Método:** GET  
  - **Endpoint:** `/api/v1/companies/:company_id/invites`  
  - **Descrição:** Retorna os convites de uma empresa.
- **Cadastro:**  
  - **Método:** POST  
  - **Endpoint:** `/api/v1/companies/:company_id/invites`  
  - **Parâmetros:** `tipo` (string – valores: "e-mail", "CPF" ou "código")  
  - **Descrição:** Cria um novo convite.
- **Detalhes:**  
  - **Método:** GET  
  - **Endpoint:** `/api/v1/companies/:company_id/invites/:id`  
  - **Descrição:** Exibe detalhes de um convite.
- **Atualização:**  
  - **Método:** PUT/PATCH  
  - **Endpoint:** `/api/v1/companies/:company_id/invites/:id`  
  - **Descrição:** Atualiza um convite.
- **Exclusão:**  
  - **Método:** DELETE  
  - **Endpoint:** `/api/v1/companies/:company_id/invites/:id`  
  - **Descrição:** Remove um convite.

---



## **Entrega:**

Crie o projeto suba em um repositório e nos envie o link do repositório para `lucas.rodrigues@vik.app`

PS1: Nossa API não tem o fluxo de login, use o que achar melhor.

PS2: Sinta-se a vontade para apresentar sugestões, práticas na qual você acredita serem melhores. ;)
