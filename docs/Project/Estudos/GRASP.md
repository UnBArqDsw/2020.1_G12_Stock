# Estudo Dirigido - GRASP
GRASP significa Padrões de Software para Atribuição de Responsabilidade Geral e consiste em diretrizes para atribuir responsabilidade a classes e objetos em projeto orientado a objetos.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 30/09/2020 | 1.0 | Estudos GRASP - Criador e Especialista | Sofia Patrocínio |
| 02/10/2020 | 1.1 | Criação do documento | Sofia Patrocínio |

## Criador ou Creator

Ao avaliar o modelo, primeiro questionamento é quais classes possuem as responsabilidades de criar instâncias. Seu objetivo é definir como criador o objeto que precise ser conectado ao objeto criado em algum evento.

Atribua à classe B a responsabilidade de criar uma nova instância da	classe A se uma das seguintes condições for verdadeira:

- B "contém" A ou é uma composição de A
- B registra A
- B usa A de maneira muito próxima
- B tem dados iniciais de A, os quais serão passados para A quando este for criado. B é um "especialista" em relação à criação de A

Se a relação for de agregação é melhor, pois o código está menos acoplado. Se for de composição, a parte só existe se o todo existir.

*Se a relação for de agregação é melhor, pois o código está menos acoplado. Se for de composição, a parte só existe se o todo existir.*

## Especialista

Criador é um especialista em criação de instâncias. Já o Especialista é um padrão que se preocupa em atribuir responsabilidades para a entidade mais especialista em um dado aspecto, não apenas de criação de instâncias, mas de todos os aspectos do sistema.

- Quem é a melhor entidade para calcular algo?
- Quem é a melhor entidade para ordenar algo?
- Quem é a melhor entidade para cadastrar algo?

## Baixo Acoplamento ou Acoplamento Fraco

O baixo acoplamento é um padrão de avaliação que determina como atribuir responsabilidades de suporte:

- Menor dependência entre as classes
- Mudança em uma classe com menor impacto em outras
- Maior potencial de reutilização
- Facilidade na manutenção

## Alta Coesão

Atribuir de forma coerente as responsabilidades das classes, mantendo os objetos adequadamente focados, gerenciáveis e compreensíveis.

- Mais	clareza	e	facilidade	de	compreensão	no	
projeto	
- Simplificação	de	manutenção	e	acréscimo de	funcionalidade/melhorias	
- Favorecimento	do	acoplamento	fraco	
- Aumento	no	potencial	de	reutilização

## Controlador ou Controller 

Objeto responsável por receber e lidar com um evento do sistema.

## Referências
- Apresentação: GRASP: Designing Objetos com Responsabilidades  - MC 426 IC Unicamp – M. Cecilia C. Baranauskas - <https://www.ic.unicamp.br/~ariadne/mc436/1s2017/Lar16GRASP.pdf>. Último acesso em 02/10/2020