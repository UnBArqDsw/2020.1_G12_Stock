# Entrevista 1

| Data de Realização | Entrevistada    | Entrevistadora |
| ------------------ | --------------- | -------------- |
| 31/08/2020         | Ivanete Bezerra | Gabriel Davi   |

A entrevista foi realizada com Ivanete Bezerra de 49 anos, que atualmente possui um empreendimento de pequeno porte chamado Bonnavita. O tipo de entrevista realizada foi fechada. A gravação para entrevista está disponível abaixo bem como a transcrição da mesma.

## Perguntas

### 1. Há quanto tempo você está nesse mundo dos negócios?

“Aproximadamente 3 meses."

### 2. Qual o nome de seu negócio e como ele funciona?

“O nome da minha empresa é bonavita, é uma empresa de [produtos](Modeling/objeto?id=Produto) naturais. Nós somos atacado e varejo, vendemos ‘saúde’ (slogan da empresa) . A gente capta [cliente](Modeling/objeto?id=usuário) nas redes de relacionamento e por visita presencial em estabelecimentos que vendem nossos [produtos](Modeling/objeto?id=Produto)."

### 3. Você possui quantos funcionários ou pessoas envolvidas nesse negócio?

“Eu e meu sócio”.

### 4. Qual a arrecadação bruta do negócio mensalmente?

“Em torno de 10 mil por mês, é um negócio de pequeno porte”.

### 5. Como você costuma mensurar quanto o seu negócio obteve de crescimento? E de prejuízo?

“O meu termômetro é meu [estoque](Modeling/objeto?id=Estoque). Atualmente, por exemplo, a gente fez uma compra grande. Também é pela demanda e pela carteira de [cliente](Modeling/objeto?id=usuário) que a gente tem.”

### 6. Você costuma registrar em algum lugar os [produtos](Modeling/objeto?id=Produto) que são vendidos? Se sim, como funciona esse processo?

“Hoje eu tenho uma planilha excel que eu faço controle da venda, da compra, das minhas despesas fixas e variáveis. Toda venda é anotada na planilha."

### 7. Você mantém o registro de seu [estoque](Modeling/objeto?id=Estoque)? Se sim, como ele é feito hoje?

“O [estoque](Modeling/objeto?id=Estoque) eu tabulei o saldo das minhas mercadorias e na medida que eu vou vendendo eu visito essa planilha e vou dando baixa lá. (não é a mesma planilha usada para a venda).”

### 8. Imagine que você precisa saber se tem um certo [produto](Modeling/objeto?id=Produto) em [estoque](Modeling/objeto?id=Estoque) e rápido, mas você não está em sua loja. Como você procederia?

“Eu teria que ir na loja para saber se tenho o [produto](Modeling/objeto?id=Produto).”

### 9. Já aconteceu de você se enganar quanto ao número de [produtos](Modeling/objeto?id=Produto) que possui em [estoque](Modeling/objeto?id=Estoque)?

“Ixe, várias vezes. Inclusive com saldo errado, eu olho na minha planilha e eu tenho lá 10kg de uma erva, por exemplo, ou de um chá ou de um produto sendo que na prateleira não tem isso. Isso ocorre por que eu esqueci de dar [baixa no produto](Modeling/verbo?id=Baixa-em-Produto) ou alguém vendeu e não deu baixa.”

### 10. Já aconteceu de você não possuir um [produto](Modeling/objeto?id=Produto) e ele ser extremamente requerido pelos seus [clientes](Modeling/objeto?id=usuário)?

“A princípio não, a gente tem mantido o [estoque](Modeling/objeto?id=Estoque) adequado.”

### 11. Já aconteceu de você comprar um [estoque](Modeling/objeto?id=Estoque) de certo [produto](Modeling/objeto?id=Produto) de forma exagerada e ele não ser vendido com facilidade?

“Já.”

### 12. Qual a maior dificuldade que você enfrenta na parte administrativa de seu negócio?

“Com certeza o controle do [estoque](Modeling/objeto?id=Estoque). Coisas como não haver [produtos](Modeling/objeto?id=Produto) no [estoque](Modeling/objeto?id=Estoque) e eu achar que tinha e vice e versa por que não está registrado na planilha. E eu deixei de vender por que eu pensei que não tinha.”

### 13. De 1 a 10, qual a sua afinidade com aparelhos celulares e computadores? Costuma depender de alguém para realizar certas ações?

“10. Não preciso de ajuda, eu tenho 32 anos de mercado de trabalho e trabalhando com computadores, então não tenho dificuldade alguma de lidar com tecnologia.”

### 14. De 1 a 10, quanto a tecnologia faz parte do seu dia a dia nessa parte dos negócios?

“5. Faz parte do [controle de estoque](Modeling/verbo?id=Controle-de-Estoque) que é feito via excel, no controle de venda , no controle de cotação de mercadoria.”

### 15. Em quais processos hoje em sua empresa você acha que daria para envolver tecnologia?

“Nossa, praticamente tudo. [controle de estoque](Modeling/verbo?id=Controle-de-Estoque), controle de venda, cálculo da minha margem de lucro, cotação de mercadoria, emissão de pedido para [cliente](Modeling/objeto?id=usuário).”

## Gravação

<audio controls>
  <source src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/audios/interview/entrevistaIvanete.m4a" type="audio/mpeg">
</audio>

## Requisitos levantados

|                                     Id                                      |                Nome                 |
| :-------------------------------------------------------------------------: | :---------------------------------: |
|    [#RF03](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     [Adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao estoque      |
|    [#RF04](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |         [Consulta de estoque](Modeling/verbo?id=Consultar-Produto)         |
|    [#RF05](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        [Filtro](Modeling/verbo?id=Filtrar-Produtos) por categoria         |
|    [#RF07](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |     [Remoção de itens](Modeling/verbo?id=Baixa-em-Produto) do estoque     |
|    [#RF09](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |           Gerar planilha            |
|    [#RF10](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |         Histórico de vendas         |
|   [#RF012](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |       [Filtro](Modeling/verbo?id=Filtrar-Produtos) por nome e preço       |
|   [#RF014](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |        Plotagem de gráficos         |
|   [#RF015](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | Atualização instantânea de [estoque](Modeling/objeto?id=Estoque)  |
|   [#RF017](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | App para [consulta](Modeling/verbo?id=Consultar-Produto) fácil de [produto](Modeling/objeto?id=Produto) |
| [#RNF01](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |         Rapidez na [consulta](Modeling/verbo?id=Consultar-Produto)         |
| [#RNF02](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |         Gráficos didáticos          |
| [#RNF03](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |          [Consultas]((Modeling/verbo?id=Consultar-Produto)) remotas          |
