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
| 17/11/2020 | 1.5 | Adição do Tópico 5 - Visão lógica - Diagrama de Pacotes | Sofia Patrocínio |

## 1 - Introdução

### 1.1 - Finalidade
  Este documento tem a finalidade de detalhar as decisões arquiteturais e estruturais do projeto Stock. As decisões foram tomadas em grupo e documentadas por meio de diagramas, tabelas assim como descrições. 

### 1.2 - Escopo
  Serão documentados os componentes de software, padrões, plataformas de desenvolvimento e frameworks necessários para a composição do programa Stock que propõe uma ferramenta para gerenciamento de estoque e funcionários de pequenas empresas. O software consiste um site que cumpre os requisitos de uma aplicação PWA podendo ser utilizado em qualquer dispositivo que tenha disponibilidade de um navegador web. O site realiza operações sobre o estoque de uma empresa de forma remota sendo necessária apenas uma conexão com a internet.

## 2 - Representação Arquitetural

### 2.1 - Tecnologias <Davi>

- Frontend:

- Backend:

- Banco de dados:

- Ambiente:

## 3 - Metas e restrição de arquitetura <Davi>

### 3.1 - Restrições tecnológicas

### 3.2 - Requisitos não funcionais

## 4 - Visão de Casos de Uso

A Visão de Casos de Uso descreve um modelo com alta significância de alto nível em relação às funcionalidades do sistema. Normalmente feito através do Diagrama de Casos de Uso.

O Diagrama de Casos de Uso corresponde a uma visão externa do sistema e representa graficamente os atores, os casos de uso, e os relacionamentos entre estes elementos. Ao longo do projeto, vários casos de uso foram elencados, podendo ser vistos em [**Casos de Uso**](Modeling/CasosUso/CasosUso).

Abaixo se encontra a o diagrama geral, relacionando todos os casos de uso elencados.


![caso geral](../../../assets/diagramas/casosUso/DiagramaCasoGeral.png)

<a href="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/pdf/diagramas/casosUso/DiagramaCasoGeral.pdf">Arquivo em PDF</a>

## 5 - Visão lógica 
  A visão lógica descreve as partes significativas do ponto de vista da arquitetura do modelo de design, como sua divisão em camadas, pacotes, classes e interfaces. 

### 5.1 - Diagrama de Contexto

### 5.2 - Diagrama de Pacotes
  O Diagrama de Pacotes tem demonstra a estrutura de diretórios e arquivos do projeto. A última versão é representada abaixo, as demais versões podem ser vistas em [Diagrama de Pacote](Modeling/Diagrams/Pacotes.md).

  ![Diagrama de Pacotes](../../assets/diagramas/pacotes/DiagramaPacotesV2.png)

## 6 - Visão de processos
  A visão de processos descreve a decomposição do sistema em grupos de processos que se comunicam e interagem. Esses processos de comunicação, bem como os objetos e mensagens trocadas entre eles podem ser vistos nos diagramas de [Comunicação](Modeling/Diagrams/Comunicacao.md) e de [Sequência](Modeling/Diagrams/Sequencia.md).

## 7 - Visão de implantação
  A visão de implantação pode ser visualizada no [Diagrama de Classes](Modeling/Diagrams/Classes.md) do projeto.

## 8 - Visão de implementação
  A visão de implementação pode ser visualizada no [Diagrama de Implementação](Modeling/Diagrams/Implementacao.md) do projeto.

## Referências

- Donar Arquitetura de Software: <http://repositorio.aee.edu.br/bitstream/aee/1106/3/TCC2_2018_2_GabrielLeiteDias_MatheusLimadeAlbuquerque_Apendice2.pdf>. Último acesso em 16/11/2020.
- Documentação da aplicação Pax: <https://pax-app.github.io/Wiki/#/docs/DS/dinamica-e-seminario-4-b/DAS>. Último acesso em 17/11/2020