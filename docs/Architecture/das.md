# Documento de Arquitetura de Software

É um documento que descreve as principais características arquiteturais do projeto Stock. Esse documento cobre diferentes visões de implementação que tornou possível o desenvolvimento da aplicação.

## Histórico de Revisão

| Data       | Versão | Descrição                                             | Autor                                                        |
| ---------- | ------ | ----------------------------------------------------- | ------------------------------------------------------------ |
| 16/11/2020 | 1.0    | Abertura do documento                                 | Micaella Gouveia, Gabriel Davi, Pedro Igor, Sofia Patrocínio |
| 17/11/2020 | 1.1    | Adição do Tópico 4 - Visão de Casos de Uso            | Micaella Gouveia                                             |
| 17/11/2020 | 1.2    | Adição do Tópico 1 - Introdução (Finalidade e escopo) | Pedro Igor                                                   |
| 17/11/2020 | 1.3    | Adição do Tópico 7 - Diagrama de Implantação          | Pedro Igor                                                   |
| 17/11/2020 | 1.4    | Adição do Tópico 8 - Diagrama de Implementação        | Pedro Igor                                                   |
| 18/11/2020 | 1.5    | Adição do Tópico 2.1 - Tecnologias                    | Gabriel Davi                                                 |

## 1 - Introdução

### 1.1 - Finalidade

Este documento tem a finalidade de detalhar as decisões arquiteturais e estruturais do projeto Stock. As decisões foram tomadas em grupo e documentadas por meio de diagramas, tabelas assim como descrições.

### 1.2 - Escopo

Serão documentados os componentes de software, padrões, plataformas de desenvolvimento e frameworks necessários para a composição do programa Stock que propõe uma ferramenta para gerenciamento de estoque e funcionários de pequenas empresas. O software consiste um site que cumpre os requisitos de uma aplicação PWA podendo ser utilizado em qualquer dispositivo que tenha disponibilidade de um navegador web. O site realiza operações sobre o estoque de uma empresa de forma remota sendo necessária apenas uma conexão com a internet.

## 2 - Representação Arquitetural

### 2.1 - Tecnologias

- Frontend:

  - ReactJs:
    O React é um conjunto de bibliotecas que fornece diversas facilidades para o desenvolvimento web. Ele tem como base a linguagem de programação Javascript e já é extremamente popular na comunidade e no mercado.
    A escolha dessa tecnologia se deu pela sua popularidade dentro da comunidade. Há diversos conteúdo e conteúdos em cima do tema, por isso é uma escolha segura de que qualquer dificuldade durante o desenvolvimento seria facilmente resolvida.

- Backend:

  - NodeJs:
    O Node também é bastante conhecido dentro da comunidade. Junto com Express, é possível construir serviços bastantes escaláveis e de fácil manutenção. O Node tem sua arquitetura embasada na programação assíncrona baseada em sua thread de execução e fila de espera, o que permite a manipulação do fluxo de execução de código com os comandos corretos.
    A escolha dessa tecnologia também foi com base em sua populariade no marcad e também por conta de ser construída em cima da linguagem de programação Javascript, o que confere uma sinergia positiva quando desenvolvemos com React, que tbm é feito com Javascript.
  - Express:
    O express é um framework para construção de serviços em node. Ele fornece com facilidade todas as ferramentas para construção de uma api rest dentro do ambiente NodeJs.
  - Sequelize: Sequelize é uma ORM. Sendo assim, fazendos todas as consultas e interação com banco de dados através da interface em javascript utilizando essa ferramenta. Ele tem suporte para diferentes bancos de dados incluindo Mysql, sqlite, postgres entre outros.

- Banco de dados:

  - Postgres:
    É um banco relacional extremamente popular baseado em sql. Tem uma ótima integração com o Sequelize e uma comunidade bastante ative, sendo um dos bancos de dados mais populares da atualidade.
  - Redis:
    O Redis é um banco de dados não relacional. Sua principal característica e sua leveza, o que o torna extremamente performático, ideal para manipular sessões de usuários e conexões de rede via websocket.

- Ambiente:
  - Docker: O Docker é uma ferramenta de isolamento de ambientes. É uma ótima ferramenta para uso em equipe para isolar ambientes e manter um desenvolvimento livre de inconstâncias de configuração.

## 3 - Metas e restrição de arquitetura <Davi>

### 3.1 - Restrições tecnológicas

### 3.2 - Requisitos não funcionais

## 4 - Visão de Casos de Uso

A Visão de Casos de Uso descreve um modelo com alta significância de alto nível em relação às funcionalidades do sistema. Normalmente feito através do Diagrama de Casos de Uso.

O Diagrama de Casos de Uso corresponde a uma visão externa do sistema e representa graficamente os atores, os casos de uso, e os relacionamentos entre estes elementos. Ao longo do projeto, vários casos de uso foram elencados, podendo ser vistos em [**Casos de Uso**](Modeling/CasosUso/CasosUso).

Abaixo se encontra a o diagrama geral, relacionando todos os casos de uso elecados.

![caso geral](../../../assets/diagramas/casosUso/DiagramaCasoGeral.png)

<a href="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/pdf/diagramas/casosUso/DiagramaCasoGeral.pdf">Arquivo em PDF</a>

## 5 - Visão lógica <Sofia>

## 6 - Visão de processos <Sofia>

## 7 - Visão de implantação

A visão de implantação pode ser visualizada no [diagrama de classes](Modeling/Diagrams/Classes.md) do projeto.

## 8 - Visão de implementação

A visão de implementação pode ser visualizada no [diagrama de implementação](Modeling/Diagrams/Implementacao.md) do projeto.

## Referências

- Donar Arquitetura de Software: <http://repositorio.aee.edu.br/bitstream/aee/1106/3/TCC2_2018_2_GabrielLeiteDias_MatheusLimadeAlbuquerque_Apendice2.pdf>. Último acesso em 16/11/2020.
- Documentação da aplicação Pax: <https://pax-app.github.io/Wiki/#/docs/DS/dinamica-e-seminario-4-b/DAS>. Último acesso em 17/11/2020
