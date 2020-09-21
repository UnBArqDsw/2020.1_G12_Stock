# Brainstorming

Brainstorming é uma técnica que se aproveita de um grande [fluxo](Modeling/verbo?id=fluxo) de ideias sendo discutidas para que se encontre soluções criativas. A técnica, quando aplicada em grupo, permite que no momento em que um componente do grupo expõe uma ideia, esta possa ser complementada ou até mesmo substituída por outra que seja mais viável. É utilizado o princípio de que duas cabeças pensam melhor do que uma.

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 22/08/2020 | 1.0 | Realização do Brainstorming. | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor e Sofia Patrocínio |
| 31/08/2020 | 1.1 | Criação do documento baseado na gravação da reunião. | Pedro Igor |
| 09/09/2020 | 1.2 | Adição dos requisitos. | Gabriel Davi |
| 09/09/2020 | 1.3 | Adição do requisito RF08. | Pedro Igor |
| 11/09/2020 | 1.4 | Linkagem dos léxicos. | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 17/09/2020 | 1.5 | Adição do léxico de fluxo | Gabriel Davi |


## Metodologia

A técnica de brainstorming foi aplicada na primeira reunião em grupo. O foco da discussão foi determinar o escopo do projeto. A reunião foi gravada e posteriormente acompanhada anotando o [fluxo](Modeling/verbo?id=fluxo) de ideias discutido. Algumas ideias semelhantes ou complementares foram diluídas em uma única ideia.

### Elicitação de ideias

| Funcionalidade | Observação |
|:--------------:|:----------:|
| Gerar planilha | Permitir que o [usuário](Modeling/objeto?id=usuário) possa analisar o [estoque](Modeling/objeto?id=Estoque) [exportando](Modeling/verbo?id=Exportação) um documento no formato de uma planilha excel. |
| [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto) por planilhas | Permitir que [usuários](Modeling/objeto?id=usuário) possam realizar [cadastro](Modeling/verbo?id=Cadastrar-Produto) em lote [importando](Modeling/verbo?id=Importação) uma planilha excel. |
| [Consulta de estoque](Modeling/verbo?id=Consultar-Produto) | Visualizar a quantidade disponível de determinado [produto](Modeling/objeto?id=Produto). |
| [Adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao estoque | [Cadastrar](Modeling/verbo?id=Cadastrar-Produto) um novo [item](Modeling/objeto?id=Produto) com suas informações (descrição, nome, preço). |
| [Remoção de itens](Modeling/verbo?id=Baixa-em-Produto) ao [estoque](Modeling/objeto?id=Estoque). | [Dar baixa](Modeling/verbo?id=Baixa-em-Produto) em um [produto](Modeling/objeto?id=Produto) que foi vendido ou não se encontra mais disponível. |
| Adicionar [hierarquias(níveis) de acesso](Modeling/objeto?id=Papéis-dos-colaboradores) | Dar diferentes permissões para diferentes tipos de [usuário](Modeling/objeto?id=usuário) dentro de um mesmo negócio ([admin](Modeling/objeto?id=admin), [owner](Modeling/objeto?id=Owner), [seller](Modeling/objeto?id=Seller)). |
| Login | Um [usuário](Modeling/objeto?id=usuário) logar com sua conta independentemente da [hierarquia](Modeling/objeto?id=Papéis-dos-colaboradores). |
| Histórico de vendas | Gerar um histórico do que foi [removido](Modeling/verbo?id=Baixa-em-Produto) do [estoque](Modeling/objeto?id=Estoque), quem [removeu](Modeling/verbo?id=Baixa-em-Produto) e quando, etc.. |
| Históricos temporais | Escolher um período temporal para análise (diário, semanal, mensal). |
| [Tags](Modeling/objeto?id=Tag) nos [produtos](Modeling/objeto?id=Produto) | Adicionar [tags](Modeling/objeto?id=Tag) aos [produtos](Modeling/objeto?id=Produto) que permitem fazer uma [busca](Modeling/verbo?id=Consultar-Produto) por [tag](Modeling/objeto?id=Tag). |
| [Filtro por categoria](Modeling/verbo?id=Filtrar-Produtos) | [Usuários](Modeling/objeto?id=usuário) podem procurar por um [produto](Modeling/objeto?id=Produto) por meio de sua categoria. |

### Funcionalidades por [hierarquia]((Modeling/objeto?id=Papéis-dos-colaboradores))

Dentro da discussão foi levantada a possibilidade de determinar o acesso a funcionalidades diferentes a depender do nível dentro da [hierarquia](Modeling/objeto?id=Papéis-dos-colaboradores).

<div>

| Papel | Permissões |
|:-----:|:----------:|
| [Owner](Modeling/objeto?id=Owner) | Excluir contas.<br> Criar conta [admin](Modeling/objeto?id=Admin). |
| [Admin](Modeling/objeto?id=Admin) | Adicionar [produtos](Modeling/objeto?id=Produto) ao estoque.<br> Gerar planilhas.<br> Criar acesso [Seller](Modeling/objeto?id=Seller). |
| [Seller](Modeling/objeto?id=Seller) | [Dar baixa](Modeling/verbo?id=Baixa-em-Produto) no estoque. |

Obs: A [hierarquia](Modeling/objeto?id=Papéis-dos-colaboradores) é incremental de forma que um [papel](Modeling/objeto?id=Papéis-dos-colaboradores) superior tem todas as permissões inerentes ao seu papel e aos papeis inferiores.

</div>

## Requisitos levantados

| Id | Nome |
|:--:|:----:|
| [#RF01](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | Login |
| [#RF02](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [Hierarquia](Modeling/objeto?id=Papéis-dos-colaboradores) |
| [#RF03](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [Adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao  [estoque](Modeling/objeto?id=Estoque) |
| [#RF04](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [Consulta de estoque](Modeling/verbo?id=Consultar-Produto) |
| [#RF05](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [Filtro por categoria](Modeling/verbo?id=Filtrar-Produtos) |
| [#RF06](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [Tags](Modeling/objeto?id=Tag) em [produtos](Modeling/objeto?id=Produto) |
| [#RF07](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [Remoção de itens](Modeling/verbo?id=Baixa-em-Produto) do [estoque](Modeling/objeto?id=Estoque) |
| [#RF08](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto) por planilhas |
| [#RF09](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | Gerar planilha |
| [#RF10](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | Histórico de vendas |
| [#RF11](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | Histórico temporais |
| [#RF012](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [Filtro por nome e preço](Modeling/verbo?id=Filtrar-Produtos) |
| [#RF014](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | Plotagem de gráficos |
| [#RF015](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | Atualização instantânea de [estoque](Modeling/objeto?id=Estoque) |
| [#RF016](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais) | [Importação](Modeling/verbo?id=Importação) de planilha para [load de estoque](Modeling/verbo?id=Cadastrar-Produto) |

## Referências

- WOEBCKEN, Cayo. O que é brainstorming e as 7 melhores técnicas para a tomada de decisões inteligentes. [S. l.], 10 jul. 2019. Disponível em: <https://rockcontent.com/blog/brainstorming/>. Último acesso em: 31/08/2020.
- Wiki PAX App: <https://pax-app.github.io/Wiki/#/>. Último acesso em: 31/08/2020.
