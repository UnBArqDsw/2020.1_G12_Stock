# Documento de Arquitetura de Software

É um documento que descreve as principais características arquiteturais do projeto Stock. Esse documento cobre diferentes visões de implementação que tornou possível o desenvolvimento da aplicação.

## Histórico de Revisão

| Data | Versão | Descrição | Autor |
|------|--------|-----------|-------|
| 16/11/2020 | 1.0 | Abertura do documento | Micaella Gouveia, Gabriel Davi, Pedro Igor, Sofia Patrocínio |
| 17/11/2020 | 1.1 | Adição do Tópico 4 - Visão de Casos de Uso | Micaella Gouveia |
| 17/11/2020 | 1.2 | Adição do Tópico 1 - Introdução (Finalidade e escopo) | Pedro Igor |
| 17/11/2020 | 1.3 | Adição do Tópico 7 - Diagrama de Implantação | Pedro Igor |
| 17/11/2020 | 1.4 | Adição do Tópico 8 - Diagrama de Implementação | Pedro Igor |
| 17/11/2020 | 1.5 | Adição do Tópico 6 - Visão de processos | Sofia Patrocínio |
| 17/11/2020 | 1.6 | Adição do Tópico 5 - Visão lógica - Diagrama de Pacotes | Sofia Patrocínio |
| 18/11/2020 | 1.7 | Adição do Tópico 2.1 - Tecnologias | Gabriel Davi |
| 19/11/2020 | 1.8 | Adição dos tópicos de restrições tecnológicas | Gabriel Davi |
| 19/11/2020 | 1.9 | Adição dos diagramas de implantação de implementação mais atuais | Micaella Gouveia |
| 19/11/2020 | 2.0 | Adição do diagrama de contexto | Sofia Patrocínio |
| 20/11/2020 | 2.1 | Revisão e correção de erros ortográficos | Micaella Gouveia |

## 1 - Introdução

### 1.1 - Finalidade

Este documento tem a finalidade de detalhar as decisões arquiteturais e estruturais do projeto Stock. As decisões foram tomadas em grupo e documentadas por meio de diagramas, tabelas assim como descrições.

### 1.2 - Escopo

Serão documentados os componentes de software, padrões, plataformas de desenvolvimento e frameworks necessários para a composição do programa Stock que propõe uma ferramenta para gerenciamento de estoque e funcionários de pequenas empresas. O software consiste um site que cumpre os requisitos de uma aplicação PWA podendo ser utilizado em qualquer dispositivo que tenha disponibilidade de um navegador web. O site realiza operações sobre o estoque de uma empresa de forma remota sendo necessária apenas uma conexão com a internet.

## 2 - Representação Arquitetural

### 2.1 - Tecnologias

- **Frontend**:

  - ReactJs:
    O React é um conjunto de bibliotecas que fornece diversas facilidades para o desenvolvimento web. Ele tem como base a linguagem de programação Javascript e já é extremamente popular na comunidade e no mercado.
    A escolha dessa tecnologia se deu pela sua popularidade dentro da comunidade. Há diversos conteúdo e conteúdos em cima do tema, por isso é uma escolha segura de que qualquer dificuldade durante o desenvolvimento seria facilmente resolvida.

- **Backend**:

  - NodeJs:
    O Node também é bastante conhecido dentro da comunidade. Junto com Express, é possível construir serviços bastantes escaláveis e de fácil manutenção. O Node tem sua arquitetura embasada na programação assíncrona baseada em sua thread de execução e fila de espera, o que permite a manipulação do fluxo de execução de código com os comandos corretos.
    A escolha dessa tecnologia também foi com base em sua populariade no mercado e também por conta de ser construída em cima da linguagem de programação Javascript, o que confere uma sinergia positiva quando desenvolvemos com React, que também é feito com Javascript.
  - Express:
    O express é um framework para construção de serviços em NodeJS. Ele fornece com facilidade todas as ferramentas para construção de uma API REST dentro do ambiente NodeJs.
  - Sequelize: 
    Sequelize é uma ORM. Sendo assim, é possível fazer todas as consultas e interação com banco de dados através da interface em Javascript utilizando essa ferramenta. Ele tem suporte para diferentes bancos de dados incluindo Mysql, SQLite, Postgres entre outros.

- **Banco de dados**:

  - Postgres:
    É um banco relacional extremamente popular baseado em SQL. Tem uma ótima integração com o Sequelize e uma comunidade bastante ativa, sendo um dos bancos de dados mais populares da atualidade.
  - Redis:
    O Redis é um banco de dados não relacional. Sua principal característica é sua leveza, o que o torna extremamente performático, ideal para manipular sessões de usuários e conexões de rede via websocket.

