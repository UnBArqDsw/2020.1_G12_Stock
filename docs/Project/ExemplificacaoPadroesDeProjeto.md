# Exemplificação dos Padrões de Projeto

Foram realizados estudos dos padrões de projeto sugeridos pela professora assim como alguns padrões emergentes. O [estudo dirigido](Project/EstudoDirigido.md) foi realizado em duas sprints com revezamento entre os tipos de padrão de projeto. Após o estudo das técnicas foram feitas reuniões onde foram discutidos cada um dos padrões assim como viabilidade de aplicação em nosso projeto. As decisões estão documentadas no presente documento e representam uma decisão prévia que podem ser alteradas no decorrer da implementação da aplicação.

|    Data    | Versão |                     Descrição                      |    Autor(es)     |
| :--------: | :----: | :------------------------------------------------: | :--------------: |
| 10/10/2020 |  1.0   |                Criação do documento                |    Pedro Igor    |
| 10/10/2020 |  1.1   |                Adição das exemplificações          |       Todos      |    

## Utilizar o abstract factory method para criação dos produtos
Vimos que esse padrão é utilizado para evitar as várias instâncias de um classe e isso acontece em nossa classe Product, já que existe uma família de produtos perecíveis e não perecíveis. Pensamos em criar nossa fábrica de produtos e separá-las por perecíveis e não perecíveis. Esta classe já está presente no nosso diagrama, e seria utilizada para criar os tipos de produto descrito criando as famílias, definição que vimos nesse padrão.

## Utilizar o factory method para criação dos colaboradores
Um dos problemas que encontramos na definição do diagrama de classes foi: como definir os métodos de cada tipo de colaborador e além disso, como alterar seu nível de acesso? Pelo factory method teríamos uma classe factory Collaborator e 3 classes que implementam a classes factory tornando possível a remoção de dependência do objeto por sua classe e possibilitando essa alteração de tipo de colaborador.

## Utilizar o adaptive para criação dos gráficos
Um dos passos para plotagem de gráficos é o tratamento de informações. Essa informação pode chegar de diversas formas possíveis porém há poucas formas de entrada no gráfico em si. Poderíamos utilizar uma classe adaptador que, independentemente do que a classe que gera informações para os gráficos retorne, seja capaz de traduzir tudo e mandar para o gráfico. Dessa forma seria possível alterar até mesmo os algoritmos utilizados assim como cálculos e tudo seria adaptado para a classe do gráfico por essa classe intermediadora.

## Utilizar o controller para definição das classes
O Controller se trata de atribuir a responsabilidade de receber ou tratar uma mensagem de evento do sistema a uma classe. No projeto utilizaremos padrão de MVC (Model-View-Controller), então para o uso de Controller é feita uma classe para delegar a outros objetos o trabalho que precisa ser feito, coordena ou controla a atividade. Funciona como uma camada que não faz muito trabalho sozinho normalmente.

## Utilizar o state para definição do estado do estoque
O objetivo principal é o controle de estoque e esse controle tem todo um contexto de entrada e saída de produtos, com regras diferentes de saída. É de suma importância para o usuário saber o estado de desse estoque como por exemplo, cheio, metade, estado crítico e vazio. Acreditamos que o GoF State consegue atender essa necessidade.