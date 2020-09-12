# Entrevista 2

| Data de Realização | Entrevistada      | Entrevistadora   |
| ------------------ | ----------------- | ---------------- |
| 07/09/2020         | Dinamara Carvalho | Micaella Gouveia |

A entrevista foi realizada com Dinamara Carvalho de 44 anos, que atualmente possui uma pequena empresa chamada ED Design de Móveis. O tipo de entrevista realizada foi fechada. A gravação para entrevista está disponível abaixo bem como a transcrição da mesma.

## Perguntas

### 1. Há quanto tempo você está nesse mundo dos negócios?

"Nós fazemos parte do nicho de móveis planejados e estamos neste mercado há 5 anos".

### 2. Qual o nome de seu negócio e como ele funciona?

"O nome do nosso negócio é ED Design de Móveis. O primeiro passo é a área de vendas onde é vendido o ambiente, depois esse ambiente é transformado em um projeto executivo, e desse projeto desce para o almoxarifado um listagem dos [produtos](Modeling/objeto?id=Produto) que devem ser separados para ir para a fabricação."

### 3. Você possui quantos funcionários ou pessoas envolvidas nesse negócio?

"Hoje nós estamos com 24 pessoas. Temos um grupo de 4 pessoas na área de vendas, no projeto nós temos 3 pessoas, nas máquinas 3, na área de fabricação de porta e alumínio 1, no almoxarifado 1, no administrativo 2, e na área de fabricação e montagem 6 pessoas.".

### _4. Qual a arrecadação bruta do negócio mensalmente?_

Esta pergunta não foi respondida nesta entrevista.

### 5. Como você costuma mensurar quanto o seu negócio obteve de crescimento? E de prejuízo?

"Neste período que estamos neste mercado só crescemos. Começamos com 8 funcionários, depois com 12 e agora com 24. Com a pandemia pensávamos que ia dar um freada, mas como as pessoas estão muito em casa elas estão investindo muito nas suas casas, então desde março que está interessante."

### 6. Você costuma registrar em algum lugar os [produtos](Modeling/objeto?id=Produto) que são vendidos? Se sim, como funciona esse processo?

"Nossa parte de controle de [estoque](Modeling/objeto?id=Estoque) eu acho muito arcaico e primitivo, pois fazemos todo o controle através de planilha, e temos um percentual de erro enorme e é muito cansativo pois tem que ficar atualizando as planilhas, nem sempre conseguimos pegar todos os [produtos](Modeling/objeto?id=Produto) que saíram, os que entraram conseguimos colocar todos, mas o que saiu temos uma dificuldade muito grande."

### 7. Você mantém o registro de seu [estoque](Modeling/objeto?id=Estoque)? Se sim, como ele é feito hoje?

"É por planilha, cada setor recebe uma planilha e eles vão atualizando. Essa planilha é feita manualmente, temos um Drive dentro da fábrica, e essa planilha feita manualmente vai para o Drive, para que o setor administrativo possa ter acesso."

### 8. Imagine que você precisa saber se tem um certo [produtos](Modeling/objeto?id=Produto) em [estoque](Modeling/objeto?id=Estoque) e rápido, mas você não está em sua loja. Como você procederia?

"Através do Drive. Nem sempre eu pego essa planilha atualizada, pois como a gente atualiza a cada 15 dias, se eu for fazer a [consulta]((Modeling/verbo?id=Consultar-Produto)) cinco dias depois, cinco dias ela já vai estar desatualizada, no décimo dia então ela vai estar dez dias desatualizada."

### 9. Já aconteceu de você se enganar quanto ao número de [produtos](Modeling/objeto?id=Produto) que possui em [estoque](Modeling/objeto?id=Estoque)?

"Já e até quando vamos fazer a compra já aconteceu."

### 10. Já aconteceu de você não possuir um [produto](Modeling/objeto?id=Produto) e ele ser extremamente requerido pelos seus [clientes](Modeling/objeto?id=usuário)?

