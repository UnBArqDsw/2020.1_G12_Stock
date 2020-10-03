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

![DiagramaComportamental](../../assets/img/estudo/gof-criacional/strategy.png)

### Pontos Positivos
- O software passa a ser extremamente escalável, pois a inserção de uma nova funcionalidade ligada a uma **strategy** passa a ser simples, além de não interferir nas outras soluções concretas já implementadas.
- A manutenção do código passa a ser mais simples, pois os erro erros são encontrados de maneira mais veloz, indo diretamente em sua respectiva **strategy** e em sua respectiva camada de implementação.

### Pontos Negativos
- Vários níveis de abstração, pode se fazer necessário em determinado contexto, porém isso poderá impactar significativamente na performance da aplicação.

### É possível adaptar a nossa forma de organização de projeto com esse padrão?
Sim, porém tem que avaliar quais serão as **strategys** e quantas camadas de abstração cada uma terá, pois impactará no desempenho do sistema.

### Quais documentos necessitam de refatoração para implementação deste padrão?
Principalmente Diagrama de Classes e o Projeto de Banco de Dados.