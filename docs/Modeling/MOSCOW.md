# MoSCoW

O método MoSCoW é uma técnica de priorização usada na gestão como um todo, principalmente na gestão de projetos e desenvolvimento de softwares com o intuito de encontrar um entendimento em comum entre as partes interessadas sobre a importância que elas atribuem a cada requisito.

O termo MoSCoW é um acrônimo em inglês derivado da primeira letra de cada uma das quatro categorias. Sua priorização é definida da seguinte forma:

1. **Must** (Tenho que fazer)
2. **Should** (Devo fazer)
3. **Could** (Poderia fazer)
4. **Won’t** (Não vou fazer)


## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 18/09/2020 | 1.0 | Priorização MoSCoW. | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 18/09/2020 | 1.1 | Criação do documento e adição da tabela. | Sofia Patrocínio |
| 19/09/2020 | 1.2 | Adição da introdução e priorização dos requisitos 26 a 33.| Micaella Gouveia |

## MoSCoW
Essa técnica é utilizada para priorizar os requisitos funcionais elicitados, então segue abaixo os requisitos com as suas devidas priorizações.


| Nome | ID | Descrição | Prioridade |
|------|----|-----------|---------------|
| Login | **RF01** | O sistema deve permitir que o [usuário](Modeling/objeto?id=usuário) faça login em sua conta. | Must |
| [Hierarquia](Modeling/objeto?id=Papéis-dos-colaboradores) | **RF02** | O sistema deve permitir que sejam adicionadas [hierarquias](Modeling/objeto?id=Papéis-dos-colaboradores). | Should |
| [Adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao [estoque](Modeling/objeto?id=Estoque) | **RF03** | O sistema deve permitir que itens sejam [cadastrados](Modeling/verbo?id=Cadastrar-Produto) no [estoque](Modeling/objeto?id=Estoque). | Must |
| [Consulta de estoque](Modeling/verbo?id=Consultar-Produto) | **RF04** | O sistema deve permitir que o [usuário](Modeling/objeto?id=usuário) faça [consulta no estoque](Modeling/verbo?id=Consultar-Produto). | Must |
| [Filtro por categoria](Modeling/verbo?id=Filtrar-Produtos) | **RF05** | O sistema deve permitir que [filtros](Modeling/verbo?id=Filtrar-Produtos) sejam utilizados nas [consultas](<(Modeling/verbo?id=Consultar-Produto)>). | Could |
| [Tags](Modeling/objeto?id=Tag) nos [produtos](Modeling/objeto?id=Produto) | **RF06** | O sistema deve permitir sejam adicionadas [tags](Modeling/objeto?id=Tag) ao cadastrar um [produtos](Modeling/objeto?id=Produto). | Should |
| [Remoção de itens](Modeling/verbo?id=Baixa-em-Produto) do [estoque](Modeling/objeto?id=Estoque) | **RF07** | O sistema deve permitir [remover](Modeling/verbo?id=Baixa-em-Produto) itens do [estoque](Modeling/objeto?id=Estoque). | Must |
| [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto) por planilhas | **RF08** | O sistema deve permitir que cadastros em lote sejam feitos enviando documentos de planilhas. | Could |
| Gerar planilha | **RF09** | O sistema deve permitir que sejam [exportados](Modeling/verbo?id=Exportação) documentos de planilha com informações sobre o [estoque](Modeling/objeto?id=Estoque). | Could |
| Histórico de vendas | **RF10** | O sistema deve gerar um [log](Modeling/objeto?id=Log) de registro de remoção e [adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao estoque. | Should |
| Histórico temporais | **RF11** | O sistema deve permitir [consultar](Modeling/verbo?id=Consultar-Produto) registros demarcados por períodos temporais. (diário, semanal, mensal, anual) | Could |
| [Filtro](Modeling/verbo?id=Filtrar-Produtos) por nome e preço | **RF12** | O sistema dever permitir [filtrar produtos](Modeling/verbo?id=Filtrar-Produtos) pelo nome e por preço. | Should |
| [Filtro](Modeling/verbo?id=Filtrar-Produtos) por data | **RF13** | O sistema deve permitir [filtrar](Modeling/verbo?id=Filtrar-Produtos) itens pela data. | Could |
| Plotagem de gráficos | **RF14** | O sistema deve gerar gráficos baseados no fluxo do [estoque](Modeling/objeto?id=Estoque). | Should |
| Atualização instantânea de [estoque](Modeling/objeto?id=Estoque) | **RF15** | O sistema deve ser capaz de atualizar a base de dados no momento em que uma operação é realizada. | Must |
| App para [consulta](Modeling/verbo?id=Consultar-Produto) fácil de [produtos](Modeling/objeto?id=Produto) | **RF16** | Possuir uma aplicação [PWA](Modeling/objeto?id=PWA) que funcione somente com acesso a internet para [busca](Modeling/verbo?id=Consultar-Produto) rápida de [produtos](Modeling/objeto?id=Produto) | Should |
| App para baixa fácil de [produtos](Modeling/objeto?id=Produto) | **RF17** | Possuir uma aplicação [PWA](Modeling/objeto?id=PWA) que funcione somente com acesso a internet para [remoção](Modeling/verbo?id=Baixa-em-Produto) rápida de [produtos](Modeling/objeto?id=Produto) | Should |
| Delimitar quantidade mínima de um [produto](Modeling/objeto?id=Produto) | **RF18** | O usuário deve ser capaz de delimitar uma quantidade mínima de um [produto](Modeling/objeto?id=Produto). |Could  |
| [Alertar](Modeling/verbo?id=Alertar) sobre quantidade mínima atingida | **RF19** | O sistema deve ser capaz de [alertar](Modeling/verbo?id=Alertar) o usuário quando um [produto](Modeling/objeto?id=Produto) ultrapassar o limite mínimo de quantidade. | Could |
| [Notificação](Modeling/verbo?id=Alertar) de [prazo de vencimento](Modeling/estado?id=Prazo-de-Validade) | **RF20** | O sistema deve [notificar](Modeling/verbo?id=Alertar) o usuário na data próxima ao [prazo de vencimento](Modeling/estado?id=Prazo-de-Validade) do [produto](Modeling/objeto?id=Produto) | Should |
| Lista de Compra | **RF21** | O sistema deve ter uma lista de compras de [produtos](Modeling/objeto?id=Produto) pedidos por [clientes](Modeling/objeto?id=usuário) que não têm em [estoque](Modeling/objeto?id=Estoque). | Would |
| Cadastro de diferentes lotes do mesmo produto | **RF22** | O sistema deve permitir o cadastro de um mesmo produto de lotes/validades diferentes. | Could |
| Personalização da geração dos gráficos | **RF23** | O sistema deve permitir a personalização da geração dos gráficos por período, categoria de produtos e funcionários. | Could |
| Registrar valor do [produto](Modeling/objeto?id=Produto) | **RF24** | O sistema deve ser capaz de armazenar o preço do [produto](Modeling/objeto?id=Produto). | Should |
| Consulta de [produtos](Modeling/objeto?id=Produto) mais vendidos | **RF25** | O sistema deve ser capaz de informar os [produtos](Modeling/objeto?id=Produto) que mais estão saindo do [estoque](Modeling/objeto?id=Estoque). | Would |
| Consulta de [produtos](Modeling/objeto?id=Produto) mais vendidos | **RF26** | O sistema deve ser capaz de informar os [produtos](Modeling/objeto?id=Produto) que mais estão saindo do [estoque](Modeling/objeto?id=Estoque). | Would |
| [Feedback](Modeling/verbo?id=feedback) | **RF27** | O sistema deve permitir que o usuário dê [feedbacks](Modeling/verbo?id=feedback) em relação a erros e novas funcionalidades.|  Would |
| Pedido de cadastro da empresa | **RF28** | O sistema deve permitir que o usuário preencha um formulário de pedido de cadastro de [estoque](Modeling/objeto?id=Estoque) de sua empresa.| Must  |
| Filtro pela [prazo de validade](Modeling/estado?id=Prazo-de-Validade) | **RF29** | O sistema deve permitir que o usuário filtre sua pesquisa pelo [prazo de validade](Modeling/estado?id=Prazo-de-Validade).| Could  |
| Nível de acesso | **RF30** | O sistema deve permitir que o usuário owner e admin edite o nível de acesso de um colaborador. |  Could  |
| Controle de colaboradores | **RF31** | O sistema deve permitir que o usuário owner ou admin adicione ou remova colaboradores da aplicação. | Must  |
| Cadastro de valor de fábrica | **RF32** | O sistema deve permitir que o usuário cadastre um [produto](Modeling/objeto?id=Produto) adicionando seu valor de fábrica. | Would   |
| Margem de lucro | **RF33** | O sistema deve permitir que o usuário Visualizar a margem de lucro dos seus [produto](Modeling/objeto?id=Produto). | Would   |


## Referências
* Técnica Moscow: <https://rockcontent.com/br/blog/metodo-moscow/>. Último acesso em 19/09/2020.
 
