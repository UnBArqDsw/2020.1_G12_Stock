# CONTROLE DE RISCOS

## Histórico de Revisão
| Data | Versão | Descrição | Autor(es) |
| :--: | :----: | :-------: | :-------: |
| 03/09/2020| 1.0|Criação do documento e elicitação dos riscos, probabilidades, impactos e ações| Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio
| 03/09/2020| 1.1| Adição da estrutura analítica de riscos| Sofia Patrocínio|

## Introdução

O objetivo deste documento é explicitar como acontecerá o gerenciamento de riscos. O gerenciamento de riscos está incluso no processo de gerenciamento de projeto que inclui, além dos riscos, pessoas, custos, escopo, etc. O documento define como serão identificados, mantidos e controlados todos os riscos previstos.

## Estrutura Análitica de Riscos

![Estutura Análitica de riscos](../assets/img/riscos/fluxoAnaliseRiscos.png)

### Descrição dos Itens da Estrutura analítica de Risco

#### Organizacional
- **Recursos Humanos**: Corresponde aos riscos relacionados aos recursos humanos, bem como o comprometimento da equipe de desenvolvimento e falta de comunicação entre as partes envolvidas.
- **Priorização**: São riscos relacionados aos erros de priorização, gerando atrasos nas entregas, por existir dependências entre as tarefas.

#### Técnico
- **Requisitos**: Riscos relacionados aos requisitos levantados e ao escopo definido;
- **Tecnologia**: É relativo a riscos relacionados às tecnologias e ferramentas utilizadas no projeto.
- **Infraestrutura**: Um dos pontos mais críticos do gerenciamento de riscos em projetos de software, pois geralmente nos esquecemos de providenciar com antecedência a infraestrutura onde o software será executado. É um ponto crítico de conflitos entre a área de infraestrutura, suporte e desenvolvimento.

#### Qualidade
- **Funcionalidade**: Contempla tudo relacionado à funcionalidade do software, como garantir que os requisitos foram atendidos de forma satisfatória, garantir que atende a real necessidade do usuário e se retornará resultados precisos.
- **Usabilidade**: A usabilidade engloba todos os aspectos referentes à interface com o usuário, que se sinta a vontade com o uso do sistema e que o entenda, com o mínimo de treinamento.
- **Eficiência**: Garantir que o usuário consiga ter as respostas da aplicação de forma rápida e coesa.
- **Portabilidade**: Se refere a que plataformas/sistemas operacionais o software irá rodar e como será feita a compatibilidade.

#### Gerencia de projeto
- **Planejamento**: São riscos relacionados a erros de planejamento, como tarefas grandes em períodos curtos.
- **Estimativa**: São erros que dizem respeito a erros de estimativa, como por exemplo erros de pontuação de histórias de usuário.
- **Controle**: São riscos referentes a falta de ação sobre riscos identificados.

#### Externos
- **Mercado**: Baixa adesão dos usuários a aplicação, risco relacionado à utilização e evolução do projeto no mercado.
- **Cliente**: Diz respeito aos riscos relacionados com o cliente, como aprovação da solução. No caso do "A Monitoria" a sazonalidade do uso do produto pode representar um risco.
- **Ambiente**: O ambiente pode influenciar no desempenho da equipe e no desenvolvimento do produto, um exemplo aplicado ao nosso projeto é o fato de a maior parte do desenvolvimento acontecer na FGA e uma das limitações que pode ocorrer é a falta da internet ou a realização greves.

## Análise quantitativa dos riscos
A análise quantitativa dos riscos será feita através da matriz de probabilidade e impacto, cada risco é classificado de acordo com a sua probabilidade de ocorrência e impacto em um objetivo, se ele realmente ocorrer. A organização deve determinar que combinações de probabilidade e impacto resultam em uma classificação de alto risco, risco moderado e baixo risco.

## Probabilidade 

| Probabilidade | % de certeza | Peso |
| - | - | - |
| Nula | 0% | 0 |
| Muito baixa | 0 a 20%| 1 |
| Baixa | 20 a 40% | 2 |
| Média | 40 a 60% | 3 |
| Alta | 60 a 80% | 4 |
| Muito alta | 80 a 100% | 5 |   


### Impacto
| Impacto | Descrição | Peso |
| :-----: | :-------: | :--: |
| Muito Baixo |	Quase imperceptível para o projeto | 1 |
| Baixo	| Emite pouco impacto sobre o projeto |	2 |
| Médio | Existe um impacto considerável, mas é recuperável |	3 |
| Alto | Existe grande impacto no projeto | 4 |
| Muito Alto | Impede o prosseguimento do projeto | 5 |


## Matrizes de impacto

### Riscos organizacionais
|ID | Risco | Consequência |
| - | - | - |              |
| 1 |   |   |              |    

### Riscos técnicos
|ID | Risco | Consequência |
| - | - | - |              |
| 1 |   |   |              |   

### Riscos de Qualidade
|ID | Risco | Consequência |
| - | - | - |              |
| 1 |   |   |              |   

### Riscos de Gerência de projeto
|ID | Risco | Consequência |
| - | - | - |              |
| 1 |   |   |              |   

### Riscos Externos
|ID | Risco | Consequência |
| - | - | - |              |
| 1 |   |   |              |   



### O grau de risco é definido pela multiplicação da probabilidade pelo impacto. Conforme tabela abaixo:

![ear](https://i.imgur.com/UgqOw1k.png)


Sendo que:

1. Risco >= 15: **Elevado**
2. 5 < Risco < 15: **Médio**
3. Risco =< 5: **Baixo** 


## Análise dos Riscos

| # | Descrição | Probabilidade | Impacto | Risco |
| - | -         | -             | -       | -     |
|ID | -         | -             | -       | -     |

<br />
<br />

# Planejamento de respostas aos riscos

| ID | Descrição | Risco | Ação | Descrição da Ação | Responsável |
| - | - | - | - | - | - |
| 1 | Mudança Arquitetural | 20 | Mitigar |  Pensamento crítico a respeito da arquitetura e procurando professores e outros suportes para a sua construção   | Arquiteta |


### Análise

De acordo com o diagrama acima é possivel visualizar que o caminho crítico do projeto está relacionado com os artefatos que são os fundamentos de um desenvolvimento saudavel de um projeto. Com isso é fácil notar que o atraso dos artefatos acarretaria no atraso do projeto, devendo ter uma maior prioridade.

## Referências

