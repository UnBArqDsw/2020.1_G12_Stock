# Reutilização de Software

Neste módulo, será melhor explicado o que é a Reutilização de Software.

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 05/11/2020 | 1.0 | Criação do documento e adição de explicação geral | Sofia Patrocínio |
| 06/11/2020 | 1.1 | Adição do tópico de frameworks | Sofia Patrocínio |
| 07/11/2020 | 1.2 | Adição dos tópico de plug-in, serviços, componentes e linha de produtos | Sofia Patrocínio |

A reutilização de componentes de software existentes ou convenientemente disponíveis para reduzir tempo e custos de computação e recursos humanos é chamada de capacidade de reutilização de software. 

A reutilização de software não envolve somente fatores técnicos, como a utilização de métodos, ferramentas ou métricas.  Mas também no nível de requisitos, projeto e outros.

Os componentes reutilizáveis ​​podem ser desenvolvidos por meio do código-fonte existente. Uma vez desenvolvidos, eles podem ser usados ​​posteriormente em diferentes classes. Esses componentes reduzem significativamente o custo e o tempo de desenvolvimento de software.

O movimento *open source* cria uma enorme base de código disponível.

| Pontos Positivos | Pontos Negativos |
|-----------|--------------|
| Redução de custo e tempo |  Alto custo de manutenção, pois componentes reusados podem se tornar incompatíveis em versões futuras  |
| Confiabilidade | Falta de apoio de ferramenta (Ambientes de desenvolvimento podem não estar preparados para a reutilização) |
| Melhor qualidade de serviço | Dificuldade de reutilização software terceiro (Deve-se encontrar e entender o software que pretende reutilizar) |
| Compartilhamento de conhecimento | |
| Adequação aos padrões dentro da aplicação | |

## Formas comuns de reutilização

### Framework
- Os *frameworks* dão suporte ao reúso de projeto, bem como ao reúso de classes específicas de sistema, pois fornecem uma arquitetura de esqueleto para a aplicação. A arquitetura é definida por classes de objetos e suas interações. As classes são reusadas diretamente e podem ser prorrogadas usando-se recursos, como a herança.

- Possuem aspectos variáveis (*hot-spots*) e inváriáveis (*frozen-spots*)

| Hot-Spots | Frozen-Spots |
|-----------|--------------|
| Partes espeíficas de sistemas individuas |  Arquitetura geral de um sistema  |
| Projetados para serem genéricos | Permanecem fixos em todas as instanciações do *framework* de aplicação |
| Normalmente representados com classes abstratas | Também conhecido como "core" do *framework* |

- Classificação de *Frameworks* quanto à Adaptação

| Framework Caixa Branca | Framework Caixa Preta | Framework Caixa Cinza |
|-----------|--------------|--------------|
| Orientado a *hot spots* |  Orientado a *frozen spots*  | Híbrido Caixa Branca e Caixa Preta |
| Baseiam-se no conceito de herança e ligação dinâmica | Composição de objetos sem detalhes internos | Permite adaptação tanto por herança, quanto por composição de componentes |

### Plugins

O padrão, consiste em dois tipos de componentes de arquitetura: um único sistema-núcleo e os módulos plug-ins. A lógica das aplicações, está dividida entre os módulos de plug-ins independentes e o sistema-núcleo básico, de forma a proporcionar extensibilidade, flexibilidade e isolamento das características-chave do núcleo, e da lógica adicional do processamento plugado

### Serviços

A essência de um serviço é que o fornecimento de serviço é independente da aplicação que o usa (TURNER et al., 2003). Os provedores de serviços podem desenvolver serviços especializados e oferecê-los para uma variedade de usuários de serviço de diferentes organizações.

### Componentes

Os componentes são abstrações de nível mais alto do que objetos e são definidos por suas interfaces. Geralmente, eles são maiores que objetos individuais e todos os detalhes de implementação são escondidos de outros componentes.

- Componentes são independentes, então eles não interferem na operação uns dos outros. Detalhes de implementação são ocultados. Implementação dos componentes pode ser alterada sem afetar o restante do sistema.

- Os componentes comunicam-se por meio de interfaces bem definidas. Se essas interfaces forem mantidas, um componente poderá ser substituído por outro, que forneça funcionalidade adicional ou aumentada.

- As infraestruturas dos componentes oferecem uma gama de serviços-padrão que podem ser usados em sistemas de aplicações, o que reduz a quantidade de códigos novos a serem desenvolvidos.

### Linhas de Produto

Um tipo de aplicação é generalizado em torno de uma arquitetura comum para que esta possa ser adaptada para diferentes clientes. Uma linha de produtos de software é um conjunto de aplicações com uma arquitetura comum e componentes compartilhados, sendo cada aplicação especializada para refletir necessidades diferentes. 

## Referências

- Neelamdhab Padhy, R.P. Singh, Suresh Chandra Satapathy, Software reusability metrics estimation: Algorithms, models and optimization techniques, Computers & Electrical Engineering, Volume 69, 2018,Pages 653-668, ISSN 0045-7906, [https://doi.org/10.1016/j.compeleceng.2017.11.022](http://www.sciencedirect.com/science/article/pii/S0045790617323327)

- Ian Sommerville. Engenharia de Software, 9ª Edição. Pearson Education, 2011 - Cap. 16 Reuso de Software (até Seção 16.1)

