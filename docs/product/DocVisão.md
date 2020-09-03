# Stock


## Histórico de Revisão

| Data | Versão | Descrição | Autor |
| ---- | ------ | --------- | ----- |
|02/09/2020| 1.0 | Criação do documento. | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor e Sofia Patrocínio | 


## 1. Introdução
### 1.1 Objetivo
Esse documento visa especificar de maneira geral as características do desenvolvimento da aplicação Stock, deixando claro seu objetivo, razão de sua necessidade, características, utilidade e requisitos do sistema.

### 1.2 Escopo
A aplicação Stock possuirá cinco funcionalidades chave: 
- Crud de estoque: Nesta funcionalidade, o usuário poderá criar, atualizar, listar por categorias e remover. A aplicação ficará responsável por apresentar de forma clara a lista dos produtos separados por tags. 
- Geração, Importação e Exportação de planilhas de consulta de estoque: Essa funcionalidade constituirá na geração de planilhas com dados do estoque, bem como importar e exportar arquivos de planilha.
- Geração de gráficos: Baseado em dados do estoque, será possível plotar gráficos que irão simplificar visualização dos dados de estoque e vendas. Além de poder filtrar por período, funcionários e categorias. 
- Notificação de prazo de validade dos produtos: Para produtos perecíveis, será possível receber alertas para avisar quando o vencimento do produto está próximo.
- Personalização de acesso baseado em papéis: A aplicação permite limitar funcionalidades e acesso à informações baseado nos papéis dos colaboradores. 

Em relação ao planejamento de produto, mas não como escopo do projeto temos funcionalidades que também farão parte, como:
- Log de vendas: Exibição em tempo real das vendas que estão sendo efetuadas.
- Cadastro de contato do fornecedor: Botão de ação para contato rápido com fornecedores, de acordo com a necessidade de realimentação do estoque.


### 1.3 Definições, Acrônimos e Abreviações
| Abreviação | Definição |
|--|--|
| MIT | Licença de software livre criada pelo Massachusetts Institute of Technology |

