# Estudo Dirigido - GoF Estrutural

Um dos fatores que afetam o custo de manutenção/evolução de um sistema é a dependência gerada na interação entre os objetos desse sistema. Os padrões de projeto estruturais tem o objetivo de diminiuir essa dependência entre os objetos. Padrões desse tipo acabam alterando a estrutura do projeto no nível de classes. Serão apresentados dois padrões de projeto GOF(Gang of Four) Estruturais, o Adapter e o Composite.

## Histórico de Revisões

|    Data    | Versão |                            Descrição                             |  Autor(es)   |
| :--------: | :----: | :--------------------------------------------------------------: | :----------: |
| 02/10/2020 |  1.0   |           Criação do documento e inserção dos estudos.           |  Pedro Igor  |
| 02/10/2020 |  1.1   |      Adição das respostas as perguntas do estudo dirigido.       |  Pedro Igor  |
| 02/10/2020 |  1.2   |                    Inserção das referências.                     |  Pedro Igor  |
| 04/10/2020 |  1.3   | Adição dos padrões proxy, decorator, facade, flyweight e bridge. | Gabriel Davi |

## Adapter

Um objeto adapter é capaz de ser substituído por outro que desempenha as mesmas tarefas, porém com interfaces diferentes, isto é, como o próprio nome sugere, é adaptativo. Este padrão é bastante utilizado há algum tempo para pequenas adaptações de um modelo até mesmo em andamento. Esta característica possibilita maior flexibilidade e menor dependência.<br>
Na prática, um objeto que será servido por um segundo objeto que oferece tarefas complexas, pode passar por problemas ao ter este objeto servidor substituído.<br>
Para evitar problemas no objeto a ser servido, que não tem o objetivo de, por si só, ser complexo, é criado então um objeto intermediador. Este objeto intermediador simplifica, ou filtra, o que está sendo enviado pelo objeto servidor, que foi substituído, de forma que o objeto a ser servido possa não sofrer alterações. Desta forma é possível incrementar, em desempenho, níveis mais baixos sem afetar, em código, os níveis mais altos.<br>

<div style="text-align: center;">
    <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/img/estudo/gof-estrutural1/diagrama_de_classes_adapter.jpeg"/>
</div><br>

Como é possível visualizar no diagrama, a classe "Alvo" realiza solicitações a classe "Adaptado". Neste padrão de projeto, a classe "Adaptado" pode ser substituída por outra classe implementada por outra interface que desempenha as mesmas tarefas sem que seja modificada a classe "Alvo". A classe "Adaptador" realiza as alterações necessárias para que tudo esteja compreensível a classe "Alvo".

### Pontos positivos

- Permite atualizações catastróficas sem aumento de complexidade em níveis superiores.

- Permite atualizações com o projeto em andamento.

- Facilita manutenção por permitir mais de uma forma de implementar a mesma funcionalidade.

### Pontos negativos

- Excesso de classes e implementações para projetos relativamente pequenos.

- Domínio de todo o fluxo e comunicação entre os componentes para a implementação de uma classe Adapter.

### É possível adaptar a nossa forma de organização de projeto com este padrão?

Sim, é possível. A implementação parece ser simples e, aparentemente, é necessário subdividir ao máximo determinada ação de forma que seja possível adaptar as subdivisões do fluxo. Dessa forma, uma tarefa A é subdivida em 3 tarefas A, B, C onde há uma tarefa responsável por alimentar, outra por filtrar e ainda outra por simplesmente ser alimentada.

### Quais documentos necessitam de refatoração para implementação deste padrão?

Como ainda não iniciamos a parte prática do projeto não é necessário alterações em código. Mas como a implementação de diagramas referentes ao código já foram implementados em sprints anteriores, é necessária revisão dos diagramas:

- Diagrama de Classes: Identificação de tarefas complexas realizadas por algumas classes e substituição por tarefas com mediação de classes Adapter.

- Diagrama de Sequência: Inserção das classes Adapter mediadoras definidas no diagrama de classes. Não parece ter modificações estruturais graves, apenas passos extras na execução de métodos.

