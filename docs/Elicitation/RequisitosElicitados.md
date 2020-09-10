# Requisitos Elicitados

Ao longo do projeto são utilizadas diversas técnicas para aprofundamento do domínio do público alvo e definição de requisitos que serão úteis, posteriormente, na construção de funcionalidades dentro da aplicação.<br>
Os requisitos apresentados a seguir estão baseados nos documentos: Brainstorming, Entrevista, Questionário e StoryBoard elaborados em sprints anteriores. Outros requisitos serão inseridos a medida que outras técnicas sejam realizadas.<br>

## Histórico de Revisões

|    Data    | Versão |                                     Descrição                                      |  Autor(es)   |
| :--------: | :----: | :--------------------------------------------------------------------------------: | :----------: |
| 07/09/2020 |  1.0   |        Adição de requisitos funcionais baseados na técnica de Brainstorming        |  Pedro Igor  |
| 07/09/2020 |  1.1   | Adição de requisitos funcionais e não funcionais baseados na técnica de StoryBoard |  Pedro Igor  |
| 07/09/2020 |  1.2   |       Adição de requisitos não funcionais baseados na técnica de Entrevista.       |  Pedro Igor  |
| 07/09/2020 |  1.3   |                         Adição de requisitos RF17 E RF18.                          | Gabriel Davi |
| 09/09/2020 |  1.4   |                         Edição do requisito RF9 e adição de requisito RF21.                                  | Sofia Patrocínio |

## Requisitos Funcionais

|                    Nome                     |    ID    |                                                    Descrição                                                    |    Pré-Condições    | Backword From |
| :-----------------------------------------: | :------: | :-------------------------------------------------------------------------------------------------------------: | :-----------------: | :-------- : |
|                    Login                    | **RF01** |                         O sistema deve permitir que o usuário faça login em sua conta.                          |         N/A         | Brainstorming |
|                 Hierarquia                  | **RF02** |                           O sistema deve permitir que sejam adicionadas hierarquias.                            |      **RF01**       | Brainstorming |
|         Adição de itens ao estoque          | **RF03** |                         O sistema deve permitir que itens sejam cadastrados no estoque.                         | **RF01** e **RF02** | Brainstorming, StoryBoard, Entrevista |
|             Consulta de estoque             | **RF04** |                         O sistema deve permitir que o usuário faça consulta no estoque.                         |      **RF03**       | Brainstorming, StoryBoard, Entrevista |
|            Filtro por categoria             | **RF05** |                       O sistema deve permitir que filtros sejam utilizados nas consultas.                       |      **RF04**       | Brainstorming, StoryBoard, Entrevista |
|              Tags nos produtos              | **RF06** |                     O sistema deve permitir sejam adicionadas tags ao cadastrar um produto.                     |      **RF03**       | Brainstorming |
|         Remoção de itens do estoque         | **RF07** |                                O sistema deve permitir remover itens do estoque.                                |      **RF03**       | Brainstorming, Entrevista |
|      Cadastrar produtos por planilhas       | **RF08** |           O sistema deve permitir que cadastros em lote sejam feitos enviando documentos de planilhas.           |      **RF03**       | Brainstorming |
|               Gerar planilha                | **RF09** |      O sistema deve permitir que sejam exportados documentos de planilha com informações sobre o estoque.       |      **RF04**       | Brainstorming, Entrevista e StoryBoard |
|             Histórico de vendas             | **RF10** |                O sistema deve gerar um log de registro de remoção e adição de itens ao estoque.                | **RF03** e **RF07** | Brainstorming, Entrevista |
|             Histórico temporais             | **RF11** | O sistema deve permitir consultar registros demarcados por períodos temporais. (diário, semanal, mensal, anual) |      **RF10**       | Brainstorming |
|           Filtro por nome e preço           | **RF12** |                        O sistema dever permitir filtrar produtos pelo nome e por preço.                         |      **RF04**       | Brainstorming, StoryBoard, Entrevista |
|               Filtro por data               | **RF13** |                                O sistema deve permitir filtrar itens pela data.                                 |      **RF04**       | StoryBoard |
|            Plotagem de gráficos             | **RF14** |                           O sistema deve gerar gráficos baseados no fluxo do estoque.                           |      **RF04**       | Brainstorming, StoryBoard, Entrevista |
|     Atualização instantânea de estoque      | **RF15** |        O sistema deve ser capaz de atualizar a base de dados no momento em que uma operação é realizada.        | **RF03** e **RF07** |  StoryBoard, Entrevista |
| Importação de planilha para load de estoque | **RF16** |    O sistema deve ser capaz de importar uma planilha que irá carregar o estoque com os produtos da planilha     |          N/A          | Brainstorming, Entrevista |
|     App para consulta fácil de produtos     | **RF17** |       Possuir uma aplicação PWA que funcione somente com acesso a internet para busca rápida de produtos        |          N/A          | StoryBoard, Entrevista |
|      App para baixa fácil de produtos       | **RF18** |      Possuir uma aplicação PWA que funcione somente com acesso a internet para remoção rápida de produtos       |          N/A          | StoryBoard |
<<<<<<< HEAD
|      Notificação de prazo de vencimento      | **RF21** |      O sistema deve notificar o usuário na data próxima ao prazo de vencimento do produto       |         **RF03**          | StoryBoard |
=======
|      Delimitar quantidade mínima de um produto       | **RF19** |      O usuário deve ser capaz de  delimitar uma quantidade mínima de um produto.      |          **RF03**          | Entrevista |
|      Alertar sobre quantidade mínima atingida      | **RF20** |      O sistema deve ser capaz de alertar o usuário quando um produto ultrapassar o limite mínimo de quantidade.      |          **RF03** e **RF19**         | Entrevista |

>>>>>>> aa159edff3b64060e63f6af7322d386a7824a8fd

## Requisitos Não Funcionais

|        Nome         |    ID     |                                                  Descrição                                                  | Pré-Condições | Backward From |
| :-----------------: | :-------: | :---------------------------------------------------------------------------------------------------------: | :-----------: | :-----: |
| Rapidez na consulta | **RNF01** |               O sistema deve retornar o resultado de uma consulta quase que instantaneamente.               |   **RF04**    | StoryBoard, Entrevista |
| Gráficos didáticos  | **RNF02** |  O sistema deve garantir que os gráficos plotados são abrangentes em detalhes porém de fácil entendimento.  |   **RF14**    | StoryBoard, Entrevista |
|  Consultas remotas  | **RNF03** | O sistema deve ser capaz de ser consultado remotamente. (longe do local físico de armazenamento do estoque) |   **RF04**    | Entrevista, StoryBoard, Entrevista |