# Exemplificação dos Padrões de Projeto

Foram realizados estudos dos padrões de projeto sugeridos pela professora assim como alguns padrões emergentes. O [Estudo Dirigido](Project/EstudoDirigido.md) foi realizado em duas sprints com revezamento entre os tipos de padrão de projeto. Após o estudo das técnicas foram feitas reuniões onde foram discutidos cada um dos padrões assim como viabilidade de aplicação em nosso projeto. As ideias estão documentadas no presente documento e representam uma decisão prévia que podem ser alteradas no decorrer da implementação da aplicação. Algumas das ideias podem não ser aplicadas e o que foi aplicado estará melhor documentado em [**Padrões de Projeto**](Index/projectPatternsIndex.md).

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 10/10/2020 | 1.0 | Criação do documento | Pedro Igor |
| 10/10/2020 | 1.1 | Adição das exemplificações | Todos |
| 10/10/2020 | 1.2 | Adição dos léxicos | Pedro Igor |
| 19/10/2020 | 1.3 | Correção de erros e adição da link para as aplicações utilizadas | Micaella Gouveia |


## Utilizar o Abstract Factory Method para criação dos produtos
Vimos que esse padrão é utilizado para evitar as várias instâncias de um classe e isso acontece em nossa classe [Product](Modeling/objeto.md?id=Produto), já que existe uma família de [produtos](Modeling/objeto.md?id=Produto) perecíveis e não perecíveis. Pensamos em criar nossa fábrica de [produtos](Modeling/objeto.md?id=Produto) e separá-las por perecíveis e não perecíveis. Esta classe já está presente no nosso diagrama, e seria utilizada para criar os tipos de [produto](Modeling/objeto.md?id=Produto) descrito criando as famílias, definição que vimos nesse padrão.

## Utilizar o Factory Method para criação dos colaboradores
Um dos problemas que encontramos na definição do diagrama de classes foi: como definir os métodos de cada [tipo de colaborador](Modeling/objeto.md?id=papéis-dos-colaboradores) e além disso, como alterar seu [nível de acesso](Modeling/objeto.md?id=papéis-dos-colaboradores)? Pelo Factory Method teríamos uma classe factory Collaborator e 3 classes que implementam a classes factory tornando possível a remoção de dependência do objeto por sua classe e possibilitando essa alteração de [tipo de colaborador](Modeling/objeto.md?id=papéis-dos-colaboradores).

## Utilizar o Adapter para criação dos gráficos
Um dos passos para plotagem de gráficos é o tratamento de informações. Essa informação pode chegar de diversas formas possíveis porém há poucas formas de entrada no gráfico em si. Poderíamos utilizar uma classe Adaptador que, independentemente do que a classe que gera informações para os gráficos retorne, seja capaz de traduzir tudo e mandar para o gráfico. Dessa forma seria possível alterar até mesmo os algoritmos utilizados assim como cálculos e tudo seria adaptado para a classe do gráfico por essa classe intermediadora.

## Utilizar o Controller para definição das classes
O Controller se trata de atribuir a responsabilidade de receber ou tratar uma mensagem de evento do sistema a uma classe. No projeto utilizaremos padrão de MVC (Model-View-Controller), então para o uso de Controller é feita uma classe para delegar a outros objetos o trabalho que precisa ser feito, coordena ou controla a atividade. Funciona como uma camada que não faz muito trabalho sozinho normalmente.

## Utilizar o State para definição do estado do estoque
O objetivo principal é o [controle de estoque](Modeling/verbo?id=controle-de-estoque) e esse controle tem todo um contexto de [entrada e saída](Modeling/verbo?id=fluxo) de [produtos](Modeling/objeto.md?id=Produto), com regras diferentes de [saída](Modeling/verbo?id=baixa-em-produto). É de suma importância para o usuário saber o estado de desse [estoque](Modeling/objeto.md?id=estoque) como por exemplo, cheio, metade, estado crítico e vazio. Acreditamos que o GoF State consegue atender essa necessidade.

## Utilizar o Decorator para as ações principais de Crud. 

Aqui, o objetivo é criar uma nova camada para os métodos principais que o [Sequelize](Modeling/objeto?id=Sequelize) oferece como findAll, findOne, create e assim por diante para utilização pelas controllers, porém cada uma irá alterar o comportamento de acordo com sua necessidade. Para isso, utilizaremos o método Decorator, onde o Decorator Base irá implementar os métodos do [Sequelize](Modeling/objeto?id=Sequelize) e assim cada controller poderá herdar desse Decorator Base. 