- Diagrama de Comunicação: Inserção das classes Adapter mediadoras definidas no diagrama de classes. Não parece ter modificações estruturais graves, apenas passos extras na comunicação entre classes. Pode não ser necessária refatoração se for considerado um nível mais prático na elaboração deste diagrama.

## Composite

Cada objeto de um conjunto de objetos composite que fazem parte de uma relação todo-parte são tratados sem distinção. O objetivo é que por mais que haja complexidade e diferença entre cada um dos objetos, em determinado nível, estejam todos sem distinção.<br>
Na prática, uma interface, ou até mesmo uma classe abstrata, é implementada por diversas outras classes que são tratadas sem distinção. No entanto, uma dessas classes tem a capacidade de inserir ou remover outras classes nesse nível de implementação. Esta classe, com estes métodos, é determinada Composite pois tem a capacidade de compor as classes que implementam a classe inicial.

<div style="text-align: center;">
    <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/img/estudo/gof-estrutural1/diagrama_de_classes_composite.png"/>
</div><br>

Como é possível visualizar no diagrama, a classe "Arquivo" pode ser implementada por diversas outras classes de tipos diferentes de arquivos. Todas as classes que implementam a classe principal estão, nesta abstração, em um mesmo nível. No entanto, a classe "ArquivoComposite" tem a capacidade de adicionar e remover classes que estão neste mesmo nível de abstração e também implementam a classe principal. Não há distinções, neste nível, entre as classes resultantes da classe Composite.

### Pontos positivos

- Permite uma manipulação (criação e remoção) de classes "personalizáveis".

- Permite abstração até determinado ponto, porém consegue conciliar detalhamento em cada classe.

### Ponto negativos

- Entendimento do padrão parece muito complexo para aplicação adequada.

- Em uma aplicação minimamente equivocada pode aumentar ainda mais dificuldade de implementação.

- Alteração completa na modelagem de bancos de dados que fizemos.

### É possível adaptar a nossa forma de organização de projeto com este padrão?

Sim, é possível mas parece ser muito difícil. Classes como "Produto" seriam decompostas em classes como "Smartphone", "Tv", "Geladeira" além de uma classe "ProdutoComposite" que teria a capacidade de adicionar e remover classes "folhas".

### Quais documentos necessitam de refatoração para implementação deste padrão?

Como ainda não iniciamos a parte prática do projeto não é necessário alterações em código. Mas como a implementação de diagramas referentes ao código já foram implementados em sprints anteriores, é necessária revisão dos diagramas:

- Diagrama de Classes: Generalização de algumas classes para que sejam implementadas por classes "folhas" adicionadas por uma classe Composite. A refatoração nesse diagrama não parece ser muito complicada.

- Diagrama de Sequência: Inserção das classes "folhas" ao diagrama deixando claro que implementam as classes generalizadas.

- Diagrama de Comunicação: Inserção das classes "folhas" ao diagrama deixando claro que implementam as classes generalizadas. Não parece ter modificações estruturais graves, especificação de que a classe que realizará determinadas ações, será uma classe que implementa uma principal.

- Diagrama Entidade Relacionamento: Teríamos que pensar em uma nova estratégia de modelagem já que a classe "Produto", por exemplo, seria simplificada comparada ao estado atual. Porém, como representar implementações de classes folhas em uma base de dados?

## Flyweight

O método de flyweight é uma otimização. Ele vem para solucionar o problema de gerenciamento de memória em programas que consomem muito RAM durante sua execução devido ao uso repetitivo de um objeto em diferentes contextos do programa. Para isso, cria-se uma classe "Flyweight" que será responsável por guardar as instâncias do objeto que antes era repetida excessivamente durante todo o programa e compartilhá-la via método para as demais partes do sistema.

<div style="text-align: center;">
    <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/img/estudo/gof-estrutural1/flyweight.png"/>
</div><br>

É possível ver no diagrama, temos uma classe flyweight que guarda o objeto que será repetido no sistema. O FlywightFactory será responsável por guardar todas as instâncias de uma classe flyweight e compartilhá-la por todo o Context que deseja utilizá-la.

### Pontos positivos

É uma ótima forma de salvar processamento de memória RAM.

### Pontos negativos

- Talvez você estará trocando otimização de RAM por mais ciclos de CPU se uma classe que consome flyweight(contexto) precisar ser recriada se outro contexto distinto chamar a classe flyweight.

