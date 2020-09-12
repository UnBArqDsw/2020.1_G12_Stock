# Plano de Metodologia

## Históricos de Revisões
|    Data    | Versão |         Descrição         |           Autor(es)            |
| :--------: | :----: | :-----------------------: | :----------------------------: |
| 05/09/2020 |  1.0   |  Criação do documento e adição das práticas ágeis, ferramentas e plano de métricas | Micaella Gouveia e Sofia Patrocínio |
| 05/09/2020 |  1.1   |  Adição da imagem de ferramentas e ajustes no texto | Sofia |
| 07/09/2020 | 1.2 | Adição do texto explicativo das metodologias | Micaella Gouveia e Sofia Patrocínio |
| 11/09/2020 |  1.3   |  Linkagem dos léxicos. | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |


# Práticas Ágeis 

Para este projeto, decidimos utilizar diferentes metodologias de forma híbrida, usando a combinação das ferramentas que mais se aplicam ao contexto do time e do projeto. Nossa base é a metodologia Scrum, com algumas práticas do XP e do Kanban. 

* O **Scrum** adota uma abordagem iterativa e incremental voltada para o [produto](Modeling/objeto?id=Produto), ou seja, a cada iteração, é adicionado algo relevante para o [produto](Modeling/objeto?id=Produto). 
* O **XP** *(Extreme Programming)* já é mais voltado para qualidade de código, produtividade do time e lida bem com requisitos vagos que mudam frequentemente, times pequenos e mais disciplina dos [desenvolvedores](Modeling/objeto?id=Desenvolvedor) ao invés de processos formais, enfatizando o trabalho em equipe.
* O **Kanban** visa a gestão de fluxo de tarefas, com o intuito de aumentar a eficiência da produção e realizações de tarefas, otimizar sistemas de movimentaçao e produção.   


## Scrum

