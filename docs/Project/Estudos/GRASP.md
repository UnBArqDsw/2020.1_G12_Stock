# Estudo Dirigido - GRASP

GRASP significa Padrões de Software para Atribuição de Responsabilidade Geral e consiste em diretrizes para atribuir responsabilidade a classes e objetos em projeto orientado a objetos.

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 30/09/2020 | 1.0 | Estudos GRASP - Criador e Especialista | Sofia Patrocínio |
| 02/10/2020 | 1.1 | Criação do documento | Sofia Patrocínio |
| 02/10/2020 | 1.2 | Adição das explicações dos padrões | Sofia Patrocínio |
| 03/10/2020 | 1.3 | Adição dos pontos positivos e negativos e documentos pra refatoração | Sofia Patrocínio |

## Criador ou Creator

Ao avaliar o modelo, primeiro questionamento é quais classes possuem as responsabilidades de criar instâncias. Seu objetivo é definir como criador o objeto que precise ser conectado ao objeto criado em algum evento.

Atribua à classe B a responsabilidade de criar uma nova instância da classe A se uma das seguintes condições for verdadeira:

- B "contém" A ou é uma composição de A
- B registra A
- B usa A de maneira muito próxima
- B tem dados iniciais de A, os quais serão passados para A quando este for criado. B é um "especialista" em relação à criação de A

*Se a relação for de agregação é melhor, pois o código está menos acoplado. Se for de composição, a parte só existe se o todo existir.*

### Pontos Positivos e Negativos

- Positivos
    - Favorece o acoplamento fraco

### É possível adaptar a nossa forma de organização de projeto com esse padrão? Quais documentos necessitam de refatoração para implementação deste padrão?

Sim, principalmente diagramas de classe, de sequência e comunicação.

## Especialista

Criador é um especialista em criação de instâncias. Já o Especialista é um padrão que se preocupa em atribuir responsabilidades para a entidade mais especialista em um dado aspecto, não apenas de criação de instâncias, mas de todos os aspectos do sistema.

- Quem é a melhor entidade para calcular algo?
- Quem é a melhor entidade para ordenar algo?
- Quem é a melhor entidade para cadastrar algo?

### Pontos Positivos e Negativos

- Positivos
  
    - Mantém encapsulamento, favorece o acoplamento fraco.
    - Comportamento fia distribuído entre as classes que têm a informação necessária, favorece a alta coesão.

- Negativos
    - Não é indicado quando aumenta o acoplamento e reduz coesão.

### É possível adaptar a nossa forma de organização de projeto com esse padrão? Quais documentos necessitam de refatoração para implementação deste padrão?

Sim, diagramas de classe, de sequência e comunicação e de entidades de banco de dados.

## Baixo Acoplamento ou Acoplamento Fraco

Determina que as classes não devem depender de objetos concretos, mas sim de abstrações. O baixo acoplamento é um padrão de avaliação que determina como atribuir responsabilidades de suporte:

- Menor dependência entre as classes
- Mudança em uma classe com menor impacto em outras
- Maior potencial de reutilização
- Facilidade na manutenção

### Pontos Positivos e Negativos

