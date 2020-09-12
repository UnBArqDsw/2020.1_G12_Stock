# Entrevista

A entrevista é uma técnica de elicitação de requisitos que se baseia em questionar os [stakeholders](Modeling/objeto?id=Stakeholder) sobre processos e sistemas atuais e sobre o que é desejado para o que vai ser desenvolvido. Entrevistas podem ser fechadas ou abertas, enquanto as fechadas são baseadas em um conjunto pré-existente de perguntas as abertas são sem script pré-definido, se adptando de acordo com o conhecimento do [stakeholder](Modeling/objeto?id=Stakeholder).

## Históricos de Revisões

|    Data    | Versão |                          Descrição                           |    Autor(es)     |
| :--------: | :----: | :----------------------------------------------------------: | :--------------: |
| 31/08/2020 |  1.0   | Criação do documento de entrevista e adição da entrevista 1. |   Gabriel Davi   |
| 08/09/2020 |  1.1   |  Adição da entrevista 2 e adição do roteiro da entrevista.   | Micaella Gouveia |
| 09/09/2020 |  1.2   |             Adição dos requisitos da entrevista 1.           |   Gabriel Davi   |
| 09/09/2020 |  1.3   |             Adição da entrevista 3 e requisitos.           |   Sofia Patrocínio   |

## Roteiro de Perguntas

Foi desenvolvido um roteiro de perguntas que será utilizado para todas as entrevistas realizadas. Ele tem o intuito de padronizar as perguntas e possibilitar uma comparação entre as respostas, sendo possível elicitar os requisitos. Segue abaixo este roteiro:

1. Há quanto tempo você está nesse mundo dos negócios?
2. Qual o nome de seu negócio e como ele funciona?
3. Você possui quantos funcionários ou pessoas envolvidas nesse negócio?
4. Qual a arrecadação bruta do negócio mensalmente?_(Opcional)_
5. Como você costuma mensurar quanto o seu negócio obteve de crescimento? E de prejuízo?
6. Você costuma registrar em algum lugar os [produtos](Modeling/objeto?id=Produto) que são vendidos? Se sim, como funciona esse processo?
7. Você mantém o registro de seu [estoque](Modeling/objeto?id=Estoque)? Se sim, como ele é feito hoje?
8. Imagine que você precisa saber se tem um certo [produto](Modeling/objeto?id=Produto) em [estoque](Modeling/objeto?id=Estoque) e rápido, mas você não está em sua loja. Como você procederia?
9. Já aconteceu de você se enganar quanto ao número de [produtos](Modeling/objeto?id=Produto) que possui em [estoque](Modeling/objeto?id=Estoque)?
10. Já aconteceu de você não possuir um [produto](Modeling/objeto?id=Produto) e ele ser extremamente requerido pelos seus [clientes](Modeling/objeto?id=usuário)?
11. Já aconteceu de você comprar um [estoque](Modeling/objeto?id=Estoque) de certo [produto](Modeling/objeto?id=Produto) de forma exagerada e ele não ser vendido com facilidade?
12. Qual a maior dificuldade que você enfrenta na parte administrativa de seu negócio?
13. De 1 a 10, qual a sua afinidade com aparelhos celulares e computadores? Costuma depender de alguém para realizar certas ações?
14. De 1 a 10, quanto a tecnologia faz parte do seu dia a dia nessa parte dos negócios?
15. Em quais processos hoje em sua empresa você acha que daria para envolver tecnologia?

## Entrevistas

### [*Entrevista 1 - Ivanete Bezerra, 49 anos](Elicitation/Entrevistas/entrevista1.md)
### [*Entrevista 2 - Dinamara Carvalho, 44 anos](Elicitation/Entrevistas/entrevista2.md)
### [*Entrevista 3 - Raissa, 27 anos](Elicitation/Entrevistas/entrevista3.md)


## Requisitos Totais levantados

|                                     Id                                      |                Nome                 |
| :-------------------------------------------------------------------------: | :---------------------------------: |
|    [#RF03](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     [Adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao estoque      |
|    [#RF04](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |         [Consulta de estoque](Modeling/verbo?id=Consultar-Produto)         |
|    [#RF05](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        [Filtro por categoria](Modeling/verbo?id=Filtrar-Produtos)         |
|    [#RF07](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     Remoção de itens do estoque     |
|    [#RF08](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |           [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto) por planilhas            |
|    [#RF09](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |           Gerar planilha            |
|    [#RF10](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |         Histórico de vendas         |
|   [#RF012](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |       [Filtro por nome e preço](Modeling/verbo?id=Filtrar-Produtos)       |
|   [#RF014](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        Plotagem de gráficos         |
|   [#RF015](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | Atualização instantânea de [estoque](Modeling/objeto?id=Estoque)  |
|   [#RF16](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | [Importação](Modeling/verbo?id=Importação) de planilha para load de estoque  |
|   [#RF017](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | App para [consulta fácil de produto](Modeling/verbo?id=Consultar-Produto) |
|   [#RF018](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | App para baixa fácil de [produto](Modeling/objeto?id=Produto) |
|    [#RF19](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     Delimitar quantidade mínima de um [produto](Modeling/objeto?id=Produto)            |
|    [#RF20](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     [Alertar](Modeling/verbo?id=Alertar) sobre quantidade mínima atingida            |
| [#RF22](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     Lista de Compra                   |
| [#RNF01](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |         Rapidez na [consulta](Modeling/verbo?id=Consultar-Produto)         |
| [#RNF02](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |         Gráficos didáticos          |
| [#RNF03](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |          [Consultas](Modeling/verbo?id=Consultar-Produto) remotas          |
