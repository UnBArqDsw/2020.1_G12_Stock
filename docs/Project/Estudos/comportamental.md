# Estudo Dirigido - GoF Comportamental

## Padrão de Projeto
No desenvolvimento de Software é usual, que os desenvolvedores acumulem soluções para os problemas que resolvem com frequência, e essas soluções são difíceis de serem desenvolvidas e podem aumentar a produtividade, qualidade e uniformidade do software. Dessa forma surgiram os padrões de projeto.

Esse padrão foi descrito por Christopher Alexander, como: "Cada padrão descreve um problema que ocorre repetidas vezes em nosso ambiente, e então descreve o núcleo da solução para esse problema, de forma que você possa utilizar essa solução milhões de vezes sem usá-la do mesmo modo duas vezes" (CHRISTOPHER ALEXANDER, 1977).<br>
Além de Christopher, Gamma definiu Padrões de Software da sequinte forma: "descrevem soluções para produtos frequêntes no desenvolvimento de software." (Gamma 95)

## GoF Comportamental
O padrão GoF Comportamental resumidamente atua sobre qual o comportamento das entidades, ou seja, quais são as responsabilidades que são atribuidas a cada uma das entidades.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 02/10/2020 | 1.0 | Criação do documento | Gabriel Alves |

## Strategy
Em situações rotineiras no desenvolvimento de software, ocorre ocasiões onde se vê necessário uma gama de soluções/algoritmos para um problema específico, como por exemplo, uma ordenação. Existem diversos algoritmos de ordenação e cada um atua de forma otimizada para um contexto específico no software. Com isso, é necessário permitir de maneira simples a variação dos algoritmos utilizados na resolução de um problema específico.

Esse padrão é facilmente implementado utilizando as classes abstratas e/ou interfaces da programação orientada a objetos. O contexto relaciona-se com a parte mais abstrata, onde ainda não se sabe o como deve ser feito, apenas com quem. Dessa forma, caba a camada mais concreta a implementação do método em sí, fornecendo uma escalabilidade maior ao software, onde novas soluções para aquele contexto são facilmente acopladas ao sistema.

Segue um exemplo de um diagrama de classes, aplicado esse padrão. No contexto de uma compra em site de e-commerce.

![Strategy](../../assets/img/estudo/gof-comportamental/strategy.png)

### Pontos Positivos
- O software passa a ser extremamente escalável, pois a inserção de uma nova funcionalidade ligada a uma **strategy** passa a ser simples, além de não interferir nas outras soluções concretas já implementadas.
- A manutenção do código passa a ser mais simples, pois os erro erros são encontrados de maneira mais veloz, indo diretamente em sua respectiva **strategy** e em sua respectiva camada de implementação.

### Pontos Negativos
- Vários níveis de abstração, pode se fazer necessário em determinado contexto, porém isso poderá impactar significativamente na performance da aplicação.

### É possível adaptar a nossa forma de organização de projeto com esse padrão?
Sim, porém tem que avaliar quais serão as **strategys** e quantas camadas de abstração cada uma terá, pois impactará no desempenho do sistema.

### Quais documentos necessitam de refatoração para implementação deste padrão?
Principalmente Diagrama de Classes e o Projeto de Banco de Dados.


## Template Method
O **Template Method** foi pensado sobre uma ótica de processos, onde as etapas desse processo definem o coração desse padrão. Com isso, é definido os passos de maneira imutável, pois idependentes de como eles serão implementados sempre ocorrerão na mesma ordem.<br>
Para cada tipo de situação a formas diferentes de se resolver, porém cada uma delas obedece a mesma ordem das etapas.<br>
Os participantes do **Template Method** são as classes abstratas, onde simbolizam os processos e defiem qual será a ordem de cada etapa. E as classes concretas, onde irão implementar como farão cada etapa.

Para exemplificar, imagine uma fábrica de carros, onde as etapas do processo de fabricação é o mesmo, porém como é feito cada etapa varia para cada modelo de carro. Dessa forma o diagrama de classe ficaria da seguinte forma:

![Template_Method](../../assets/img/estudo/gof-comportamental/templateMethod.png)

### Pontos Positivos
- Com o **template method** existe a garantia de que as classes filhas irão respeitas a ordem de cada uma das etapas do processo.

### Pontos Negativos
- Limitado a problemas liagados a processos, pouco abrangente.

### É possível adaptar a nossa forma de organização de projeto com esse padrão?
Não vejo processos no projeto em que haja necessidade de respeitar uma ordem específica de execução das etapas.

### Quais documentos necessitam de refatoração para implementação deste padrão?
Diagrama de classes.