- Positivos
    
    - Uma classe fracamente acoplada não é afetada (ou pouco afetada por mudanças em outras classes
    - Simples de entender isoladamente
    - Reuso mais fácil

### É possível adaptar a nossa forma de organização de projeto com esse padrão? Quais documentos necessitam de refatoração para implementação deste padrão?

Sim, o uso de padrões de projeto GRASP influenciam diretamente no baixo acoplamento.

## Alta Coesão

Atribuir de forma coerente as responsabilidades das classes, mantendo os objetos adequadamente focados, gerenciáveis e compreensíveis.

- Mais	clareza	e	facilidade	de	compreensão	no	
projeto	
- Simplificação	de	manutenção	e	acréscimo de	funcionalidade/melhorias	
- Favorecimento	do	acoplamento	fraco	
- Aumento	no	potencial	de	reutilização

### Pontos Positivos e Negativos

- Positivos

    - Melhor claridade e facilidade de compreensão do projeto
    - Simplificação da manutenção
    - Frequentemente vai mão na mão com acoplamento fraco
    - Com granularidade baixa e funcionalidade bem focada, aumenta o reuso

### É possível adaptar a nossa forma de organização de projeto com esse padrão? Quais documentos necessitam de refatoração para implementação deste padrão?

Sim, o uso de padrões de projeto GRASP influenciam diretamente na alta coesão.

## Controlador ou Controller 

Objeto responsável por receber e lidar com um evento do sistema. Os controladores devem somente coordenar a tarefa, delegando sua execução para os outros objetos do sistema.
- O uso de controladores *Facade* é válido somente quando existem poucos eventos do sistema.

### Pontos Positivos e Negativos

- Positivos

    - Aumento das possibilidades de	reutilização de	classes	
    - Aumento das possibilidades de	interfaces “plugáveis”		
    - Conhecimento do estado do	caso de	uso	– controlador	
pode armazenar estado do caso de uso, garantindo a sequência	correta	de execução de	operações	

### É possível adaptar a nossa forma de organização de projeto com esse padrão? Quais documentos necessitam de refatoração para implementação deste padrão?

O padrão Controller já está sendo utilizado em nosso projeto, revisar diagrama de componentes.

## Polimorfismo

As responsabilidades são atribuídas a abstrações. Lida com o comportamento com base no tipo (classe), mas que não usa uma instrução *if ou *switch, com o uso dele, as seções de código se tornam menos acopladas e mais coesas.

### Pontos Positivos e Negativos

- Positivos

    - Acoplamento de código
    - Facilidade de manutenção
    - Facilidade de inserção de um novo tipo de autorização

### É possível adaptar a nossa forma de organização de projeto com esse padrão? Quais documentos necessitam de refatoração para implementação deste padrão?

O padrão Polimorfismo já está sendo utilizado em nosso projeto, revisar diagrama de classes.

## Invenção Pura ou Fabricação Própria

Atribuição de um conjunto coeso de responsabilidades à classes artificiais que não representa um conceito no domínio da aplicação, uma classe fictícia que mantenham alta coesão e baixo acoplamento e o reuso.

### Pontos Positivos e Negativos

- Positivos

    - Remove as características não coesas das classes do domínio de negócio
    - Cria classes muito coesas com essas características

- Negativos

    - Cria classes altamente funcionais, que não fazem parte da realidade
    - Se utilizado em excesso, poderá transformar um sistema OO em um sistema orientado a eventos

### É possível adaptar a nossa forma de organização de projeto com esse padrão? Quais documentos necessitam de refatoração para implementação deste padrão?

É possível adaptar, esse padrão é relacionado fortemente aos GOF's criacionais e se aplicaria melhor em um projeto com maior escopo.


## Indireção

Atribuição de um objeto intermediário que faça a mediação entre componentes ou serviços de modo que eles não sejam diretamente acoplados. Com o uso do objeto intermediário entre dois componentes, passam a não depender mais um do outro, mas sim da indireção.

*A maior parte dos problemas em Ciência da Computação pode ser resolvida por um nível adicional de indireção* - citação em Larman, p 427.

Alguns exemplos de problemas resolvidos com outro nível de indireção:

- Implementação de polimorfismo 
- Um ponteiro para uma matriz de pontos de método.
- Passar por referência.
- Listas vinculadas.
- Uma matriz multidimensional onde as linhas / colunas têm tamanhos diferentes,tratando um ponteiro de cabeça da mesma forma que um ponteiro em um registro.
- Herança em linguagens de protótipo, como Javascript.

### Pontos Positivos e Negativos

- Positivos

    - Uma classe fracamente acoplada não é afetada (ou pouco afetada por mudanças em outras classes
    - Simples de entender isoladamente
    - Reuso mais fácil

### É possível adaptar a nossa forma de organização de projeto com esse padrão? Quais documentos necessitam de refatoração para implementação deste padrão?

Sim, diagramas de classe, de sequência e comunicação e de entidades de banco de dados.

## Varições Protegidas

Diminuir que variações ou instabilidades em elementos tenham impacto indesejado em outros elementos. Soluções:

- Identificar pontos de variação ou instabilidades potenciais.
- Atribuir responsabilidades para criar uma interface estável em volta desses pontos.
- Encapsulamento, interfaces, polimorfismo, indireção e padrões:
máquinas virtuais e brokers são motivados por este princípio.
- Evite enviar mensagens a objetos muito distantes.

### Pontos Positivos e Negativos

- Positivos

    - Uma classe fracamente acoplada não é afetada (ou pouco afetada por mudanças em outras classes
    - Simples de entender isoladamente
    - Reuso mais fácil

### É possível adaptar a nossa forma de organização de projeto com esse padrão? Quais documentos necessitam de refatoração para implementação deste padrão?

Sim, diagramas de classe, de sequência e comunicação e de entidades de banco de dados.


## Referências
- Apresentação: GRASP: Designing Objetos com Responsabilidades  - MC 426 IC Unicamp – M. Cecilia C. Baranauskas - <https://www.ic.unicamp.br/~ariadne/mc436/1s2017/Lar16GRASP.pdf>. Último acesso em 02/10/2020.

- Apresentação: Padrões GRASP - <http://www.facom.ufu.br/~bacala/ESOF/05a-Padr%C3%B5es%20GRASP.pdf>. Último acesso em 03/10/2020.