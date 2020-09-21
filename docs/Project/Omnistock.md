# OmniStock

Com o desenvolvimento do projeto, o time notou que muitos membros não tinham familiaridade com o framework [React JS](https://pt-br.reactjs.org/). O membro Gabriel Davi já trabalha com esse framework há um tempo e se propôs a realizar um treinamento para os demais participantes, a fim de alinhar todo o time com a tecnologia. Apelidamos carinhosamente essa semana de treinamento de OmniStock, fazendo alusão às semanas de treinamento disponibilizadas pela [Rockeseat](https://rocketseat.com.br/).

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 20/09/2020 | 1.0 | Planejamento do treinamento. | Gabriel Davi |
| 21/09/2020 | 1.1 | Criação do documento e adição da explicação e link para o treinamento. | Micaella Gouveia |


## Metodologia
Ficou acordado que esse treinamento aconteceria durante a Semana Universitária, com duração de quatro dias. O membro Gabriel Davi planejou todas as aulas e o time preencheu um heatmap para definir o horário de cada encontro. Cada encontro terá duração de uma a duas horas, e conta com a presença de todos os membros.

## Planejamento
***Planejamento realizado pelo membro Gabriel Davi***

Será produzido na semana omniStock a aplicação "Stock Beta", que consiste em uma versão bem simplificada da aplicação Stock com o intuito de somente apresentar os principais conceitos de express e node com o ReactJS.

* Link para o protótipo (produzido com o [Figma](https://www.figma.com/)): 

[**https://www.figma.com/file/9NQvC0XBRNhA36afyeWJfS/Stock-Beta?node-id=0%3A1**](https://www.figma.com/file/9NQvC0XBRNhA36afyeWJfS/Stock-Beta?node-id=0%3A1)

## Dia 1 - Backend

### Conceitos NodeJS e Express

- [ ]  POST, GET, PUT/PATCH, DELETE
- [ ]  Request, Response
- [ ]  Rotas
- [ ]  Middlewares

### Backend do Stock beta

- [ ]  Configurar banco de dados
- [ ]  Configurar o sucrase
- [ ]  Configurar dotenv
- [ ]  Criar rotas
- [ ]  Criar Model de user
    - [ ]  Nome
    - [ ]  Email
    - [ ]  Senha
    - [ ]  Criar função de criptografia de senha
- [ ]  Criar Model de produtos
    - [ ]  Nome
    - [ ]  Preço
    - [ ]  Id da categoria
    - [ ]  Id do usuário
- [ ]  Criar Model de categoria
    - [ ]  Nome
    - [ ]  Descrição
    - [ ]  Id do usuário
- [ ]  Criar Controller de usuário
    - [ ]  Criação de um usuário
    - [ ]  Autenticação
- [ ]  Criar função para criação de token JWT
- [ ]  Criar middleware de autenticação JWT
- [ ]  Criar controller de produtos
    - [ ]  Listar produtos de um usuário logado (Popular as relações de usuário e de categoria)
    - [ ]  Criar um produto
    - [ ]  Editar um produto
    - [ ]  Deletar um produto

### Dia 2 - Frontend Stock Beta (Parte 1)

#### Conceitos fundamentais react

- [ ]  Estrutura de pastas
- [ ]  Estado
- [ ]  Hooks (useEffect, useState)
- [ ]  Ciclo de vida de um componente
- [ ]  Virtual DOM

#### Login/Cadastro de usuário

- [ ]  Página de login
    - [ ]  Campo de digitação de email
    - [ ]  Campo de digitação de senha
    - [ ]  Redirecionamento para a página principal
- [ ]  Página de cadastro
    - [ ]  Campo para digitar o nome
    - [ ]  Campo para digitar o email
    - [ ]  Campo para digitar a senha
    - [ ]  Campo para confirmar a senha
    - [ ]  Redirecionamento para a página de login

### Dia 3 - Frontend Stock Beta (Parte 2)

- [ ]  Configuração de rotas para a nossa aplicação
- [ ]  Criação do contexto para fluxo de autenticação
- [ ]  Configuração do fluxo de rotas e proteção de rotas (Só acessar determinadas rotas quando logado)
- [ ]  Criação da estrutura da página inicial (Hardcoded)

### Dia 4 - Frontend Stock Beta (Parte 3)

- [ ]  Implementação do modal de adicionar novo produto
- [ ]  Implementação do serviço para listagem dos produtos
- [ ]  Implementação do modal de editar um produto
- [ ]  Implementação do modal para adicionar nova categoria
- [ ]  Botão de logoff da aplicação (Redirecionar para o login)

## Referências
* Rockseat: <https://rocketseat.com.br> . Último acesso em 21/09/2020.
* React JS: <https://pt-br.reactjs.org> . Último acesso em 21/09/2020.
* Figma: <https://www.figma.com> . Último acesso em 21/09/2020.



