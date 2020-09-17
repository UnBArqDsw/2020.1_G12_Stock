# Entrevista 4

| Data de Realização | Entrevistado | Entrevistador   |
| ------------------ | ------------ | ---------------- |
| 11/09/2020         | Ricardo      | Pedro Igor |

O entrevistado é [sócio](Modeling/objeto?id=Owner) da confeitaria Nutricakes, que trabalha com bolos, doces e salgados desde 2012. A confeitaria é localizada no Bairro Asa Norte - DF, porém realiza vendas em todo o DF por meio das redes sociais. A gravação para entrevista está disponível abaixo bem como a transcrição da mesma.

## Perguntas

### 1. Há quanto tempo você está nesse mundo dos negócios?

"Há 8 anos."

### 2. Qual o nome de seu negócio e como ele funciona?

"Chama-se Nutricakes Confeitaria Personalizada. É uma [empresa](Modeling/objeto?id=Micro-empresa) de bolos, doces e salgados nutritivos e trabalhamos com alimentos para pessoas com restrição alimentar."

### 3. Você possui quantos funcionários ou pessoas envolvidas nesse negócio?

"São 3 pessoas."

### 4. Qual a arrecadação bruta do negócio mensalmente?

"Em média de 7 a 8 mil em períodos normais. Em datas comemorativas chega a casa dos 15 mil reais."

### 5. Como você costuma mensurar quanto o seu negócio obteve de crescimento? E de prejuízo?

"Fazemos o controle financeiro, quase que contábil. Fazemos o controle de fluxo de caixa atraveś de DFC. Apuramos lucros e prejuízos com uma DRE que a gente tem, a gente sabe o ponto de equilíbrio e tudo mais. Temos um número de faturamento a se buscar."

### 6. Você costuma registrar em algum lugar os [produtos](Modeling/objeto?id=Produto) que são vendidos? Se sim, como funciona esse processo?

"Registramos em uma [planilha](Modeling/objeto?id=Planilha) de gerenciamento de vendas. Nela listamos todos os pedidos que foram feitos e quais itens estão nesses pedidos. Fazemos o controle do valor bruto do [produto](Modeling/objeto?id=Produto) e item por item para saber o controle de margem, quais [produtos](Modeling/objeto?id=Produto) tem vendido mais."

### 7. Você mantém o registro de seu [estoque](Modeling/objeto?id=Estoque)? Se sim, como ele é feito hoje?

"Sim e Não. No [estoque](Modeling/objeto?id=Estoque) de insumos não é feito. Temos um valor mínimo e quando vemos que está muito [em baixo](Modeling/estado?id=Estoque-baixo) são feitas compras. Porém temos um controle rigoroso [do que é produzido](Modeling/objeto?id=Produto), nosso [estoque](Modeling/objeto?id=Estoque) principal é o de [produtos](Modeling/objeto?id=Produto) já elaborados."

### 8. Imagine que você precisa saber se tem um certo [produto](Modeling/objeto?id=Produto) em [estoque](Modeling/objeto?id=Estoque) e rápido, mas você não está em sua loja. Como você procederia?
"Nesse caso não procede. É necessário estar lá presente para [acompanhar](Modeling/verbo?id=Consultar-produto)."

### 9. Já aconteceu de você se enganar quanto ao número de [produtos](Modeling/objeto?id=Produto) que possui em [estoque](Modeling/objeto?id=Estoque)?

"Sim."

### 10. Já aconteceu de você não possuir um [produto](Modeling/objeto?id=Produto) e ele ser extremamente requerido pelos seus [clientes](Modeling/objeto?id=usuário)?

"Não."

### 11. Já aconteceu de você comprar um [estoque](Modeling/objeto?id=Estoque) de certo produto de forma exagerada e ele não ser vendido com facilidade?

"Também não."

### 12. Qual a maior dificuldade que você enfrenta na parte administrativa de seu negócio?

"Mais na questão de controle de produção e administrativo. Administrar a produção, quanto tempo leva a produção de cada um dos [produtos](Modeling/objeto?id=Produto). Às vezes acredita-se que é possível fazer várias coisas em dado tempo e acaba não dando."

### 13. De 1 a 10, qual a sua afinidade com aparelhos celulares e computadores? Costuma depender de alguém para realizar certas ações?

"10."

### 14. De 1 a 10, quanto a tecnologia faz parte do seu dia a dia nessa parte dos negócios?

"10."

### 15. Em quais processos hoje em sua empresa você acha que daria para envolver tecnologia?

"Em todos eles. Desde produção a [gerenciamento](Modeling/verbo?id=Controle-de-Estoque), questão de entrega e logística."

## Gravação

<audio controls>
  <source src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/audios/interview/entrevistaRicardo.mp3" type="audio/mpeg">
</audio>

## Requisitos levantados
|                                     Id                                      |                Nome                 |
| :-------------------------------------------------------------------------: | :---------------------------------: |
| [#RF03](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  | [Adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao estoque |
| [#RF04](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  | [Consulta de estoque](Modeling/verbo?id=Consultar-Produto) |
| [#RF07](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  | [Remoção de itens](Modeling/verbo?id=Baixa-em-Produto) do estoque |
| [#RF10](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  | Histórico de vendas |
| [#RF19](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  | Delimitar quantidade mínima de um [produto](Modeling/objeto?id=Produto) |
| [#RF20](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  | [Alertar](Modeling/verbo?id=Alertar) sobre quantidade mínima atingida |
| [#RF25](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  | Registrar valor do [produto](Modeling/objeto?id=Produto) |
| [#RF26](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)  | Consulta de [produtos](Modeling/objeto?id=Produto) mais vendidos |
| [#RNF03](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) | [Consultas](Modeling/verbo?id=Consultar-Produto) remotas | 