# OmniStock

Com o desenvolvimento do projeto, o time notou que muitos membros não tinham familiaridade com o framework [React JS](https://pt-br.reactjs.org/). O membro Gabriel Davi já trabalha com esse framework há um tempo e se propôs a realizar um treinamento para os demais participantes, a fim de alinhar todo o time com a tecnologia. Apelidamos carinhosamente essa semana de treinamento de OmniStock, fazendo alusão às semanas de treinamento disponibilizadas pela [Rockeseat](https://rocketseat.com.br/).

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 20/09/2020 | 1.0 | Planejamento do treinamento. | Gabriel Davi |
| 21/09/2020 | 1.1 | Criação do documento e adição da explicação e link para o treinamento. | Micaella Gouveia |
| 26/09/2020 | 1.2 | Adição dos vídeos do dia 1 e 2 | Sofia Patrocínio |
| 28/09/2020 | 1.3 | Adição dos vídeos do dia 3 e 4 e links para github | Micaella Gouveia |


## Metodologia
Ficou acordado que esse treinamento aconteceria durante a Semana Universitária, com duração de quatro dias. O membro Gabriel Davi planejou todas as aulas e o time preencheu um heatmap para definir o horário de cada encontro. Cada encontro terá duração de uma a duas horas, e conta com a presença de todos os membros.

| Dia | Data | Horário |
| - | - | - |
| 1 | Terça-feira (22/09/2020) | 14:00 |
| 2 | Quarta-feira (23/09/2020) | 16:00 |
| 3 | Sexta-feira (25/09/2020) | 22:00 |
| 4 | Sábado (26/08/2020) | 9:00 |

## Planejamento
***Planejamento realizado pelo membro Gabriel Davi***

Será produzido na semana OmniStock a aplicação "Stock Beta", que consiste em uma versão bem simplificada da aplicação Stock com o intuito de somente apresentar os principais conceitos de Express e NodeJS com o ReactJS.

* Link para o protótipo (produzido com o [Figma](https://www.figma.com/)): 

[**https://www.figma.com/file/9NQvC0XBRNhA36afyeWJfS/Stock-Beta?node-id=0%3A1**](https://www.figma.com/file/9NQvC0XBRNhA36afyeWJfS/Stock-Beta?node-id=0%3A1)

## Dia 1 - Backend

### Conceitos NodeJS e Express

- [x]  POST, GET, PUT/PATCH, DELETE
- [x]  Request, Response
- [x]  Rotas
- [x]  Middlewares

### Backend do Stock beta

- [x]  Configurar banco de dados
- [x]  Configurar o sucrase
- [x]  Configurar dotenv
- [x]  Criar rotas
- [x]  Criar Model de user
    - [x]  Nome
    - [x]  Email
    - [x]  Senha
    - [x]  Criar função de criptografia de senha
- [x]  Criar Model de produtos
    - [x]  Nome
    - [x]  Preço
    - [x]  Id da categoria
    - [x]  Id do usuário
- [x]  Criar Model de categoria
    - [x]  Nome
    - [x]  Descrição
    - [x]  Id do usuário
- [x]  Criar Controller de usuário
    - [x]  Criação de um usuário
    - [x]  Autenticação
- [x]  Criar função para criação de token JWT
- [x]  Criar middleware de autenticação JWT
- [x]  Criar controller de produtos
    - [x]  Listar produtos de um usuário logado (Popular as relações de usuário e de categoria)
    - [x]  Criar um produto
    - [x]  Editar um produto
    - [x]  Deletar um produto

## Gravações Disponíveis

<iframe allowFullScreen="allowFullScreen" src="https://www.youtube.com/embed/qFIssRB3Ag0?ecver=1&amp;iv_load_policy=1&amp;yt:stretch=16:9&amp;autohide=1&amp;color=red&amp;width=560&amp;width=560" width="560" height="315" allowtransparency="true" frameborder="0"><div><a  id="x4Kmoha6" href="https://www.rockpamperscissors.co.uk/a-new-one-on-me/">Emma hybrid</a></div><div><a  id="x4Kmoha6" href="https://www.earth-essentials.co.uk/is-buying-a-mattress-the-worst-thing-possible-for-your-health/">VOCs</a></div><script type="text/javascript">function execute_YTvideo(){return youtube.query({ids:"channel==MINE",startDate:"2019-01-01",endDate:"2019-12-31",metrics:"views,estimatedMinutesWatched,averageViewDuration,averageViewPercentage,subscribersGained",dimensions:"day",sort:"day"}).then(function(e){},function(e){console.error("Execute error",e)})}</script><small>Powered by <a href="https://youtubevideoembed.com/ ">Embed YouTube Video</a></small></iframe>

<iframe allowFullScreen="allowFullScreen" src="https://www.youtube.com/embed/BIOu52NfqZ0?ecver=1&amp;iv_load_policy=3&amp;yt:stretch=16:9&amp;autohide=1&amp;color=red&amp;width=560&amp;width=560" width="560" height="315" allowtransparency="true" frameborder="0"><div><a  id="x4Kmoha6" href="https://www.rockpamperscissors.co.uk/a-new-one-on-me/">Emma hybrid</a></div><div><a  id="x4Kmoha6" href="https://www.earth-essentials.co.uk/is-buying-a-mattress-the-worst-thing-possible-for-your-health/">VOCs</a></div><script type="text/javascript">function execute_YTvideo(){return youtube.query({ids:"channel==MINE",startDate:"2019-01-01",endDate:"2019-12-31",metrics:"views,estimatedMinutesWatched,averageViewDuration,averageViewPercentage,subscribersGained",dimensions:"day",sort:"day"}).then(function(e){},function(e){console.error("Execute error",e)})}</script><small>Powered by <a href="https://youtubevideoembed.com/ ">Embed YouTube Video</a></small></iframe>

### Dia 2 - Frontend Stock Beta (Parte 1)

#### Conceitos fundamentais react

- [x]  Estrutura de pastas
- [x]  Estado
- [x]  Hooks (useEffect, useState)
- [x]  Ciclo de vida de um componente
- [x]  Virtual DOM

#### Login/Cadastro de usuário

- [x]  Página de login
    - [x]  Campo de digitação de email
    - [x]  Campo de digitação de senha
    - [x]  Redirecionamento para a página principal
- [x]  Página de cadastro
    - [x]  Campo para digitar o nome
    - [x]  Campo para digitar o email
    - [x]  Campo para digitar a senha
    - [x]  Campo para confirmar a senha
    - [x]  Redirecionamento para a página de login

## Gravações Disponíveis

<iframe allowFullScreen="allowFullScreen" src="https://www.youtube.com/embed/DhmPSM8-2OM?ecver=1&amp;iv_load_policy=3&amp;yt:stretch=16:9&amp;autohide=1&amp;color=red&amp;width=560&amp;width=560" width="560" height="315" allowtransparency="true" frameborder="0"><div><a  id="x4Kmoha6" href="https://www.rockpamperscissors.co.uk/a-new-one-on-me/">Emma hybrid</a></div><div><a  id="x4Kmoha6" href="https://www.earth-essentials.co.uk/is-buying-a-mattress-the-worst-thing-possible-for-your-health/">VOCs</a></div><script type="text/javascript">function execute_YTvideo(){return youtube.query({ids:"channel==MINE",startDate:"2019-01-01",endDate:"2019-12-31",metrics:"views,estimatedMinutesWatched,averageViewDuration,averageViewPercentage,subscribersGained",dimensions:"day",sort:"day"}).then(function(e){},function(e){console.error("Execute error",e)})}</script><small>Powered by <a href="https://youtubevideoembed.com/ ">Embed YouTube Video</a></small></iframe>

### Dia 3 - Frontend Stock Beta (Parte 2)

- [x]  Configuração de rotas para a nossa aplicação
- [x]  Criação do contexto para fluxo de autenticação
- [x]  Configuração do fluxo de rotas e proteção de rotas (Só acessar determinadas rotas quando logado)
- [x]  Criação da estrutura da página inicial (Hardcoded)

## Gravações Disponíveis

<iframe allowFullScreen="allowFullScreen" src="https://www.youtube.com/embed/l7c2Gbf2b-c?ecver=1&amp;iv_load_policy=3&amp;yt:stretch=16:9&amp;autohide=1&amp;color=red&amp;width=560&amp;width=560" width="560" height="315" allowtransparency="true" frameborder="0"><div><a  id="x4Kmoha6" href="https://www.rockpamperscissors.co.uk/a-new-one-on-me/">Emma hybrid</a></div><div><a  id="x4Kmoha6" href="https://www.earth-essentials.co.uk/is-buying-a-mattress-the-worst-thing-possible-for-your-health/">VOCs</a></div><script type="text/javascript">function execute_YTvideo(){return youtube.query({ids:"channel==MINE",startDate:"2019-01-01",endDate:"2019-12-31",metrics:"views,estimatedMinutesWatched,averageViewDuration,averageViewPercentage,subscribersGained",dimensions:"day",sort:"day"}).then(function(e){},function(e){console.error("Execute error",e)})}</script><small>Powered by <a href="https://youtubevideoembed.com/ ">Embed YouTube Video</a></small></iframe>

<iframe allowFullScreen="allowFullScreen" src="https://www.youtube.com/embed/Cm8H3CsnJwI?ecver=1&amp;iv_load_policy=3&amp;yt:stretch=16:9&amp;autohide=1&amp;color=red&amp;width=560&amp;width=560" width="560" height="315" allowtransparency="true" frameborder="0"><div><a  id="x4Kmoha6" href="https://www.rockpamperscissors.co.uk/a-new-one-on-me/">Emma hybrid</a></div><div><a  id="x4Kmoha6" href="https://www.earth-essentials.co.uk/is-buying-a-mattress-the-worst-thing-possible-for-your-health/">VOCs</a></div><script type="text/javascript">function execute_YTvideo(){return youtube.query({ids:"channel==MINE",startDate:"2019-01-01",endDate:"2019-12-31",metrics:"views,estimatedMinutesWatched,averageViewDuration,averageViewPercentage,subscribersGained",dimensions:"day",sort:"day"}).then(function(e){},function(e){console.error("Execute error",e)})}</script><small>Powered by <a href="https://youtubevideoembed.com/ ">Embed YouTube Video</a></small></iframe>

### Dia 4 - Frontend Stock Beta (Parte 3)

- [x]  Implementação do modal de adicionar novo produto
- [x]  Implementação do serviço para listagem dos produtos
- [x]  Implementação do modal de editar um produto
- [x]  Implementação do modal para adicionar nova categoria
- [x]  Botão de logoff da aplicação (Redirecionar para o login)

## Gravações Disponíveis

<iframe allowFullScreen="allowFullScreen" src="https://www.youtube.com/embed/mQCKdZBs0WA?ecver=1&amp;iv_load_policy=3&amp;yt:stretch=16:9&amp;autohide=1&amp;color=red&amp;width=560&amp;width=560" width="560" height="315" allowtransparency="true" frameborder="0"><div><a  id="x4Kmoha6" href="https://www.rockpamperscissors.co.uk/a-new-one-on-me/">Emma hybrid</a></div><div><a  id="x4Kmoha6" href="https://www.earth-essentials.co.uk/is-buying-a-mattress-the-worst-thing-possible-for-your-health/">VOCs</a></div><script type="text/javascript">function execute_YTvideo(){return youtube.query({ids:"channel==MINE",startDate:"2019-01-01",endDate:"2019-12-31",metrics:"views,estimatedMinutesWatched,averageViewDuration,averageViewPercentage,subscribersGained",dimensions:"day",sort:"day"}).then(function(e){},function(e){console.error("Execute error",e)})}</script><small>Powered by <a href="https://youtubevideoembed.com/ ">Embed YouTube Video</a></small></iframe>

<iframe allowFullScreen="allowFullScreen" src="https://www.youtube.com/embed/Mn0yXY-y4C4?ecver=1&amp;iv_load_policy=3&amp;yt:stretch=16:9&amp;autohide=1&amp;color=red&amp;width=560&amp;width=560" width="560" height="315" allowtransparency="true" frameborder="0"><div><a  id="x4Kmoha6" href="https://www.rockpamperscissors.co.uk/a-new-one-on-me/">Emma hybrid</a></div><div><a  id="x4Kmoha6" href="https://www.earth-essentials.co.uk/is-buying-a-mattress-the-worst-thing-possible-for-your-health/">VOCs</a></div><script type="text/javascript">function execute_YTvideo(){return youtube.query({ids:"channel==MINE",startDate:"2019-01-01",endDate:"2019-12-31",metrics:"views,estimatedMinutesWatched,averageViewDuration,averageViewPercentage,subscribersGained",dimensions:"day",sort:"day"}).then(function(e){},function(e){console.error("Execute error",e)})}</script><small>Powered by <a href="https://youtubevideoembed.com/ ">Embed YouTube Video</a></small></iframe>

## Repositórios produzidos na Semana OmniStock
* Gabriel Davi:
    * [Backend](https://github.com/GabrielDVpereira/StockBeta-backend)
    * [Frontend](https://github.com/GabrielDVpereira/StockBeta-web)

* Micaella Gouveia:
    * [Backend](https://github.com/micaellagouveia/dojoReact)
    * [Frontend](https://github.com/micaellagouveia/stockBetaFront)

* Sofia Patrocínio:
    * [Backend](https://github.com/sofiapatrocinio/SemanaOmniStock/tree/master/src)
    * [Frontend](https://github.com/sofiapatrocinio/SemanaOmniStock/tree/master/front)

## Referências
* Rockseat: <https://rocketseat.com.br> . Último acesso em 21/09/2020.
* React JS: <https://pt-br.reactjs.org> . Último acesso em 21/09/2020.
* Figma: <https://www.figma.com> . Último acesso em 21/09/2020.



