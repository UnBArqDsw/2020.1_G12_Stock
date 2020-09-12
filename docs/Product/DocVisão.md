# Stock

**Este artefato foi produzido durante o dia 2 da Design Sprint, para saber mais sobre a metodologia e como ela foi feita, clique aqui: _[Design Sprint](DesignSprint/DesignSprint.md)_**

## Histórico de Revisão

| Data       | Versão | Descrição                                        | Autor                                                                        |
| ---------- | ------ | ------------------------------------------------ | ---------------------------------------------------------------------------- |
| 02/09/2020 | 1.0    | Criação do documento.                            | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor e Sofia Patrocínio |
| 03/09/2020 | 1.1    | Adição do documento na wiki.                     | Sofia Patrocínio                                                             |
| 09/09/2020 | 1.2    | Adição de hyperlink para página de Design Sprint | Sofia Patrocínio                                                             |

## 1. Introdução

### 1.1 Objetivo

Esse documento visa especificar de maneira geral as características do desenvolvimento da aplicação Stock, deixando claro seu objetivo, razão de sua necessidade, características, utilidade e requisitos do sistema.

### 1.2 Escopo

A aplicação Stock possuirá cinco funcionalidades chave:

- Crud de [estoque](Modeling/objeto?id=Estoque): Nesta funcionalidade, o [usuário](Modeling/objeto?id=usuário) poderá criar, atualizar, listar por categorias e remover. A aplicação ficará responsável por apresentar de forma clara a lista dos [produtos](Modeling/objeto?id=Produto) separados por [tags](Modeling/objeto?id=Tag).
- Geração, [Importação](Modeling/verbo?id=Importação) e [Exportação](Modeling/verbo?id=Exportação) de planilhas de [consulta de estoque](Modeling/verbo?id=Consultar-Produto): Essa funcionalidade constituirá na geração de planilhas com dados do [estoque](Modeling/objeto?id=Estoque), bem como [importar](Modeling/verbo?id=Importação) e [exportar](Modeling/verbo?id=Exportação) arquivos de planilha.
- Geração de gráficos: Baseado em dados do [estoque](Modeling/objeto?id=Estoque), será possível plotar gráficos que irão simplificar visualização dos dados de [estoque](Modeling/objeto?id=Estoque) e vendas. Além de poder filtrar por período, funcionários e categorias.
- Notificação de [prazo de validade](Modeling/estado?id=Prazo-de-Validade) dos [produtos](Modeling/objeto?id=Produto): Para [produtos](Modeling/objeto?id=Produto) perecíveis, será possível receber [alertas](Modeling/verbo?id=Alertar) para avisar quando o [vencimento](Modeling/estado?id=Prazo-de-Validade) do [produto](Modeling/objeto?id=Produto) está próximo.
- Personalização de acesso baseado em [papéis](Modeling/objeto?id=Papéis-dos-colaboradores) : A aplicação permite limitar funcionalidades e acesso à informações baseado nos [papéis dos colaboradores](Modeling/objeto?id=Papéis-dos-colaboradores).

Em relação ao planejamento de [produto](Modeling/objeto?id=Produto), mas não como escopo do projeto temos funcionalidades que também farão parte, como:

- [Log](Modeling/objeto?id=Log) de vendas: Exibição em tempo real das vendas que estão sendo efetuadas.
- Cadastro de contato do [fornecedor](Modeling/objeto?id=Fornecedor): Botão de ação para contato rápido com [fornecedores](Modeling/objeto?id=Fornecedor), de acordo com a necessidade de realimentação do [estoque](Modeling/objeto?id=Estoque).

### 1.3 Definições, Acrônimos e Abreviações

| Abreviação                    | Definição                                                                   |
| ----------------------------- | --------------------------------------------------------------------------- |
| MIT                           | Licença de software livre criada pelo Massachusetts Institute of Technology |
| [PWA](Modeling/objeto?id=PWA) | Progressive Web App                                                         |

### 1.4 Referências

