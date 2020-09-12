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
|             Gerar planilha              |   Permitir que o [usuário](../Modeling/objeto?id=usuário) possa analisar o [estoque](../Modeling/objeto?id=Estoque) exportando um documento no formato de uma planilha excel.   |
|    [cadastrar produto](../Modeling/verbo?id=cadastrar-produto) por planilhas     |             Permitir que [usuário](../Modeling/objeto?id=usuário) possam realizar cadastro em lote importando uma planilha excel.             |
|           Consulta de [estoque](../Modeling/objeto?id=Estoque)           |                          Visualizar a quantidade disponível de determinado [produto](../Modeling/objeto?id=produto).                           |
|       Adição de itens ao [estoque](../Modeling/objeto?id=Estoque)        |                     Cadastrar um novo item com suas informações (descrição, nome, preço).                     |
|      Remoção de itens ao [estoque](../Modeling/objeto?id=Estoque).       |                  Dar [baixa em produto](../Modeling/verbo?id=baixa-em-produto) que foi vendido ou não se encontra mais disponível.                  |
| Adicionar hierarquias(níveis) de acesso | Dar diferentes permissões para diferentes tipos de [usuário](../Modeling/objeto?id=usuário) dentro de um mesmo negócio ([admin](../Modeling/objeto?id=Admin), [owner](../Modeling/objeto?id=Owner), [seller](../Modeling/objeto?id=Seller)). |
|                  Login                  |                        Um [usuário](../Modeling/objeto?id=usuário) logar com sua conta independentemente da hierarquia.                        |
|           Histórico de vendas           |                Gerar um histórico do que foi removido do [estoque](../Modeling/objeto?id=Estoque), quem removeu e quando, etc..                |
|          Históricos temporais           |                     Escolher um período temporal para análise (diário, semanal, mensal).                      |
|            Tags nos [produtos](../Modeling/objeto?id=produto)            |                       Adicionar tags aos [produtos](../Modeling/objeto?id=produto) que permitem fazer uma busca por tag.                       |
|          Filtro por categoria           |                       [usuário](../Modeling/objeto?id=usuário) podem procurar por um [produtos](../Modeling/objeto?id=produto) por meio de sua categoria.                       |

### Funcionalidades por hierarquia

Dentro da discussão foi levantada a possibilidade de determinar o acesso a funcionalidades diferentes a depender do nível dentro da hierarquia.

<div>

| Papel  |                                     Permissões                                      |
| :----: | :---------------------------------------------------------------------------------: |
| [Owner](../Modeling/objeto?id=Owner)  |                     _ Excluir contas.<br> _ Criar conta [Admin](../Modeling/objeto?id=Admin).                      |
| Admin  | _ Adicionar [produtos](../Modeling/objeto?id=produto) ao estoque.<br> _ Gerar planilhas.<br> \* Criar acesso [Seller](../Modeling/objeto?id=Seller). |
| [Seller](../Modeling/objeto?id=Seller) |                              \* Dar baixa no [estoque](../Modeling/objeto?id=Estoque).                               |

Obs: A hierarquia é incremental de forma que um papel superior tem todas as permissões inerentes ao seu papel e aos papeis inferiores.

</div>

## Requisitos levantados

|                                   Id                                   |                    Nome                     |
| :--------------------------------------------------------------------: | :-----------------------------------------: |
| [#RF01](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |                    Login                    |
| [#RF02](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |                 Hierarquia                  |
| [#RF03](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |         Adição de itens ao [estoque](../Modeling/objeto?id=Estoque)          |
| [#RF04](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |             Consulta de [estoque](../Modeling/objeto?id=Estoque)             |
| [#RF05](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |            Filtro por categoria             |
| [#RF06](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |              Tags em [produtos](../Modeling/objeto?id=produto)               |
| [#RF07](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |         Remoção de itens do [estoque](../Modeling/objeto?id=Estoque)         |
| [#RF08](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |               [cadastrar produto](../Modeling/verbo?id=cadastrar-produto) por planilhas               |
| [#RF09](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |               Gerar planilha                |
| [#RF10](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |             Histórico de vendas             |
| [#RF11](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  |             Histórico temporais             |
| [#RF012](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) |           Filtro por nome e preço           |
| [#RF014](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) |            Plotagem de gráficos             |
| [#RF015](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) |     Atualização instantânea de [estoque](../Modeling/objeto?id=Estoque)      |
| [#RF016](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [importação](../Modeling/verbo?id=importação) de planilha para load de [estoque](../Modeling/objeto?id=Estoque) |

## Referências

- WOEBCKEN, Cayo. O que é brainstorming e as 7 melhores técnicas para a tomada de decisões inteligentes. [S. l.], 10 jul. 2019. Disponível em: <https://rockcontent.com/blog/brainstorming/>. Último acesso em: 31/08/2020.
- Wiki PAX App - Grupo de Desenho de Software do semestre 2019/2 - Disponível em: <https://pax-app.github.io/Wiki/#/>. Último acesso em: 31/08/2020
