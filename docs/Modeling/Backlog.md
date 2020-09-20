# Backlog do Produto

O Product Backlog é uma lista de funcionalidades desejadas de um produto, ou seja, os requisitos que um cliente espera receber ao final do projeto, descrito com sua própria linguagem. Ele cresce e muda à medida que se aprende mais sobre o [produto](Modeling/objeto?id=produto) e seus [usuários](Modeling/objeto?id=usuário).

## Histórico de Revisões

|    Data    | Versão |             Descrição             |                                  Autor(es)                                  |
| :--------: | :----: | :-------------------------------: | :-------------------------------------------------------------------------: |
| 17/09/2020 |  1.0   |        Criação das histórias de [usuário](Modeling/objeto?id=usuário) e backlog do [produto](Modeling/objeto?id=produto)       | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 17/09/2020 |  1.1   |        Criação do documento e adição da introdução, estruturação e referências      | Micaella Gouveia |
| 17/09/2020 |  1.2   |      Adição da tabela      | Sofia Patrocínio |
| 18/09/2020 |  1.3   |      Linkagem dos léxicos      | Sofia Patrocínio |

## Estruturação
Para melhor estruturar o Product Backlog nós utilizamos as chamadas Histórias de [Usuário](Modeling/objeto?id=usuário), que explicitado no documento de [Metodologias](Project/Metodologias.md), são uma forma de definir e organizar os requisitos do sistema, centrando a visão no [usuário](Modeling/objeto?id=usuário), contendo a descrição detalhada dos requisitos de cada solicitação a ser implementada.
As Histórias de [Usuário](Modeling/objeto?id=usuário) foram agrupadas e formaram as Features, que irão compor nossos Épicos, dividos em [**Usuário**](Modeling/objeto?id=usuário), [**Produto**](Modeling/objeto?id=produto) e **Vendas**.

## Backlog

<style>
tr {
    background-color: white;
}
.markdown-section td.backlog {
    border: 3px solid #EBEBEB;
}


table, td.backlog{
  border-collapse: collapse;
  background-color: white;
}
</style>


