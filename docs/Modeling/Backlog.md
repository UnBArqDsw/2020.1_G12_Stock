# Backlog do Produto

O Product Backlog é uma lista de funcionalidades desejadas de um produto, ou seja, os requisitos que um cliente espera receber ao final do projeto, descrito com sua própria linguagem. Ele cresce e muda à medida que se aprende mais sobre o [produto](Modeling/objeto?id=produto) e seus [usuários](Modeling/objeto?id=usuário).

## Histórico de Revisões

|    Data    | Versão |             Descrição             |                                  Autor(es)                                  |
| :--------: | :----: | :-------------------------------: | :-------------------------------------------------------------------------: |
| 17/09/2020 |  1.0   |        Criação das histórias de [usuário](Modeling/objeto?id=usuário) e backlog do [produto](Modeling/objeto?id=produto)       | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 17/09/2020 |  1.1   |        Criação do documento e adição da introdução, estruturação e referências      | Micaella Gouveia |
| 17/09/2020 |  1.2   |      Adição da tabela      | Sofia Patrocínio |

## Estruturação
Para melhor estruturar o Product Backlog nós utilizamos as chamadas Histórias de [Usuário](Modeling/objeto?id=usuário), que explicitado no documento de [Metodologias](Project/Metodologias.md), são uma forma de definir e organizar os requisitos do sistema, centrando a visão no [usuário](Modeling/objeto?id=usuário), contendo a descrição detalhada dos requisitos de cada solicitação a ser implementada.
As Histórias de [Usuário](Modeling/objeto?id=usuário) foram agrupadas e formaram as Features, que irão compor nossos Épicos, dividos em [**Usuário**](Modeling/objeto?id=usuário), [**Produto**](Modeling/objeto?id=produto) e **Vendas**.

## Backlog