- Aumenta a complexidade do código.

### É possível adaptar a nossa forma de organização de projeto com este padrão?

Sim, é possível se as classes produtos de nosso sistema sempre manter um padrão para seus atributos, como por exemplo feedback. Porém, esse método é recomendado para quando há uma quantidade massiva de dados a serem processados, o que não será nosso caso.

### Quais documentos necessitam de refatoração para implementação deste padrão?

O primeiro passo seria analisar qual classe seria apropriada para esse método. Nesse caso, considero a classe produto uma boa candidata.

- Diagrama de classes: Se fosse o caso, daria para extrair algum estado do feedback, como seu tipo como já é feito, porém haveria uma factory entre o feedback e seu tipo. O mesmo se aplica para a relação entre produto e descrição.

- Diagrama de sequência: Nesse caso, o feedback não chamaria o typeFeedback e sim o método da factory que guarda todas as instâncias de typeFeedck, passando somente suas especificações de qual type deseja receber.

- Diagrama de comunicação: Semelhante a alteração necessária no diagrama de sequência.

## Proxy

Método que possibilita você adicionar um objeto substituto para outro objeto. Um objeto proxy controla o acesso ao objeto original, assim dando a possibilidade da execução de algumas ações antes ou depois do acesso ao objeto original.

<div style="text-align: center;">
    <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/img/estudo/gof-estrutural1/proxy.png"/>
</div><br>

Aqui, podemos ver que antes de passar por um serviço, o client passa por um proxy, que deve ter uma interface idêntica ao serviço original a ser chamado. O proxy possui uma relação de agregação com o serviço original, pois o mesmo existe idenpendente do proxy.

### Pontos positivos

- Controle de acesso pelos clients.

- Princípio aberto/fechado. Pois podemos usar quantos proxy forem necessários sem impactar no objeto original.

### Pontos negativos

- Código mais complicado pois há necessidade da criação de várias classes.

- Resposta final para o setvidor pode demorar mais tempo.

### É possível adaptar a nossa forma de organização de projeto com este padrão?

Sim, o proxy possui diversos usos e por isso poderia ser aplicado em nosso projeto. Por exemplo, para limitar o número de chamadas da criação de produtos em estoque, proteger algumas rotas do sistema, criar cache em listagem de produtos e assim por diante. Há também a possibildade de limitar a chamada para a adição de produtos, caso pessoas mal intencionadas descubram a rota e façam chamadas excessivas que irão causar uma sobrecarga em nossos bancos de dados.

### Quais documentos necessitam de refatoração para implementação deste padrão?

- Diagrama de classes: Poderia ser usando um proxy para criar cache que iria retornar a lista de categorias, para isso, uma interface de categoria poderia ser criada inicialmente e seria implementada pela classe de categoria original e também seu proxy. O mesmo se aplica para a listagem de produtos e lotes.

- Diagrama de sequência: Para o caso de baixa em produto, um proxy seria chamado para a listagem de produtos, lotes e categorias e o mesmo retornaria o resultado de listagem de produtos. Em adição de produto, haveria um proxy entre produto e seu lote, com a função de analisar a quantidade de requisições por segundo e assim barrar possíveis sobrecargas em nosso banco de dados.

- Diagrama de comunicação: Semelhante a alteração necessária no diagrama de sequência.

## Decorator

O decorator permite adicionar novos comportamentos a objetos através da adição de uma nova camada de um objeto externo que possui os comportamentos que deseja-se ser acrescentados.

<div style="text-align: center;">
    <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/img/estudo/gof-estrutural1/decorator.png"/>
</div><br>

Aqui, podemos ver que há um decorator base, que irá servir como uma ponte entre o client e os decorators que realmente irão alterar o comportamento do objeto concreto. Todos devem implementar a mesma interface.

### Pontos positivos

- Podemos extender comportamento de objetos sem precisar criar novas subclasses.

- Possibilidade de adicionar ou remover comportamentos em tempo de execução.

- Possibilidade de adicionar diversos comportamentos.

- Princípio da responsabilidade única. Cada decorator realizará seu comportamento como foi projetado.