### 1.4 Referências

 - IBM Knowledge Center - Documento de Visão: A estrutura de tópicos do documento de visão. Disponível em: [https://www.ibm.com/support/knowledgecenter/pt-br/SSWMEQ_4.0.6/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html](https://www.ibm.com/support/knowledgecenter/pt-br/SSWMEQ_4.0.6/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html). Acesso em: 3 set. 2020;
 - PEREIRA, Samuel; PATROCÍNIO, Sofia; TAIRA, Luis Henrique; GOUVEIA, Micaella; LIMA, Eduardo; DUARTE, Indiara; Projeto Gaia: Documento de Visão. Disponível em [https://fga-eps-mds.github.io/2019.1-Gaia/#/produto/DocVisao](https://fga-eps-mds.github.io/2019.1-Gaia/#/produto/DocVisao). Acesso em: 3 set. 2020;
 - Open Source Initiative: The MIT License. Disponivel em: [https://opensource.org/licenses/MIT](https://opensource.org/licenses/MIT). Acesso em: 3 set. 2020;
 - ADIDA, Ben. Understanding Open-Source Licensing. Disponível em: [https://openacs.org/about/licensing/open-source-licensing](https://openacs.org/about/licensing/open-source-licensing). Acesso em: 3 set. 2020.
 
### 1.5 Visão Geral
Este documento descreve de forma detalhada o embasamento, o planejamento e a construção da aplicação Stock. Para isso, serão apresentados tópicos referentes a descrição do problema a ser solucionado, posicionamento do produto em relação ao mercado, as partes interessadas e usuários, perspectiva geral do produto: recursos e restrições, e requisitos para a aplicação do produto.

## 2. Planejamento
### 2.1 Oportunidade de Negócios
Atualmente, pequenos comércios tem uma gestão pouco ou com nenhuma informatização e possuem dificuldade para administrar e manter seu estoque atualizado de forma manual, levando a trabalhos onerosos e de baixa produtividade. É comum o uso de softwares de gestão em empresas de maior porte, como supermercados, farmácias, entre outros. Porém o custo torna inviável para pequenos negócios.
Com isso, o Stock busca a viabilização de uso tecnológico para esses negócios. Proporcionar auxílio no controle, gerenciamento e manutenção de seus estoque, além de obter ganhos maiores.

### 2.2 Declaração do Problema
| O problema da | afeta | cujo impacto é | uma boa solução seria | 
| ------------- | ----- | -------------- | --------------------- | 
| Dificuldade de pequenos empreendedores em controlar seus próprios estoques e também de mensurar analiticamente o crescimento/recessão de seu negócio de forma manual. | Pequenos empreendedores. | Prejuízos consideráveis ao desenvolvimento do empreendimento além de prejuízos monetários  | Uma aplicação que forneça o controle de estoque de forma eficiente e consistente, acessível, prática e confiável.


### 2.3 Declaração da Posição do Produto
| Para | Que | O Stock | Que | Diferente de | Nosso produto | 
| ---- | --- | ------ | --- | ------------ | ------------- |
| Administradores de estoque de pequenas empresas  | Que possuem dificuldade em realizar controle de estoque. | É uma aplicação | Faz controle e gerenciamento de estoque e venda | Planilhas complexas que não apresentam funções necessárias e aplicações com preços exorbitantes | Possui preço e interface acessíveis


## 3. Descrições da Parte Interessada e do Usuário
### 3.1 Resumo da parte interessada
| Nome | Descrição | Responsabilidade |
| ---- | --------- | ---------------- |
|    Equipe de desenvolvimento e engenharia do produto   | Graduandos em Engenharia de Software, cursando a disciplina Arquitetura e Desenho de Software, pela Universidade de Brasília.          |  Desenvolver o software no período estipulado, bem como testá-lo e implementá-lo e garantir a aplicação do ágil e viabilidade do projeto       |
| Milene Serrano | Professora da Universidade de Brasília, do curso de Engenharia de Software. | Orientar, acompanhar e avaliar o projeto |

### 3.2 Resumo do Usuário
| Nome | Descrição | Responsabilidades |
|----- | --------- | ----------------- |
| Pequenos Comerciantes | Que possuem dificuldade em realizar controle de estoque. | Utilizar a aplicação Stock através do acesso pelo navegador ou pwa. |


### 3.3 Ambiente do Usuário


### 3.4 Perfis das partes interessadas
#### 3.4.1 Equipe de Desenvolvimento
| Representantes | Descrição | Tipo | Responsabilidade | Critério de sucesso | Envolvimento |
| -------------- | --------- | ---- | ---------------- | ------------------- | ------------ |
| Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor e Sofia Patrocínio | Desenvolvedores e Gerentes do Projeto | Alunos da Universidade de Brasília | Desenvolver o software no período estipulado, bem como testá-lo e implementá-lo e garantir a aplicação do ágil e viabilidade do projeto | Desenvolver o produto, garantindo qualidade de entrega e todos requisitos atentidos no período estipulado | Alto


#### 3.4.2 Professora
| Representantes | Descrição | Tipo | Responsabilidade | Critério de sucesso | Envolvimento |
| -------------- | --------- | ---- | ---------------- | ------------------- | ------------ |
| |  |  |  | |  |


### 3.5 Perfis de Usuário
| Representantes | Descrição | Tipo | Responsabilidade | Critério de sucesso | Envolvimento |
| -------------- | --------- | ---- | ---------------- | ------------------- | ------------ |
|  |  |  |   |  |


### 3.6 Necessidades Principais do Investidor ou Usuário
| Necessidade | Prioridade | Interesse | Solução Atual | Solução Proposta |
| ----------- | ---------- | --------- | ------------- | ---------------- |
| Controlar fluxo de estoque | Alta | Não ter dados inconsistentes  | Planilhas ou Sistemas Caros | Controlar fluxo em tempo real
| Consultar facilmente produtos no estoque | Alta | Facilitar consulta | Conferência de Estoque | Tela de produtos em estoque em poucos cliques
| Mitigar prejuízos por vencimento de produtos | Alta | Avisos com antecedência | Conferência de Estoque Periodicamente | Avisos programados sempre que produto estiver prestes a vencer
| Gerenciar vendas | Alta | Dados mais intuitivos | Planilhas | Gráficos ilustrativos e exportação de planilhas

## 4. Visão Geral do Produto
### 4.1 Perspectiva do Produto
O software será um aplicação web e mobile, com informações sobre estoque e vendas em tempo real.

### 4.2. Resumo de Recursos
| Benefício para o cliente | Recursos de suporte |
|------------------------- | ------------------- |
| Visualizar vendas feitas por cada vendedor | A aplicação fornecerá dados por período e vendedor |
| Saber quando um produto está próximo de vencer | A aplicação notificará o usuário sempre que um produto estiver prestes a vencer |
| Não ter problemas com falta de estoque | A aplicação informará o usuário a quantidade de produtos no estoque
| Fácil visualização do estoque | A aplicação mostrará o estoque de forma simples e intuitiva |

### 4.3 Licenciamento


## 5. Recursos do Produto
### 5.1 Plataforma de comunicação em linguagem natural.
### 5.2 Permitir o usuário escolher/cadastrar um local e data para obter informações sobre o tempo.
### 5.3 Enviar notificações com informações do tempo para o usuário nos dias cadastrados.
### 5.4 Fornecer informações sobre o tempo e localização, tais como:


### 5.5 Sugerir ao usuário esportes viáveis para se praticar no local desejado levando em consideração sua situação climática.

## 6. Restrições do Produto
### 6.1 Restrições de implementação


### 6.2 Restrições externas


### 6.3 Restrições de Design


### 6.4  Restrições de Uso


### 6.5  Restrições de Confiabilidade


## 7. Faixas de Qualidade


