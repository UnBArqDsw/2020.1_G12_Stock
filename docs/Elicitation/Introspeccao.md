# Introspecção

A introspecção é uma técnica muito utilizada na etapa de elicitação de requisitos. Ela tem como objetivo entender as funcionalidades importantes de um sistema. Apesar de muito usada, nem sempre a introspecção traz uma visão próxima da realidade, pois em muitos casos, a pessoa que aplica a introspecção não tem uma visão voltada para a experiência e expectativas do usuário.

## Históricos de Revisões

|    Data    | Versão |                          Descrição                           |  Autor(es)   |
| :--------: | :----: | :----------------------------------------------------------: | :----------: |
| 08/09/2020 |  1.0   | Criação do documento e adição da metodologia. | Micaella Gouveia |
| 10/09/2020 |  1.1   | Adição dos requisitos elicitados com base nas personas. | Micaella Gouveia |


## Metodologia
A elicitação dos requisitos por meio de instrospecção consiste em imaginar qual seria o fluxo de necessidades que o [usuário](Modeling/objeto?id=usuário) teria ao utilizar a aplicação.

Para o uso da técnica, utilizamos as personas criadas como base para a introspecção. Com isso, evitamos a falha desta técnica, pois os requisitos levantados serão retirados e pensados na visão do [usuário](Modeling/objeto?id=usuário), com base nas personas que possuímos, que são inspiradas em [clientes](Modeling/objeto?id=usuário) reais, pessoas reais que podem utilizar a aplicação.

Para visualizar as personas criadas, acesse: [**Personas**](Elicitation/Personas.md)

## Requisitos Levantados
|                                     Id                                      |                Nome                 |
| :-------------------------------------------------------------------------: | :---------------------------------: |
|    [#RF03](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     [Adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao estoque      |
|    [#RF04](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     [Consulta de estoque](Modeling/verbo?id=Consultar-Produto)      |
|    [#RF05](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        [Filtro por categoria]((Modeling/verbo?id=Filtrar-Produtos))         |
|    [#RF06](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |         [Tags](Modeling/objeto?id=Tag) nos [produtos](Modeling/objeto?id=Produto)         |
|    [#RF07](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     Remoção de itens do estoque     |
|    [#RF08](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto) por planilhas         |
|    [#RF09](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |           Gerar planilha            |
|    [#RF10](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |         Histórico de vendas         |
|    [#RF11](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        Históricos Temporais         |
|   [#RF015](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | Atualização instantânea de [estoque](Modeling/objeto?id=Estoque)  |
|   [#RF017](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | App para [consulta](Modeling/verbo?id=Consultar-Produto) fácil de [produtos](Modeling/objeto?id=Produto) |
|    [#RF19](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        Delimitar quantidade mínima de um [produto](Modeling/objeto?id=Produto)          |
|    [#RF20](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        [Alertar](Modeling/verbo?id=Alertar) sobre quantidade mínima atingida         |
| [#RNF01](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionaiss) |         Rapidez na [consulta](Modeling/verbo?id=Consultar-Produto)         |
| [#RNF03](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionaiss) |          [Consultas](Modeling/verbo?id=Consultar-Produto) remotas          |


## Referências
* Elicitação de Requisitos: <http://www2.dbd.puc-rio.br/pergamum/tesesabertas/0521479_08_cap_02.pdf>. Último acesso em 08/09/2020.