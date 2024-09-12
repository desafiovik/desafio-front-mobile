# Desafio Frontend / Mobile

## **Sobre a VIK**

Somos um programa de saúde inovador voltado para empresas que veio para transformar o mundo corporativo. Com a utilização de gamificação e estímulos diários, a VIK traz uma abordagem envolvente que faz das atividades físicas uma parte divertida e natural do dia a dia.

https://vik.app

## **Problema:**

Desenvolver uma aplicação em Flutter e Angular consumindo dois CRUDs da nossa API.

No e-mail que recebeu do desafio enviamos um token para consumir nossa API juntamente com a URL da API.

## **Requisitos Flutter:**
- **Login**: O usuário deve ser capaz de realizar login. Utilize autenticação simples baseada em token.
- **Tela de Empresas**:
  - Listagem de empresas associadas a um cliente.
  - Criação de nova empresa (formulário com nome, endereço e site).
  - Edição de uma empresa existente.
  - Ativação/desativação da empresa.
- **Tela de Convites**:
  - Listagem de convites associados a uma empresa.
  - Criação de convite (escolher o tipo: e-mail, CPF, código).
  - Edição do convite.
  - Ativação/desativação do convite.
- **Extras**:
  - Gerenciamento de estado com Provider, Riverpod ou qualquer outro de sua preferência.
  - Boas práticas de código e organização em camadas (separação de UI, lógica de negócios e API).
  - Layout responsivo e usabilidade fluida.

**Entrega:**
- Código-fonte em um repositório público/privado no GitHub.
- Breve documentação sobre como rodar o projeto.

## **Requisitos Angular:**
- **Login**: O usuário deve ser capaz de realizar login. Utilize autenticação simples baseada em token.
- **Tela de Empresas**:
  - Listagem de empresas associadas aos clientes.
  - Criação, edição e desativação de empresas.
  - Mostrar mais detalhes (UUID, cliente associado).
- **Tela de Convites**:
  - Exibir convites para cada empresa, com filtros de tipo de convite.
  - Criar e editar convites.
- **Extras**:
  - Utilização de boas práticas de Angular (módulos, componentes e serviços).
  - Design responsivo com layout otimizado.
  - Integração de biblioteca de componentes visuais (como Angular Material).
  - Boas práticas de acessibilidade e performance.

## **Entrega:**

Crie o projeto suba em um repositório e nos envie o link do repositório para `frankyston.lins@vik.app`

PS1: Nossa API não tem o fluxo de login, use o que achar melhor, sugerimos Firebase.

PS2: Sinta-se a vontade para apresentar sugestões, práticas na qual você acredita serem melhores. ;)
