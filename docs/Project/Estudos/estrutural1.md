# Estudo Dirigido - GoF Estrutural 1

Um dos fatores que afetam o custo de manutenção/evolução de um sistema é a dependência gerada na interação entre os objetos desse sistema. Os padrões de projeto estruturais tem o objetivo de diminiuir essa dependência entre os objetos. Padrões desse tipo acabam alterando a estrutura do projeto no nível de classes.

## Adapter
Um objeto adapter é capaz de ser substituído por outro que desempenha as mesmas tarefas, porém com interfaces diferentes, isto é, como o próprio nome sugere, é adaptativo. Este padrão é bastante utilizado há algum tempo para pequenas adaptações de um modelo até mesmo em andamento. Esta característica possibilita maior flexibilidade e menor dependência.<br>
Na prática, um objeto que será servido por um segundo objeto que oferece tarefas complexas, pode passar por problemas ao ter este objeto servidor substituído.<br>
Para evitar problemas no objeto a ser servido, que não tem o objetivo de, por si só, ser complexo, é criado então um objeto intermediador. Este objeto intermediador simplifica, ou filtra, o que está sendo enviado pelo objeto servidor que foi substituído de forma que o objeto a ser servido nem mesmo sofre alterações. Desta forma é possível incrementar, em desempenho, níveis mais baixos sem afetar, em código, os níveis mais altos.<br>
<div style="text-align: center;">
    <img src="../../assets/img/estudo/gof-estrutural1/diagrama_de_classes_adapter.jpeg"/>
</div><br>

Como é possível visualizar no diagrama, a classe "Alvo" realiza solicitações a classe "Adaptado". Neste padrão de projeto, a classe "Adaptado" pode ser substituída por outra classe implementada por outra interface que desempenha as mesmas tarefas sem que seja modificada a classe "Alvo". A classe "Adaptador" realiza as alterações necessárias para que tudo esteja compreensível a classe "Alvo".

## Composite


## Referências
Livro: Use a Cabeça! Padrões de Projetos - **Elisabeth Freeman, Eric Freeman**, Editora Alta Books, Ano 2007 2ª Edição