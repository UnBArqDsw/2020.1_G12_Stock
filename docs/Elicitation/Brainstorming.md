# Brainstorming

Brainstorming é uma técnica que se aproveita de um grande fluxo de ideias sendo discutidas para que se encontre soluções criativas. A técnica, quando aplicada em grupo, permite que no momento em que um componente do grupo expõe uma ideia, esta possa ser complementada ou até mesmo substituída por outra que seja mais viável. É utilizado o princípio de que duas cabeças pensam melhor do que uma.

## Histórico de Revisões

|    Data    | Versão |                      Descrição                       | Autor(es)  |
| :--------: | :----: | :--------------------------------------------------: | :--------: |
| 31/08/2020 |  1.0   | Criação do documento baseado na gravação da reunião. | Pedro Igor |
| 09/09/2020 |  1.1   | Adição dos requisitos. | Gabriel Davi |
| 09/09/2020 | 1.1.1 | Adição do requisito RF08. | Pedro Igor |


## Metodologia

A técnica de brainstorming foi aplicada na primeira reunião em grupo. O foco da discussão foi determinar o escopo do projeto. A reunião foi gravada e posteriormente acompanhada anotando o fluxo de ideias discutido. Algumas ideias semelhantes ou complementares foram diluídas em uma única ideia.

### Elicitação de ideias

|             Funcionalidade              |                                                  Observação                                                   |
| :-------------------------------------: | :-----------------------------------------------------------------------------------------------------------: |
|             Gerar planilha              |   Permitir que o usuário possa analisar o estoque exportando um documento no formato de uma planilha excel.   |
|    Cadastrar produtos por planilhas     |             Permitir que usuários possam realizar cadastro em lote importando uma planilha excel.             |
|           Consulta de estoque           |                          Visualizar a quantidade disponível de determinado produto.                           |
|       Adição de itens ao estoque        |                     Cadastrar um novo item com suas informações (descrição, nome, preço).                     |
|      Remoção de itens ao estoque.       |                  Dar baixa em um produto que foi vendido ou não se encontra mais disponível.                  |
| Adicionar hierarquias(níveis) de acesso | Dar diferentes permissões para diferentes tipos de usuário dentro de um mesmo negócio (admin, owner, seller). |
|                  Login                  |                        Um usuário logar com sua conta independentemente da hierarquia.                        |
|           Histórico de vendas           |                Gerar um histórico do que foi removido do estoque, quem removeu e quando, etc..                |
|          Históricos temporais           |                     Escolher um período temporal para análise (diário, semanal, mensal).                      |
|            Tags nos produtos            |                       Adicionar tags aos produtos que permitem fazer uma busca por tag.                       |
|          Filtro por categoria           |                       Usuários podem procurar por um produto por meio de sua categoria.                       |

### Funcionalidades por hierarquia

Dentro da discussão foi levantada a possibilidade de determinar o acesso a funcionalidades diferentes a depender do nível dentro da hierarquia.

<div>

| Papel  |                                     Permissões                                      |
| :----: | :---------------------------------------------------------------------------------: |
| Owner  |                     _ Excluir contas.<br> _ Criar conta Admin.                      |
| Admin  | _ Adicionar produtos ao estoque.<br> _ Gerar planilhas.<br> \* Criar acesso Seller. |
| Seller |                              \* Dar baixa no estoque.                               |

Obs: A hierarquia é incremental de forma que um papel superior tem todas as permissões inerentes ao seu papel e aos papeis inferiores.

</div>

## Requisitos levantados

|                                   Id                                   |                    Nome                     |
| :--------------------------------------------------------------------: | :-----------------------------------------: |
| [#RF01](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |                    Login                    |
| [#RF02](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |                 Hierarquia                  |
| [#RF03](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |         Adição de itens ao estoque          |
| [#RF04](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |             Consulta de estoque             |
| [#RF05](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |            Filtro por categoria             |
| [#RF06](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |              Tags em produtos               |
| [#RF07](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |         Remoção de itens do estoque         |
| [#RF08](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |               Cadastrar produtos por planilhas               |
| [#RF09](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |               Gerar planilha                |
| [#RF10](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |             Histórico de vendas             |
| [#RF11](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |             Histórico temporais             |
| [#RF012](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) |           Filtro por nome e preço           |
| [#RF014](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) |            Plotagem de gráficos             |
| [#RF015](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) |     Atualização instantânea de estoque      |
| [#RF016](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | Importação de planilha para load de estoque |

## Referências

- WOEBCKEN, Cayo. O que é brainstorming e as 7 melhores técnicas para a tomada de decisões inteligentes. [S. l.], 10 jul. 2019. Disponível em: <https://rockcontent.com/blog/brainstorming/>. Último acesso em: 31/08/2020.
- Wiki PAX App - Grupo de Desenho de Software do semestre 2019/2 - Disponível em: <https://pax-app.github.io/Wiki/#/>. Último acesso em: 31/08/2020