<table style="width: 933px; background-color:white">
<tbody>
<tr style="height: 43px; background-color:white">
<td class="backlog" style="width: 15px; height: 43px;">Épicos</td class="backlog">
<td class="backlog" style="width: 15px; height: 43px;">Features</td class="backlog">
<td class="backlog" style="width: 132px; height: 43px;">Eu como</td class="backlog">
<td class="backlog" style="width: 167px; height: 43px;">Desejo</td class="backlog">
<td class="backlog" style="width: 176px; height: 43px;">Para que eu possa</td class="backlog">
<td class="backlog" style="width: 119px; height: 43px;">Requisitos</td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 15px; height: 138px;" rowspan="6"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 15px; height: 69px; " rowspan="3"><a href="#/Modeling/verbo?id=cadastrar-produto">Cadastro</a></td class="backlog">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Fazer o pedido de cadastro da minha empresa</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Criar o meu <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a> na aplicação</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF28</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Realizar o login na aplicação</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Ter acesso &agrave; aplicação</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF01</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Criar contas para meus funcionários com diferentes <a href="#/Modeling/objeto?id=Papéis-dos-colaboradores">níveis de acesso</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Melhor controlar quais funcionalidades cada funcionário terá acesso na aplicação</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF02</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 15px; height: 46px; " rowspan="2">Hierarquia</td class="backlog">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Editar o <a href="#/Modeling/objeto?id=Papéis-dos-colaboradores">nível de acesso</a>  de um colaborador</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Alterar os <a href="#/Modeling/objeto?id=Papéis-dos-colaboradores">cargos</a> dos colaboradores</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF30</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Adicionar ou remover um colaborador da aplicação</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Ter controle dos colaboradores que estão contratados</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF31</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 15px; height: 23px;"><a href="#/Modeling/verbo?id=feedback">Feedback</a></td class="backlog">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Dar <a href="#/Modeling/verbo?id=feedback">feedbacks</a> ao suporte da aplicação</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Relatar qualquer <a href="#/Modeling/objeto?id=bug">erro</a> encontrado ou sugestões de novas funcionalidades</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF27</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 15px; height: 460px; " rowspan="20">Produto</td class="backlog">
<td class="backlog" style="width: 15px; height: 253px; " rowspan="11"><a href="#/Modeling/verbo?id=controle-de-estoque">Controle</a></td class="backlog">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=cadastrar-produto">Cadastrar</a> <a href="#/Modeling/objeto?id=produto">itens</a> no meu <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Administrar o <a href="#/Modeling/verbo?id=fluxo">fluxo</a> do <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF03</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">No momento do <a href="#/Modeling/verbo?id=cadastrar-produto">cadastro</a> de um <a href="#/Modeling/objeto?id=produto">item</a>, adicionar <a href="#/Modeling/objeto?id=tag">tags</a> aos <a href="#/Modeling/objeto?id=produto">produtos</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Melhor dividí-los em diferentes níveis de <a href="#/Modeling/objeto?id=tag">categorias</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF06</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=baixa-em-produto">Remover</a> <a href="#/Modeling/objeto?id=produto">itens</a> do <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;"><a href="#/Modeling/verbo?id=controle-de-estoque">Controlar</a> vendas e remoções do <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF07</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=Importação">Importar</a> uma <a href="#/Modeling/objeto?id=planilha">planilha</a> em excel com dados do meu <a href="#/Modeling/objeto?id=estoque">estoque</a> na aplicação</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Carregar meus dados de <a href="#/Modeling/objeto?id=estoque">estoque</a> que estão em <a href="#/Modeling/objeto?id=planilha">planilhas</a> dentro do aplicatico Stock</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF08</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF02</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Que a atualização dos dados seja feita assim que houver alguma modificação no <a href="#/Modeling/verbo?id=controle-de-estoque">controle do estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Ter precisão nos dados apresentados no <a href="#/Modeling/verbo?id=controle-de-estoque">controle</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF15</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF01</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=baixa-em-produto">Dar baixa</a> em um <a href="#/Modeling/objeto?id=produto">produto</a> pelo aplicativo mobile</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;"><a href="#/Modeling/verbo?id=baixa-em-produto">Vender ou remover</a> <a href="#/Modeling/objeto?id=produto">produtos</a> mais facilmente</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF18</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF03</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF03</a>x</td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Definir a quantidade mínima de determinado <a href="#/Modeling/objeto?id=produto">produto</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Ser <a href="#/Modeling/verbo?id=alertar">notificado</a> quando um <a href="#/Modeling/objeto?id=produto">item</a> estiver em baixa no <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF19</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Ter uma lista de <a href="#/Modeling/objeto?id=produto">produtos</a> solicitados por clientes que não estão disponíveis no <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Adquirir esses <a href="#/Modeling/objeto?id=produto">produtos</a> e disponibinizá-los no <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF22</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=cadastrar-produto">Cadastrar</a> mesmo <a href="#/Modeling/objeto?id=produto">produto</a> separados por diferentes lotes</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Ter <a href="#/Modeling/verbo?id=controle-de-estoque">controle</a> da <a href="#/Modeling/estado?id=prazo-de-validade">validade</a> de diferentes <a href="#/Modeling/objeto?id=produto">itens</a> do mesmo <a href="#/Modeling/objeto?id=produto">produto</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF23</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=cadastrar-produto">Cadastrar</a> um <a href="#/Modeling/objeto?id=produto">produto</a> adicionando seu valor de fábrica</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Visualizar uma margem de lucro satisfatória</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF32</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=cadastrar-produto">Cadastrar</a> valor de cada <a href="#/Modeling/objeto?id=produto">produto</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Visualizar preço dos <a href="#/Modeling/objeto?id=produto">produto</a>s</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF25</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 15px; height: 161px; " rowspan="7"><a href="#/Modeling/verbo?id=consultar-produto">Consulta</a></td class="backlog">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> <a href="#/Modeling/objeto?id=produto">item</a> presentes no meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Saber o que há no meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF04</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF01</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF03</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF05</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=filtrar-produtos">Filtrar</a> a minha busca por uma <a href="#/Modeling/objeto?id=tag">categoria</a> no <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Acessar com facilidade os <a href="#/Modeling/objeto?id=produto">produtos</a> relacionados a esta <a href="#/Modeling/objeto?id=tag">categoria</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF05</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=filtrar-produtos">Filtrar</a> a busca de um <a href="#/Modeling/objeto?id=produto">produto</a> por nome e/ou preço</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Acessar com facilidade as informações sobre este <a href="#/Modeling/objeto?id=produto">produto</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF12</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Gostaria de, no momento da listagem, poder <a href="#/Modeling/verbo?id=filtrar-produtos">filtrar</a> os <a href="#/Modeling/objeto?id=produto">produtos</a> pela data de <a href="#/Modeling/verbo?id=cadastrar-produto">adição</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Ter um melhor <a href="#/Modeling/verbo?id=controle-de-estoque">controle</a> dos <a href="#/Modeling/objeto?id=produto">produtos</a> que estão mais tempo parados no meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF13</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Possuir uma versão mobile do aplicativo do <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Fazer <a href="#/Modeling/verbo?id=consultar-produto">consultas</a> mais ágeis de <a href="#/Modeling/objeto?id=produto">produtos</a> no <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF17</a>, ,<a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF03</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF05</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> <a href="#/Modeling/objeto?id=produto">produtos</a> que mais saem do meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Saber quais <a href="#/Modeling/objeto?id=produto">produtos</a> devo comprar em maior quantidade</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF26</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF01</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">No momento da listagem, poder <a href="#/Modeling/verbo?id=filtrar-produtos">filtrar</a> os <a href="#/Modeling/objeto?id=produto">produtos</a> pela <a href="#/Modeling/estado?id=prazo-de-validade">data de vencimento</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Ter um melhor <a href="#/Modeling/verbo?id=controle-de-estoque">controle</a> dos <a href="#/Modeling/objeto?id=produto">produtos</a> que estão para vencer</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF29</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 15px; height: 46px; " rowspan="2"><a href="#/Modeling/verbo?id=alertar">Notificação</a></td class="backlog">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Ser <a href="#/Modeling/verbo?id=alertar">alertado</a> que um ou mais <a href="#/Modeling/objeto?id=produto">produtos</a> estão com quantidades mínimas no <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Reabastecer <a href="#/Modeling/objeto?id=produto">item</a> quando estiver em baixa no <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF20</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=usuário">Usuário</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Ser <a href="#/Modeling/verbo?id=alertar">alertado</a> caso um <a href="#/Modeling/objeto?id=produto">produto</a> ultrapasse o seu <a href="#/Modeling/estado?id=prazo-de-validade">prazo de validade</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Organizar meu <a href="#/Modeling/objeto?id=estoque">estoque</a>, retirando este <a href="#/Modeling/objeto?id=produto">produto</a> vencido</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF21</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 15px; height: 184px; " rowspan="8">Venda</td class="backlog">
<td class="backlog" style="width: 15px; height: 138px; " rowspan="6">Gráficos</td class="backlog">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Gerar <a href="#/Modeling/objeto?id=planilha">planilhas</a> de análise do <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Documentar todas as análises de vendas e <a href="#/Modeling/verbo?id=controle-de-estoque">controle de estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF09</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF02</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Visualizar gráficos baseados no <a href="#/Modeling/verbo?id=fluxo">fluxo</a> de <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Analisar de forma visual e eficiente o <a href="#/Modeling/verbo?id=fluxo">fluxo</a> do meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF14</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF02</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Gerar gráficos que marcam o periodo por quantidade total de <a href="#/Modeling/objeto?id=produto">produto</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Fazer uma análise melhor do crescimento geral do meu <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF24</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF02</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Gerar gráficos que marcam a quantidade de <a href="#/Modeling/objeto?id=produto">produtos</a> por <a href="#/Modeling/objeto?id=tag">categoria</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Saber a quantidade de <a href="#/Modeling/objeto?id=produto">produtos</a> por <a href="#/Modeling/objeto?id=tag">categorias</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF24</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF02</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Gerar gráficos que marcam a quantidade de <a href="#/Modeling/objeto?id=produto">produtos</a> por funcionários</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Ter <a href="#/Modeling/verbo?id=controle-de-estoque">controle</a> das vendas dos meus funcionários</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF24</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF02</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;">Visualizar a margem de lucro dos meus <a href="#/Modeling/objeto?id=produto">produtos</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Precificar da melhor forma os <a href="#/Modeling/objeto?id=produto">produtos</a></td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF33</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 15px; height: 46px; " rowspan="2">Histórico</td class="backlog">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> um <a href="#/Modeling/objeto?id=log">log</a> de <a href="#/Modeling/verbo?id=baixa-em-produto">remoção</a> e <a href="#/Modeling/verbo?id=cadastrar-produto">adição</a> de <a href="#/Modeling/objeto?id=produto">item</a> ao <a href="#/Modeling/objeto?id=estoque">estoque</a></td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;">Ter uma noção melhor do <a href="#/Modeling/verbo?id=fluxo">fluxo</a> do meu <a href="#/Modeling/objeto?id=estoque">estoque</a> </td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF10</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF01</a></td class="backlog">
</tr>
<tr style="height: 23px;">
<td class="backlog" style="width: 132px; height: 23px;"><a href="#/Modeling/objeto?id=owner">Usuário Owner</a> e <a href="#/Modeling/objeto?id=admin">Usuário Admin</a></td class="backlog">
<td class="backlog" style="width: 167px; height: 23px;"><a href="#/Modeling/verbo?id=filtrar-produtos">Filtrar</a> para <a href="#/Modeling/verbo?id=consultar-produto">consulta</a> um <a href="#/Modeling/objeto?id=log">log</a> de <a href="#/Modeling/verbo?id=baixa-em-produto">remoção</a> e <a href="#/Modeling/verbo?id=cadastrar-produto">adição</a> de <a href="#/Modeling/objeto?id=produto">itens</a> ao <a href="#/Modeling/objeto?id=estoque">estoque</a> de forma temporal</td class="backlog">
<td class="backlog" style="width: 176px; height: 23px;"><a href="#/Modeling/verbo?id=consultar-produto">Consultar</a> o <a href="#/Modeling/verbo?id=fluxo">fluxo</a> de <a href="#/Modeling/objeto?id=estoque">estoque</a> em um período específico</td class="backlog">
<td class="backlog" style="width: 119px; height: 23px;"><a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-funcionais">RF11</a>, <a href="#/Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais">RNF01</a></td class="backlog">
</tr>
</tbody>
</table>


## Referências
* Product Backlog: <https://bit.ly/2RycNLo>. Último acesso em 17/09/2020.
* Epic, Feature e User Story: <https://www.ateomomento.com.br/epic-feature-e-user-story/>. Último acesso em 17/09/2020.
 