- **Ambiente**:

  - Docker: O Docker é uma ferramenta de isolamento de ambientes. É uma ótima ferramenta para uso em equipe para isolar ambientes e manter um desenvolvimento livre de inconstâncias de configuração.

## 3 - Metas e restrição de arquitetura

### 3.1 - Metas

- Responsividade: Aplicação deve ser responsiva e ser usável em todas as interfaces sem que haja comprometimento nas funções da aplicação.
- Segurança: A aplicação deve ser segura para seus usuários. Isso quer dizer que qualquer infomação sensível do usuário deve estar em segurança em nossos servidores e nossos servidores devem ser protegidos contra ataques externos.
- Escalabilidade: A aplição deve ser capaz de crescer junto com a ascensão de novos usuários e também ser escalável para implementação de novas funcionalidades.

### 3.2 - Restrições

- Conectividade: É necessário estar conectado com a internet para ter acesso a aplicação.
- Idioma: A aplicação tem idioma somente para o português.
- Sociedade com uma empresa: Usuários devem ter alguma associação com empresa para utilizar o aplicativo.

## 4 - Visão de Casos de Uso

A Visão de Casos de Uso descreve um modelo com alta significância de alto nível em relação às funcionalidades do sistema. Normalmente feito através do Diagrama de Casos de Uso.

O Diagrama de Casos de Uso corresponde a uma visão externa do sistema e representa graficamente os atores, os casos de uso, e os relacionamentos entre estes elementos. Ao longo do projeto, vários casos de uso foram elencados, podendo ser vistos em [**Casos de Uso**](Modeling/CasosUso/CasosUso).

Abaixo se encontra o diagrama de casos de uso geral, relacionando todos os casos de uso elencados.

![caso geral](../../../assets/diagramas/casosUso/DiagramaCasoGeral.png)

<a href="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/pdf/diagramas/casosUso/DiagramaCasoGeral.pdf">Arquivo em PDF</a>

## 5 - Visão lógica 
  A visão lógica descreve as partes significativas do ponto de vista da arquitetura do modelo de design, como sua divisão em camadas, pacotes, classes e interfaces. 

### 5.1 - Diagrama de Contexto
  O Diagrama de Contexto descreve os processos em nível mais alto, mostrando o contexto geral do projeto.

<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/diagramas/contexto/DiagramaContexto.png"/>
</p>

<a href="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/diagramas/contexto/DiagramaContexto.pdf">Arquivo em PDF</a>

### 5.2 - Diagrama de Pacotes
  O Diagrama de Pacotes demonstra a estrutura de diretórios e arquivos do projeto. A última versão é representada abaixo, as demais versões podem ser vistas em [**Diagrama de Pacote**](Modeling/Diagrams/Pacotes.md).

  ![Diagrama de Pacotes](../../assets/diagramas/pacotes/DiagramaPacotesV2.png)

## 6 - Visão de processos
  A visão de processos descreve a decomposição do sistema em grupos de processos que se comunicam e interagem. Esses processos de comunicação, bem como os objetos e mensagens trocadas entre eles podem ser vistos em [**Diagrama de Comunicação**](Modeling/Diagrams/Comunicacao.md) e [**Diagrama de Sequência**](Modeling/Diagrams/Sequencia.md).

## 7 - Visão de implantação

A visão de implantação pode ser visualizada em [**Diagrama de Classes**](Modeling/Diagrams/Classes.md). A versão mais recente está abaixo:

![diagramaClasse](../../assets/diagramas/classe/DiagramaClassesV4.png)
<a href="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/pdf/diagramas/classe/DiagramaClassesV4.pdf">Arquivo em PDF</a>

## 8 - Visão de implementação

A visão de implementação pode ser visualizada em [**Diagrama de Implementação**](Modeling/Diagrams/Implementacao.md). A versão mais recente está abaixo:

![Diagrama de Implementação](../../assets/diagramas/Diagrama_de_Implementacao.png)
<a href="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/pdf/diagramas/implantacao/Diagrama_de_Implementacao.pdf">Arquivo em PDF</a>

## Referências

- Donar Arquitetura de Software: <http://repositorio.aee.edu.br/bitstream/aee/1106/3/TCC2_2018_2_GabrielLeiteDias_MatheusLimadeAlbuquerque_Apendice2.pdf>. Último acesso em 16/11/2020.
- Documentação da aplicação Pax: <https://pax-app.github.io/Wiki/#/docs/DS/dinamica-e-seminario-4-b/DAS>. Último acesso em 17/11/2020
