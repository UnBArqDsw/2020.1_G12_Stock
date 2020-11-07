# Reutilização de Software

Neste módulo, será melhor explicado o que é a Reutilização de Software.

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 05/11/2020 | 1.0 | Criação do documento e adição de explicação geral | Sofia Patrocínio |
| 06/11/2020 | 1.1 | Adição de tópico de frameworks | Sofia Patrocínio |

A reutilização de componentes de software existentes ou convenientemente disponíveis para reduzir tempo e custos de computação e recursos humanos é chamada de capacidade de reutilização de software. 

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

Possuem aspectos variáveis (*hot-spots*) e inváriáveis (*frozen-spots*)

| Hot-Spots | Frozen-Spots |
|-----------|--------------|
| Partes espeíficas de sistemas individuas |  Arquitetura geral de um sistema  |
| Projetados para serem genéricos | Permanecem fixos em todas as instanciações do *framework* de aplicação |
| Normalmente representados com classes abstratas | Também conhecido como "core" do *framework* |

Classificação de *Frameworks* quanto à Adaptação

- Framework Caixa Branca
    - Orientado a *hot spots*
    - Baseiam-se no conceito de herança e ligação dinâmica
- Framework Caixa Preta
    - Orientado a *frozen spots*
    - Composição de objetos sem detalhes internos
- Framework Caixa Cinza
    - Híbrido Caixa Branca e Caixa Preta
    - Permite adaptação tanto por herança, quanto por composição de componentes

### Plugins
### Serviços
### Componentes
### Linhas de Produto

## Referências
-Neelamdhab Padhy, R.P. Singh, Suresh Chandra Satapathy, Software reusability metrics estimation: Algorithms, models and optimization techniques, Computers & Electrical Engineering, Volume 69, 2018,Pages 653-668, ISSN 0045-7906, [https://doi.org/10.1016/j.compeleceng.2017.11.022](http://www.sciencedirect.com/science/article/pii/S0045790617323327)

- Ian Sommerville. Engenharia de Software, 9ª Edição. Pearson Education, 2011 - Cap. 16 Reuso de Software (até Seção 16.1)