"Já, demais. Como a gente mexe com MDF, nós não conseguimos mensurar quantos projetos vão entrar com aquele determinado MDF, e às vezes a gente se surpreende pois um determinado MDF foi vendido demais e falta em estoque."

### 11. Já aconteceu de você comprar um [estoque](Modeling/objeto?id=Estoque) de certo [produto](Modeling/objeto?id=Produto) de forma exagerada e ele não ser vendido com facilidade?

"Já aconteceu de a gente comprar o [produto](Modeling/objeto?id=Produto) e perceber que ele não foi bem aceito pelos [clientes](Modeling/objeto?id=usuário) e ele ficar lá no [estoque](Modeling/objeto?id=Estoque)."

### 12. Qual a maior dificuldade que você enfrenta na parte administrativa de seu negócio?

"Em relação ao [estoque](Modeling/objeto?id=Estoque) é essa necessidade de implementar um software que me dê essa precisão sobre o que eu tenho dentro do [estoque](Modeling/objeto?id=Estoque) para poder, na hora de fazer a compra, fazer uma melhor compra, um gerenciamento do que eu realmente preciso."

### 13. De 1 a 10, qual a sua afinidade com aparelhos celulares e computadores? Costuma depender de alguém para realizar certas ações?

"Costumo muito do meu filho mais velho, que já me ensinou muita coisa. Já dei uma avanço bom, mas eu que sou da faixa dos quarenta e poucos anos, eu tenho uma deficiência um pouco grande, mas estou tentando e avançando."

### 14. De 1 a 10, quanto a tecnologia faz parte do seu dia a dia nessa parte dos negócios?

"Acho que uns 8. Ela á um suporte enorma para a fábrica intera, todos os setores precisam dela em algum momento."

### 15. Em quais processos hoje em sua empresa você acha que daria para envolver tecnologia?

"Em todos, desde a venda até a fabricação, pois nossas máquinas estão todas interligadas na área de projeto".

## Gravação

<audio controls>
  <source src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/audios/interview/entrevistaDinamara.m4a" type="audio/mpeg">
</audio>

## Observação

- Antes da gravação da entrevista, a entrevistada mencionou a possibilidade de existir um [estoque](Modeling/objeto?id=Estoque) mínimo para um produto, em que seria possível definir a quantidade mínima de um prduto e quando esse quantidade é ultrapassada, um alerta seria enviado ao usuário.

## Requisitos Levantados

|                                     Id                                      |                Nome                 |
| :-------------------------------------------------------------------------: | :---------------------------------: |
|    [#RF03](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     [Adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao estoque      |
|    [#RF04](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |         [Consulta de estoque](Modeling/verbo?id=Consultar-Produto)         |
|    [#RF05](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        [Filtro](Modeling/verbo?id=Filtrar-Produtos) por categoria         |
|    [#RF07](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     Remoção de itens do estoque     |
|    [#RF08](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |           [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto) por planilhas            |
|    [#RF09](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |           Gerar planilha            |
|    [#RF10](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |         Histórico de vendas         |
|   [#RF12](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |       [Filtro](Modeling/verbo?id=Filtrar-Produtos) por nome e preço       |
|   [#RF15](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | Atualização instantânea de [estoque](Modeling/objeto?id=Estoque)  |
|   [#RF16](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | [Importação](Modeling/verbo?id=Importação) de planilha para load de estoque  |
|   [#RF17](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | App para [consulta](Modeling/verbo?id=Consultar-Produto) fácil de [produtos](Modeling/objeto?id=Produto) |
|   [#RF018](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | App para baixa fácil de [produtos](Modeling/objeto?id=Produto) |
|    [#RF19](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     Delimitar quantidade mínima de um [produto](Modeling/objeto?id=Produto)            |
|    [#RF20](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     [Alertar](Modeling/verbo?id=Alertar) sobre quantidade mínima atingida            |
| [#RNF01](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |         Rapidez na [consulta](Modeling/verbo?id=Consultar-Produto)         |
| [#RNF03](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |          [Consultas](Modeling/verbo?id=Consultar-Produto) remotas          |