* **Iterações**: Nossas sprints têm duração média de uma semana. Aos sábados tudo é concluído e preparado para uma nova iteração. Isso é feito através de uma reunião remota semanal, nela são feitas várias práticas ágeis de gerenciamento de projeto. 
* **Sprint Planning**: Durante a reunião semanal, há o planejamento das tarefas que serão feitas na próxima Sprint. É realizada por todos os membros, definindo as histórias de [usuário](Modeling/objeto?id=usuário) do Product Backlog que serão implementadas, suas pontuações e responsáveis. 
* **Daily Meeting**: A Daily é feita através de um grupo no Telegram em que um bot nos notifica de segunda a sábado às 22h. Ela tem como objetivo disseminar conhecimento sobre o que foi feito no dia anterior, identificar impedimentos e priorizar o trabalho a ser realizado no dia que se inicia.
* **Sprint Review**: Durante a reunião semanal, o time debate sobre o desenvolvimento da Sprint, verificando  tudo o que foi feito e entregue.
* **Retrospectiva**: Também é realizada durante a reunião semanal e seu objetivo é fazer uma análise de como foi a Sprint, o que funcionou bem, o que pode ser melhorado e que ações serão tomadas para melhorar.
*  **Product Backlog**: Um conjunto de funcionalidades pensadas e desejadas para o [produto](Modeling/objeto?id=Produto). Com o tempo, o Product Backlog cresce e muda à medida que se aprende mais sobre o [produto](Modeling/objeto?id=Produto) e seus [usuários](Modeling/objeto?id=usuário) . 
*  **Histórias de [Usuário](Modeling/objeto?id=usuário)**: Uma forma de definir e organizar os requisitos do sistema, centrando a visão no [usuário](Modeling/objeto?id=usuário). 
* **Backlog de Melhoria**: Onde estarão todas as atividades, features e artefatos que deverão ser evoluídos e/ou modificados.
*  **Controle de Versão**: O controle de versão é feito com relação à documentação na Wiki e ao código no Github. De forma objetiva, os artefatos são evoluídos constantemente e para manter o rastro disso, é feito o controle de versão.
* **Testes de Aceitação**: Os testes de aceitação visam alinhar as expectativas quanto ao que foi definido no início da Sprint e o que está sendo entregue. 
*  **Planning Poker**: É uma técnica baseada no consenso para estimar o esforço para cada tarefa. Utilizaremos o **[Plan it Poker](https://www.planitpoker.com/)** para a pontuação das [issues](Modeling/objeto?id=Issue).

## XP

*  **Pair-Programming**: É eficaz para reduzir a incidência de [bugs](Modeling/objeto?id=Bug) em um sistema e consiste em uma forma de trocar conhecimento, alinhar o grupo, tirar dúvidas e desenvolver algo em conjunto. É o momento em que os pares se juntam para que um desenvolva (piloto) e o outro axilie (co-piloto) por um curto período até que o papel rotacione.
*  **Refatoring**: É processo de refatoração de código com o intuito de melhorar a sua estrutura, tornando-o mais claro, limpo e de fácil compreensão sem que haja grandes alterações no que o sistema faz. 
* **Collective Ownership**: Encorajamento de todos os membros a contribuírem em todos os seguimentos do projeto. Consiste em revezamento de pares, total autorizaçao para edição de código por qualquer membro. Isso torna o código coletivo e responsabilizado por todos os envolvidos. 

## KanBan
* **ZenHub**: ZenHub é um produto beta que nos permite desenvolver mais rápido, comunicar melhor e lançar sem sobrecarga, integrando tudo dentro do GitHub, o lugar em que todo o nosso código reside.

## Outros
*  **Code Reviews**: A revisão de código é feita pelos membros não participantes da [issue](Modeling/objeto?id=Issue) entregue. A segunda parte é feita na reunião da Sprint onde o time avalia e repassa os conhecimento adquiridos, as dificuldades enfrentadas e então o que deve ser melhorado vem à tona.

# Ferramentas
<img src='./assets/img/metodologia/ferramentas.png' style='margin-top:50px;'>

* **GitHub**: Utilizado para armazenamento de documentos e código, versionamento e gerência e comunicação das [issues](Modeling/objeto?id=Issue).
* **Microsoft Teams**: Utilizado para realização e gravação das reuniões e pareamentos.
* **Google Drive**: Utilizado para armazenamento de documentos diversos.
* **Telegram**: Utilizado para realização das dailies e comunicação entre os membros da equipe, monitores e professora.
* **Zenhub**: Utilizado como KanBan do projeto.
* **Google Calendar**: Utilizado para organização das entregas e reuniões.

# Plano de Métricas

<p>O Plano de Métricas tem como objetivo descrever todas as ferramentas e métodos utilizados para coletar as métricas e indicadores do projeto. As métricas e indicadores levantados serão levados para todo o time e as decisões serão tomadas em conjunto, levando para a equipe, a importância e o valor de coletar métricas.</p>
<p>É muito importante lembrar que os indicadores permitem  um aspecto muito importante do <b>Manifesto de Desenvolvimento Ágil</b>:<b> Melhoria Contínua</b>, ou seja, avaliando a produtividade do time e percebendo algum problema por meio da coleta de dados, será possível então procurar melhorar</p>

## Burndown

O Burndown é uma ferramenta que permite a visualização das tarefas completadas por dia, mostrando ao final um gráfico em que é possível ver a produtividade da equipe na Sprint. O Burndown nos permite, como time, ter uma boa noção de como está o projeto ao longo da Sprint e consequentemente tomar decisões para que a equipe alcance o seu nível ótimo de produtividade. 

## Velocity

O Velocity é um indicador utilizado para definir a quantidade média entre os pontos do Backlog do [produto](Modeling/objeto?id=Produto) e o incremento do [produto](Modeling/objeto?id=Produto) durante a sprint, ou seja, o Velocity indica uma média entre o planejado e o entregue. 


## Quadro de conhecimento

O quadro de conhecimento tem como objetivo servir de monitoramento do conhecimento da equipe e ele deve ser modificado toda Sprint para que seja possível ver o progresso do time.

## Referências
* Agile Project Management Best Practices & Guides: <https://blog.zenhub.com/how-the-zenhub-team-uses-zenhub-boards-on-github/>. Último acesso em 05/09/2020.
* Desenvolvimento Ágil Srum: <http://www.desenvolvimentoagil.com.br/scrum/>. Último acesso em 05/09/2020.
* Desenvolvimento Ágil XP: <http://www.desenvolvimentoagil.com.br/xp/>. Último acesso em 05/09/2020.
* Cultura Ágil: <https://www.culturaagil.com.br/kanban-do-inicio-ao-fim/>. Último acesso em 05/09/2020.
* Kanban: O que é, como funciona e como implantar esse método: <https://blog.egestor.com.br/kanban/>. Último acesso em 07/09/2020.

