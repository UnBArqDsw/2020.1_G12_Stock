# Estudo Dirigido - GoF Estrutural 1

Um dos fatores que afetam o custo de manutenção/evolução de um sistema é a dependência gerada na interação entre os objetos desse sistema. Os padrões de projeto estruturais tem o objetivo de diminiuir essa dependência entre os objetos. Padrões desse tipo acabam alterando a estrutura do projeto no nível de classes. Será apresentado de dois padrões de projeto GOF(Gang of Four) Estruturais, o Adapter e o Composite.

## Adapter
Um objeto adapter é capaz de ser substituído por outro que desempenha as mesmas tarefas, porém com interfaces diferentes, isto é, como o próprio nome sugere, é adaptativo. Este padrão é bastante utilizado há algum tempo para pequenas adaptações de um modelo até mesmo em andamento. Esta característica possibilita maior flexibilidade e menor dependência.<br>
Na prática, um objeto que será servido por um segundo objeto que oferece tarefas complexas, pode passar por problemas ao ter este objeto servidor substituído.<br>
Para evitar problemas no objeto a ser servido, que não tem o objetivo de, por si só, ser complexo, é criado então um objeto intermediador. Este objeto intermediador simplifica, ou filtra, o que está sendo enviado pelo objeto servidor que foi substituído de forma que o objeto a ser servido nem mesmo sofre alterações. Desta forma é possível incrementar, em desempenho, níveis mais baixos sem afetar, em código, os níveis mais altos.<br>
<div style="text-align: center;">
    <img src="../../assets/img/estudo/gof-estrutural1/diagrama_de_classes_adapter.jpeg"/>
</div><br>

Como é possível visualizar no diagrama, a classe "Alvo" realiza solicitações a classe "Adaptado". Neste padrão de projeto, a classe "Adaptado" pode ser substituída por outra classe implementada por outra interface que desempenha as mesmas tarefas sem que seja modificada a classe "Alvo". A classe "Adaptador" realiza as alterações necessárias para que tudo esteja compreensível a classe "Alvo".

## Composite
Cada objeto de um conjunto de objetos composite que fazem parte de uma relação todo-parte são tratados sem distinção. O objetivo é que por mais que haja complexidade e diferença entre cada um dos objetos, em determinado nível estejam todos sem distinção no nível analisado.<br>
Na prática, uma interface, ou até mesmo uma classe abstrata, é implementada por diversas outras classes que são tratadas sem distinção. No entanto, uma dessas classes tem a capacidade de inserir ou remover outras classes nesse nível de implementação. Esta classe, com estes métodos, é determinada composite pois tem a capacidade de compor as classes que implementam a classe inicial.
<div style="text-align: center;">
    <img src="../../assets/img/estudo/gof-estrutural1/diagrama_de_classes_composite.png"/>
</div><br>

Como é possível visualizar no diagrama, a classe "Arquivo" pode ser implementada por diversas outras classes de tipos diferentes de arquivos. Todas as classes que implementam a classe principal estão, nesta abstração, em um mesmo nível. No entanto, a classe "ArquivoComposite" tem a capacidade de adicionar e remover classes que estão neste mesmo nível de abstração e também implementam a classe principal. Não há distinções entre as classes resultantes da classe Composite.
## Referências
- Livro: Use a Cabeça! Padrões de Projetos - **Elisabeth Freeman, Eric Freeman**, Editora Alta Books, Ano 2007 2ª Edição

- Site: **Thiengo** - Visão geral do livro "Use a Cabeça! Padrões de Projetos - Elisabeth, Eric Freeman" - <https://www.thiengo.com.br/use-a-cabeca-padroes-de-projetos> Último acesso em 02/10/2020.

- Site: **Thiengo** - Padrões de projeto Adapter - <https://www.thiengo.com.br/padrao-de-projeto-adapter> Último acesso em 02/10/2020

- **Marcos Brizeno**: Mão na massa - Composite - <https://brizeno.wordpress.com/category/padroes-de-projeto/composite/> Último acesso em 02/10/2020