### Pontos negativos

- Difícil de remover uma classe que foi criada como decorator.

- Código pode ficar bem confuso a princípio.

### É possível adaptar a nossa forma de organização de projeto com este padrão?

Sim, um lugar em que seria uma ótima oportunidade de para adição de decorators seria na classe de análise que retorna dos dados para a geração de gráficos em nossa aplicação. Com isso, se for necessário a criação de novos comportamentos, somente seria necessário a criação de decorators que iria extender a classe de Análise e então implementar o novo comportamento. Atualmente, essa classe possui três métodos, cada um poderia se tornar um decorator que iria implementar sua própria tratativa de dados.

### Quais documentos necessitam de refatoração para implementação deste padrão?

- Diagrama de classes: a classe Analysis poderia ter uma interface que possuiria o método generateData para geração dados para gráficos. Seria assim criados os decorators de AnalysisFlow, AnalysisCollaborator, AnalysisCategory que implementariam seu próprio método generateData baseado em suas peculiaridades.

- Diagrama de comunicação: Admin poderia se comunicar agora com os decorators de produto, colaborador e categoria sem precisar depender de Analisys.

## Bridge

Esse padrão permite a divisão de uma classe em implementações menores que podem ser desenvolvidas indenpendentes umas das outras.

<div style="text-align: center;">
    <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/img/estudo/gof-estrutural1/decorator.png"/>
</div><br>

Aqui, podemos ver que há uma separação em uma interface de algum parametro ou atributo. O bridge é bem simples porém muito eficaz pois possibilita a adição e modificação de quantas classes forem necessárias.

### Pontos positivos

- Independencia entre diferentes partes.

- O client não possui acesso direto aos detalhes de implementação das classes mais específicas

- Princípio aberto/fechado. Pois podemos implementar diferentes classes em que a classe mais abstrata irá basear seu comportamento.

- Princípio da responsabilidade única.

### Pontos negativos

Aumenta a complexidade do código.

### É possível adaptar a nossa forma de organização de projeto com este padrão?

De certa forma, já usamos esse padrão quando separamos as categorias em uma classe separada e produto e também para o tipo de feedback.

### Quais documentos necessitam de refatoração para implementação deste padrão?

Como já usamos esse padrão, acredito que não há necessidade de mudanças em nossos diagramas.

## Facade

Facade fornece uma interface simplificada para uma biblioteca, framework ou qualquer conjunto complexo de classes. Esse método é extremamente eficaz quando você deseja usar uma biblioteca externa que possui diversar funcionalidades, porém você precisa somente de uma pequena porção dessas funcionalidades.

<div style="text-align: center;">
    <img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/img/estudo/gof-estrutural1/facade.png"/>
</div><br>

Aqui, a classe facade irá instanciar somente a classe que interessa para o client e implementar o método que irá executar alguma ação em cima disso.

### Pontos positivos

- Isola a complexidade de um sistema maior

### Pontos negativos

- Há a possibilidade de uma classe facade se tornar muito grande e complexa, realizando diversas ações.

### É possível adaptar a nossa forma de organização de projeto com este padrão?

Não iremos a princípio utilizar bibliotecas complexas a ponto de se fazer necessário a utilização desse padrão

### Quais documentos necessitam de refatoração para implementação deste padrão?

Nenhum.

## Referências

- Livro: Use a Cabeça! Padrões de Projetos - **Elisabeth Freeman, Eric Freeman**, Editora Alta Books, Ano 2007 2ª Edição

- Site: **Thiengo** - Visão geral do livro "Use a Cabeça! Padrões de Projetos - Elisabeth, Eric Freeman" - <https://www.thiengo.com.br/use-a-cabeca-padroes-de-projetos> Último acesso em 02/10/2020.

- Site: **Thiengo** - Padrões de projeto Adapter - <https://www.thiengo.com.br/padrao-de-projeto-adapter> Último acesso em 02/10/2020

- Site: **Refactoring Guru** - <https://refactoring.guru/design-patterns> Último acesso em 04/10/2020

- **Marcos Brizeno**: Mão na massa - Composite - <https://brizeno.wordpress.com/category/padroes-de-projeto/composite/> Último acesso em 02/10/2020
