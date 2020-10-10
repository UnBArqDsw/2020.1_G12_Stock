# Documento de Decisão Arquitetural

Aqui será descrito as tecnologias utilizadas no desenvolvimento do projeto, juntamente com as suas respectivas arquiteturas.

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 09/10/2020 | 1.0 | Criação do documento | Gabriel Alves |

## Contexto
O Stock será uma aplicação web de controle de estoque, voltada para o pequeno comerciante, para auxiliá-lo no controle e gestão dos seus produtos.<br> Desenvolvida por cinco graduandos do curso de Engenharia de Software, pela disciplina de Arquitetura e Desenho de Software com tempo estimado de cinco meses de desenvolvimento, tempo de duração da matéria.

## Decisão
O principal critério para decisão arquitetural e escolha das tecnologias foi o tempo disponível de desenvolvimento da aplicação web, cinco meses. Além do tempo, outro critério importante é que a tecnologia tivesse como aplicar padrões de Orientação a Objetos, para melhor aproveitamento das técnicas ministradas durante a disciplina.

Com isso, foi escolhido o padrão arquitetural Model–view–controller (MVC), na qual a model representa a manipulação dos dados, view representa a camada de interação com o usuário e a controller representando a camada de controle onde organiza a intermediação das requisições vindas da view e as mandando para a model.

As tecnologias escolhidas foram NodeJS e React, pois atendiam as necessidades mencionadas anteriormente além de possuir uma curva de aprendizagem mais curta, essencial para o tempo disponível de desenvolvimento.

## Tecnologias

### Back End
**NodeJS** "Ambiente de execução Javascript server-side" (LENON, 2018)
Um grande motivo de sucesso do Node é o seu grande potencial de escalabilidade. Além do fato de usar uma das linguagens mais utilizadas no mundo, o JavaScript.

### Front End
**React** É um framework open source de desenvolvimento web. Mais simples de desenvolver, comparado com outros frameworks, Angular por exemplo. Além do uso de JavaScript, abordagem baseada em componentes e um ciclo de vida bem definidos são pontos fortes desse framework. Grandes empresas como Facebook e Uber demonstram a confiabilidade do React.

## Referências
- O QUE É REACT.JS E PORQUE DEVEMOS USÁ-LO?: <https://edit.com.pt/blog/o-que-e-reactjs-e-porque-devemos-usa-lo/#:~:text=Abordagem%20nativa-,O%20React.,aplica%C3%A7%C3%B5es%20IOS%2C%20Android%20e%20Web.> Último acesso em: 09/10/2020.

- Node.js – O que é, como funciona e quais as vantagens: <https://www.opus-software.com.br/node-js/> Último acesso em: 09/10/2020.

- O que é MVC?: <https://tableless.com.br/mvc-afinal-e-o-que/#:~:text=MVC%20%C3%A9%20nada%20mais%20que,camada%20de%20controle(controller).> Último acesso em: 09/10/2020.

- Descrição Arquitetural: <https://unbarqdsw.github.io/2020.1_G11_SYA/#/modelagem/descricao_arquitetural> Último acesso em: 09/10/2020.

- Escreva documentos de decisão de arquitetura em projetos de software: <https://gustavohenrique.net/2018/02/escreva-documentos-de-decisao-de-arquitetura-em-projetos-de-software/> Último acesso em: 09/10/2020.