<table style="width: 933px;">
<tbody>
<tr style="height: 43px;">
<td style="width: 15px; height: 43px;">Épicos</td>
<td style="width: 15px; height: 43px;">Features</td>
<td style="width: 132px; height: 43px;">Eu como</td>
<td style="width: 167px; height: 43px;">Desejo</td>
<td style="width: 176px; height: 43px;">Para que eu possa</td>
<td style="width: 119px; height: 43px;">Requisitos</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 138px; border: 3px solid #F7F7F7;" rowspan="6">Usuário</td>
<td style="width: 15px; height: 69px; border: 3px solid #F7F7F7;" rowspan="3">&nbsp;Cadastro</td>
<td style="width: 132px; height: 23px;">Usuário Owner</td>
<td style="width: 167px; height: 23px;">Fazer o pedido de cadastro da minha empresa</td>
<td style="width: 176px; height: 23px;">&nbsp;Criar o meu controle de estoque na aplicação</td>
<td style="width: 119px; height: 23px;">&nbsp;RF28</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Realizar o login na aplicação</td>
<td style="width: 176px; height: 23px;">&nbsp;Ter acesso &agrave; aplicação</td>
<td style="width: 119px; height: 23px;">&nbsp;RF01</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">&nbsp;Criar contas para meus funcionários com diferentes níveis de acessos</td>
<td style="width: 176px; height: 23px;">Melhor controlar quais funcionalidades cada funcionário terá acesso na aplicação&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF02</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 46px; border: 3px solid #F7F7F7;" rowspan="2">&nbsp;Hierarquia</td>
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">&nbsp;Editar o nível de acesso de um colaborador</td>
<td style="width: 176px; height: 23px;">&nbsp;Alterar os cargos dos colaboradores</td>
<td style="width: 119px; height: 23px;">&nbsp;RF30</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">&nbsp;Adicionar ou remover um colaborador da aplicação</td>
<td style="width: 176px; height: 23px;">Ter controle dos colaboradores que estão contratados&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF31</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 23px;">&nbsp;Feedback</td>
<td style="width: 132px; height: 23px;">Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Dar feedbacks ao suporte da aplicação</td>
<td style="width: 176px; height: 23px;">&nbsp;Relatar qualquer erro encontrado ou sugestões de novas funcionalidades</td>
<td style="width: 119px; height: 23px;">&nbsp;RF27</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 460px; border: 3px solid #F7F7F7;" rowspan="20">Produto</td>
<td style="width: 15px; height: 253px; border: 3px solid #F7F7F7;" rowspan="11">&nbsp;Controle</td>
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">&nbsp;Cadastrar itens no meu controle de estoque</td>
<td style="width: 176px; height: 23px;">Administrar o fluxo do estoque&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF03</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">&nbsp;No momento do cadastro de um item, adicionar tags aos produtos</td>
<td style="width: 176px; height: 23px;">Melhor dividí-los em diferentes níveis de categorias&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF06</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Remover itens do controle de estoque</td>
<td style="width: 176px; height: 23px;">&nbsp;Controlar vendas e remoções do estoque</td>
<td style="width: 119px; height: 23px;">&nbsp;RF07</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Importar uma planilha em excel com dados do meu estoque na aplicação</td>
<td style="width: 176px; height: 23px;">Carregar meus dados de estoque que estão em planilhas dentro do aplicatico Stock&nbsp;</td>
<td style="width: 119px; height: 23px;">RF08, RNF02&nbsp;</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário</td>
<td style="width: 167px; height: 23px;">Que a atualização dos dados seja feita assim que houver alguma modificação no controle do estoque</td>
<td style="width: 176px; height: 23px;">&nbsp;Ter precisão nos dados apresentados no controle</td>
<td style="width: 119px; height: 23px;">&nbsp;RF15, RNF01</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário</td>
<td style="width: 167px; height: 23px;">Dar baixa em um produto pelo aplicativo mobile</td>
<td style="width: 176px; height: 23px;">Vender ou remover produtos mais facilmente&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF18, RNF03, RNF05</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Definir a quantidade mínima de determinado produto</td>
<td style="width: 176px; height: 23px;">&nbsp;Ser notificado quando um item estiver em baixa no estoque</td>
<td style="width: 119px; height: 23px;">&nbsp;RF19</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário</td>
<td style="width: 167px; height: 23px;">Ter uma lista de produtos solicitados por clientes que não estão disponíveis no estoque</td>
<td style="width: 176px; height: 23px;">Adquirir esses produtos e disponibinizá-los no estoque&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF22</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Cadastrar mesmo produto separados por diferentes lotes</td>
<td style="width: 176px; height: 23px;">&nbsp;Ter controle da validade de diferentes itens do mesmo produto</td>
<td style="width: 119px; height: 23px;">&nbsp;RF23</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Cadastrar um produto adicionando seu valor de fábrica</td>
<td style="width: 176px; height: 23px;">&nbsp;Visualizar uma margem de lucro satisfatória</td>
<td style="width: 119px; height: 23px;">RF32&nbsp;</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Cadastrar valor de cada produto&nbsp;</td>
<td style="width: 176px; height: 23px;">&nbsp;Visualizar preço dos produtos</td>
<td style="width: 119px; height: 23px;">&nbsp;RF25</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 161px; border: 3px solid #F7F7F7;" rowspan="7">&nbsp;Consulta</td>
<td style="width: 132px; height: 23px;">&nbsp;Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Consultar itens presentes no meu estoque</td>
<td style="width: 176px; height: 23px;">&nbsp;Saber o que há no meu estoque</td>
<td style="width: 119px; height: 23px;">&nbsp;RF04, RNF01, RNF03, RNF05</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Filtrar a minha busca por uma categoria no controle de estoque</td>
<td style="width: 176px; height: 23px;">Acessar com facilidade os produtos relacionados a esta categoria&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF05</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Filtrar a busca de um produto por nome e/ou preço</td>
<td style="width: 176px; height: 23px;">&nbsp;Acessar com facilidade as informações sobre este produto</td>
<td style="width: 119px; height: 23px;">&nbsp;RF12</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Gostaria de, no momento da listagem, poder filtrar os produtos pela data de adição</td>
<td style="width: 176px; height: 23px;">Ter um melhor controle dos produtos que estão mais tempo parados no meu estoque&nbsp;</td>
<td style="width: 119px; height: 23px;">RF13&nbsp;</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Possuir uma versão mobile do aplicativo do estoque</td>
<td style="width: 176px; height: 23px;">&nbsp;Fazer consultas mais ágeis de produtos no estoque</td>
<td style="width: 119px; height: 23px;">&nbsp;RF17, ,RNF03, RNF05</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">&nbsp;Consultar produtos que mais saem do meu estoque</td>
<td style="width: 176px; height: 23px;">&nbsp;Saber quais produtos devo comprar em maior quantidade</td>
<td style="width: 119px; height: 23px;">&nbsp;RF26, RNF01</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;No momento da listagem, poder filtrar os produtos pela data de vencimento</td>
<td style="width: 176px; height: 23px;">&nbsp;Ter um melhor controle dos produtos que estão para vencer</td>
<td style="width: 119px; height: 23px;">&nbsp;RF29</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 46px; border: 3px solid #F7F7F7;" rowspan="2">&nbsp;Notificação</td>
<td style="width: 132px; height: 23px;">&nbsp;Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Ser alertado que um ou mais produtos estão com quantidades mínimas no estoque</td>
<td style="width: 176px; height: 23px;">Reabastecer itens quando estiver em baixa no estoque&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF20</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário</td>
<td style="width: 167px; height: 23px;">&nbsp;Ser alertado caso um produto ultrapasse o seu prazo de validade</td>
<td style="width: 176px; height: 23px;">Organizar meu estoque, retirando este produto vencido&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF21</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 184px; border: 3px solid #F7F7F7;" rowspan="8">Venda</td>
<td style="width: 15px; height: 138px; border: 3px solid #F7F7F7;" rowspan="6">&nbsp;Gráficos</td>
<td style="width: 132px; height: 23px;">&nbsp;Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Gerar planilhas de análise do estoque&nbsp;</td>
<td style="width: 176px; height: 23px;">&nbsp;Documentar todas as análises de vendas e controle de estoque</td>
<td style="width: 119px; height: 23px;">&nbsp;RF09, RNF02</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Visualizar gráficos baseados no fluxo de estoque</td>
<td style="width: 176px; height: 23px;">Analisar de forma visual e eficiente o fluxo do meu estoque&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF14, RNF02</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Gerar gráficos que marcam o periodo por quantidade total de produto</td>
<td style="width: 176px; height: 23px;">&nbsp;Fazer uma análise melhor do crescimento geral do meu estoque</td>
<td style="width: 119px; height: 23px;">&nbsp;RF24, RNF02</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Gerar gráficos que marcam a quantidade de produtos por categoria&nbsp;</td>
<td style="width: 176px; height: 23px;">&nbsp;Saber a quantidade de produtos por categorias</td>
<td style="width: 119px; height: 23px;">&nbsp;RF24, RNF02</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Gerar gráficos que marcam a quantidade de produtos por funcionários&nbsp;</td>
<td style="width: 176px; height: 23px;">Ter controle das vendas dos meus funcionários&nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF24, RNF02</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Visualizar a margem de lucro dos meus produtos</td>
<td style="width: 176px; height: 23px;">&nbsp;Precificar da melhor forma os produtos</td>
<td style="width: 119px; height: 23px;">&nbsp;RF33</td>
</tr>
<tr style="height: 23px;">
<td style="width: 15px; height: 46px; border: 3px solid #F7F7F7;" rowspan="2">&nbsp;Histórico</td>
<td style="width: 132px; height: 23px;">&nbsp;Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Consultar um log de remoção e adição de itens ao estoque</td>
<td style="width: 176px; height: 23px;">Ter uma noção melhor do fluxo do meu estoque &nbsp;</td>
<td style="width: 119px; height: 23px;">&nbsp;RF10, RNF01</td>
</tr>
<tr style="height: 23px;">
<td style="width: 132px; height: 23px;">&nbsp;Usuário Owner e Usuário Admin</td>
<td style="width: 167px; height: 23px;">Filtrar para consulta um log de remoção e adição de itens ao estoque de forma temporal&nbsp;</td>
<td style="width: 176px; height: 23px;">&nbsp;Consultar o fluxo de estoque em um período específico</td>
<td style="width: 119px; height: 23px;">&nbsp;RF11, RNF01</td>
</tr>
</tbody>
</table>


## Referências
* Product Backlog: <https://bit.ly/2RycNLo>. Último acesso em 17/09/2020.
* Epic, Feature e User Story: <https://www.ateomomento.com.br/epic-feature-e-user-story/>. Último acesso em 17/09/2020.
 