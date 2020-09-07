# Requisitos Elicitados

Ao longo do projeto são utilizadas diversas técnicas para aprofundamento do domínio do público alvo e definição de requisitos que serão úteis, posteriormente, na construção de funcionalidades dentro da aplicação.<br>
Os requisitos apresentados a seguir estão baseados nos documentos: Brainstorming, Entrevista, Questionário e StoryBoard elaborados em sprints anteriores. Outros requisitos serão inseridos a medida que outras técnicas sejam realizadas.<br>

## Histórico de Revisões
|    Data    | Versão |         Descrição         |           Autor(es)            |
| :--------: | :----: | :-----------------------: | :----------------------------: |
| 07/08/2020 |  1.0   | Adição de requisitos funcionais elicitados na técnica de Brainstorming | Pedro Igor |

## Requisitos Funcionais
|    Nome   |  ID | Descrição |          Pré-Condições       |
| :-------: | :--:| :-------: | :--------------------------: |
| Login   | **RF01** | O sistema deve permitir que o usuário faça login em sua conta. | N/A |
| Hierarquia | **RF02** | O sistema deve permitir que sejam adicionadas hierarquias. | **RF01** |
| Adição de itens ao estoque | **RF03** | O sistema deve permitir que itens sejam cadastrados no estoque. | **RF01** e **RF02**|
| Consulta de estoque | **RF04** | O sistema deve permitir que o usuário faça consulta no estoque. | **RF03** |
| Filtro por categoria | **RF05** | O sistema deve permitir que filtros sejam utilizados nas consultas. | **RF04** |
| Tags nos produtos | **RF06** | O sistema deve permitir sejam adicionadas tags ao cadastrar um produto. | **RF03** |
| Remoção de itens do estoque | **RF07** | O sistema deve permitir remover itens do estoque. | **RF03** |
| Cadastrar produtos por planilhas | **RF08** | O sistema deve permitir que cadastros em lote sejam feito enviando documentos de planilhas. | **RF03** |
| Gerar planilha | **RF09** | O sistema deve permitir que sejam exportados documentos de planilha com informações sobre o estoque. | **RF04** |
| Histórico de vendas | **RF10** | O sistema deve gerar um log de registro de remoções e adição de itens ao estoque. | **RF03** e **RF07** |
| Histórico temporais | **RF11** | O sistema deve permitir consultar registros demarcados por períodos temporais. (diário, semanal, mensal, anual) | **RF10**|