- IBM Knowledge Center - Documento de Visão: A estrutura de tópicos do documento de visão. Disponível em: [https://www.ibm.com/support/knowledgecenter/pt-br/SSWMEQ_4.0.6/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html](https://www.ibm.com/support/knowledgecenter/pt-br/SSWMEQ_4.0.6/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html). Acesso em: 3 set. 2020;
- PEREIRA, Samuel; PATROCÍNIO, Sofia; TAIRA, Luis Henrique; GOUVEIA, Micaella; LIMA, Eduardo; DUARTE, Indiara; Projeto Gaia: Documento de Visão. Disponível em [https://fga-eps-mds.github.io/2019.1-Gaia/#/produto/DocVisao](https://fga-eps-mds.github.io/2019.1-Gaia/#/produto/DocVisao). Acesso em: 3 set. 2020;
- Open Source Initiative: The MIT License. Disponivel em: [https://opensource.org/licenses/MIT](https://opensource.org/licenses/MIT). Acesso em: 3 set. 2020;
- ADIDA, Ben. Understanding Open-Source Licensing. Disponível em: [https://openacs.org/about/licensing/open-source-licensing](https://openacs.org/about/licensing/open-source-licensing). Acesso em: 3 set. 2020.

### 1.5 Visão Geral

Este documento descreve de forma detalhada o embasamento, o planejamento e a construção da aplicação Stock. Para isso, serão apresentados tópicos referentes a descrição do problema a ser solucionado, posicionamento do [produto](Modeling/objeto?id=Produto) em relação ao mercado, as partes interessadas e usuários, perspectiva geral do [produto](Modeling/objeto?id=Produto): recursos e restrições, e requisitos para a aplicação do [produto](Modeling/objeto?id=Produto).

## 2. Planejamento

### 2.1 Oportunidade de Negócios

Atualmente, pequenos comércios tem uma gestão pouco ou com nenhuma informatização e possuem dificuldade para administrar e manter seu [estoque](Modeling/objeto?id=Estoque) atualizado de forma manual, levando a trabalhos onerosos e de baixa produtividade. É comum o uso de softwares de gestão em empresas de maior porte, como supermercados, farmácias, entre outros. Porém o custo torna inviável para pequenos negócios.
Com isso, o Stock busca a viabilização de uso tecnológico para esses negócios. Proporcionar auxílio no controle, gerenciamento e manutenção de seus [estoques](Modeling/objeto?id=Estoque), além de obter ganhos maiores.

### 2.2 Declaração do Problema

| O problema da                                                                                                                                                                                      | afeta                   | cujo impacto é                                                                            | uma boa solução seria                                                                                                                                     |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------- | ----------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Dificuldade de pequenos empreendedores em controlar seus próprios [estoques](Modeling/objeto?id=Estoque) e também de mensurar analiticamente o crescimento/recessão de seu negócio de forma manual | Pequenos empreendedores | Prejuízos consideráveis ao desenvolvimento do empreendimento além de prejuízos monetários | Uma aplicação que forneça o [controle de estoque](Modeling/verbo?id=Controle-de-Estoque) de forma eficiente e consistente, acessível, prática e confiável |

### 2.3 Declaração da Posição do [Produto](Modeling/objeto?id=Produto)

| Para                                                                                                      | Que                                                                                              | O Stock         | Que                                                                                      | Diferente de                                                                                    | Nosso [produto](Modeling/objeto?id=Produto) |
| --------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ | --------------- | ---------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------- | ------------------------------------------- |
| [Administradores](Modeling/objeto?id=Admin) de [estoque](Modeling/objeto?id=Estoque) de pequenas empresas | Que possuem dificuldade em realizar [controle de estoque](Modeling/verbo?id=Controle-de-Estoque) | É uma aplicação | Faz controle e [gerenciamento de estoque](Modeling/verbo?id=Controle-de-Estoque) e venda | Planilhas complexas que não apresentam funções necessárias e aplicações com preços exorbitantes | Possui preço e interface acessíveis         |

## 3. Descrições da Parte Interessada e do Usuário

### 3.1 Resumo da parte interessada

| Nome                                                                            | Descrição                                                                                                                    | Responsabilidade                                                                                                                        |
| ------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| Equipe de desenvolvimento e engenharia do [produto](Modeling/objeto?id=Produto) | Graduandos em Engenharia de Software, cursando a disciplina Arquitetura e Desenho de Software, pela Universidade de Brasília | Desenvolver o software no período estipulado, bem como testá-lo e implementá-lo e garantir a aplicação do ágil e viabilidade do projeto |
| Milene Serrano                                                                  | Professora da Universidade de Brasília, do curso de Engenharia de Software.                                                  | Orientar, acompanhar e avaliar o projeto                                                                                                |

### 3.2 Resumo do [Usuário](Modeling/objeto?id=usuário)

| Nome                  | Descrição                                                                                         | Responsabilidades                                                                                                            |
| --------------------- | ------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Pequenos Comerciantes | Que possuem dificuldade em realizar [controle de estoque](Modeling/verbo?id=Controle-de-Estoque). | Utilizar a aplicação Stock através do acesso pelo [navegador](Modeling/objeto?id=Navegador) ou [PWA](Modeling/objeto?id=PWA) |

### 3.3 Ambiente do [Usuário](Modeling/objeto?id=usuário)

O Stock poderá ser acessado através de um [navegador](Modeling/objeto?id=Navegador) ou [PWA](Modeling/objeto?id=PWA) e é necessário conexão com internet.

### 3.4 Perfis das partes interessadas

#### 3.4.1 Equipe de Desenvolvimento

| Representantes                                                               | Descrição                                                               | Tipo                               | Responsabilidade                                                                                                                        | Critério de sucesso                                                                                                                     | Envolvimento |
| ---------------------------------------------------------------------------- | ----------------------------------------------------------------------- | ---------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | ------------ |
| Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor e Sofia Patrocínio | [Desenvolvedor](Modeling/objeto?id=Desenvolvedor) e Gerentes do Projeto | Alunos da Universidade de Brasília | Desenvolver o software no período estipulado, bem como testá-lo e implementá-lo e garantir a aplicação do ágil e viabilidade do projeto | Desenvolver o [produto](Modeling/objeto?id=Produto), garantindo qualidade de entrega e todos requisitos atentidos no período estipulado | Alto         |

#### 3.4.2 Professora

| Representante  | Descrição                                                                  | Tipo       | Responsabilidade                                             | Critério de sucesso                                               | Envolvimento |
| -------------- | -------------------------------------------------------------------------- | ---------- | ------------------------------------------------------------ | ----------------------------------------------------------------- | ------------ |
| Milene Serrano | Professora da Universidade de Brasília, do curso de Engenharia de Software | Professora | Orientar, acompanhar e avaliar o processo de desenvolvimento | Avaliar o [produto](Modeling/objeto?id=Produto) em sua completude | Médio        |

### 3.5 Perfis de [Usuário](Modeling/objeto?id=usuário)

| Representantes        | Descrição                                                                                | Tipo                                  | Responsabilidade                             | Critério de sucesso                           | Envolvimento |
| --------------------- | ---------------------------------------------------------------------------------------- | ------------------------------------- | -------------------------------------------- | --------------------------------------------- | ------------ |
| Pequenos Comerciantes | Pessoa interessada realizar [controle de estoque](Modeling/verbo?id=Controle-de-Estoque) | [Usuário](Modeling/objeto?id=usuário) | Utilizar o Stock nas plataformas disponíveis | Controlar de forma prática o estoque e vendas | Alto         |

### 3.6 Necessidades Principais do Investidor ou [Usuário](Modeling/objeto?id=usuário)

| Necessidade                                                                | Prioridade | Interesse                    | Solução Atual                         | Solução Proposta                                                                             |
| -------------------------------------------------------------------------- | ---------- | ---------------------------- | ------------------------------------- | -------------------------------------------------------------------------------------------- |
| Controlar fluxo de estoque                                                 | Alta       | Não ter dados inconsistentes | Planilhas ou Sistemas Caros           | Controlar fluxo em tempo real                                                                |
| Consultar facilmente [produtos](Modeling/objeto?id=Produto) no estoque     | Alta       | Facilitar consulta           | Conferência de Estoque                | Tela de [produtos](Modeling/objeto?id=Produto) em estoque em poucos cliques                  |
| Mitigar prejuízos por vencimento de [produtos](Modeling/objeto?id=Produto) | Alta       | Avisos com antecedência      | Conferência de Estoque Periodicamente | Avisos programados sempre que [produto](Modeling/objeto?id=Produto) estiver prestes a vencer |
| Gerenciar vendas                                                           | Alta       | Dados mais intuitivos        | Planilhas                             | Gráficos ilustrativos e [Exportação](Modeling/verbo?id=Exportação) de planilhas              |

## 4. Visão Geral do Produto

### 4.1 Perspectiva do [Produto](Modeling/objeto?id=Produto)

O software será um [Aplicação Web](Modeling/objeto?id=Web-App) e [PWA](Modeling/objeto?id=PWA), com informações sobre [estoque](Modeling/objeto?id=Estoque) e vendas em tempo real.

### 4.2. Resumo de Recursos

| Benefício para o [cliente](Modeling/objeto?id=usuário)                       | Recursos de suporte                                                                                                                                           |
| ---------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Visualizar vendas feitas por cada [vendedor](Modeling/objeto?id=Seller)      | A aplicação fornecerá dados por período e [vendedor](Modeling/objeto?id=Seller)                                                                               |
| Saber quando um [produto](Modeling/objeto?id=Produto) está próximo de vencer | A aplicação notificará o [usuário](Modeling/objeto?id=usuário) sempre que um [produto](Modeling/objeto?id=Produto) estiver prestes a vencer                   |
| Não ter problemas com falta de estoque                                       | A aplicação informará o [usuário](Modeling/objeto?id=usuário) a quantidade de [produtos](Modeling/objeto?id=Produto) no [estoque](Modeling/objeto?id=Estoque) |
| Fácil visualização do [estoque](Modeling/objeto?id=Estoque)                  | A aplicação mostrará o [estoque](Modeling/objeto?id=Estoque) de forma simples e intuitiva                                                                     |

### 4.3 Licenciamento

O Stock será distribuído sob a licença MIT para softwares livres, que dá liberdade para todos que o adquirirem de modificar, distribuir, sublicenciar, vender e contribuir para o software.

## 5. Recursos do Produto

### 5.1 Criar, atualizar, listar por categorias e remover estoque.

### 5.2 Geração, [Importação](Modeling/verbo?id=Importação) e [Exportação](Modeling/verbo?id=Exportação) de planilhas de [consulta de estoque](Modeling/verbo?id=Consultar-Produto).

### 5.3 Geração de gráficos de [estoque](Modeling/objeto?id=Estoque) e vendas.

### 5.4 Notificação de [prazo de validade](<(Modeling/estado?id=Prazo-de-Validade)>) dos [produto](Modeling/objeto?id=Produto)

### 5.5 Personalização de acesso baseado em papéis do negócio

## 6. Restrições do Produto

### 6.1 Restrições de implementação

As tecnologias utilizadas serão definidas de acordo com a arquitetura.

### 6.2 Restrições externas

A falta de contato com as tecnologia, imprevistos com infraestrutura no home office e o agravamento da pandemia podem se tornar grandes riscos para o desenvolvimento do [produto](Modeling/objeto?id=Produto).

### 6.3 Restrições de Design

O sistema deve ser feito em uma interface de fácil usabilidade, tornando-o intuitivo e fácil de usar para o [usuário](Modeling/objeto?id=usuário).

### 6.4 Restrições de Uso

Para utilizar o Stock, o [usuário](Modeling/objeto?id=usuário) deverá ter uma conexão com a internet.

### 6.5 Restrições de Confiabilidade

O sistema terá cobertura de testes de usabilidade e testes unitários.

## 7. Faixas de Qualidade

A interação do [usuário](Modeling/objeto?id=usuário) com o software deve ocorrer de forma fácil, com pouca ou nenhuma necessidade de tutorial. Deve ser fácil entender como usar todos os recursos do Stock apenas interagindo com ele. O software oferecerá consistência e confiabilidade.
