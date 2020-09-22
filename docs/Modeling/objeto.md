# Objetos

## Histórico de Revisões

|    Data    | Versão |              Descrição               |                                  Autor(es)                                  |
| :--------: | :----: | :----------------------------------: | :-------------------------------------------------------------------------: |
| 08/09/2020 |  1.0   |         Sugestão de Léxicos          | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 09/09/2020 |  1.1   |       Estruturação dos léxicos       |                                Gabriel Alves                                |
| 10/09/2020 |  1.2   |  Revisão e finalização dos léxicos   | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 11/09/2020 |  1.3   |         Criação do documento         |                                Gabriel Alves                                |
| 11/09/2020 |  1.4   |        Linkagem dos léxicos.         | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 15/09/2020 |  1.5   |       Adição de novos léxicos.       |                                Gabriel Davi                                 |
| 15/09/2020 |  1.6   | Adição e linkagem de mais um léxico. |                                 Pedro Igor                                  |
| 19/09/2020 |  1.7  | Léxicos de requisitos não funcionais e funcionais   | Gabriel Davi |


### PWA

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Progressive Web App. <br><br> Termo usado para denotar [Aplicativos da Web](Modeling/objeto?id=Web-App) que usam as últimas tecnologias da web. | Realizar [consultas](Modeling/verbo?id=Consultar-Produto) <br><br> [Usuário](Modeling/objeto?id=usuário),[Cadastrar produto](Modeling/verbo?id=Cadastrar-Produto). | [Web App](Modeling/objeto?id=Web-App). |

### Web App

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Designa sistemas de informática projetados para utilização através de um [navegador](Modeling/objeto?id=Navegador), através da internet ou aplicativos desenvolvidos utilizando tecnologias Web. | Realizar [consultas](Modeling/verbo?id=Consultar-Produto). <br><br> [Usuário](Modeling/objeto?id=usuário) [Cadastrar produto](Modeling/verbo?id=Cadastrar-Produto). | [PWA](Modeling/objeto?id=PWA). Plataforma |

### Tag

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Termo associado com uma informação. | [Produto](Modeling/objeto?id=Produto) identificado com uma Tag. <br><br> [Issue](Modeling/objeto?id=Issue) marcado com uma Tag. | Identificador<br><br>Categoria |

### Papéis dos colaboradores

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Papéis desempenhados pelos membros da micro empresa. <br><br> [Hierarquia](Modeling/objeto?id=Papéis-dos-colaboradores) de trabalho. <br><br> Grau de permissão no [Web App](Modeling/objeto?id=Web-App). | [Admin](Modeling/objeto?id=Admin) supervisiona os [Sellers](Modeling/objeto?id=Seller). <br><br> [Seller](Modeling/objeto?id=Seller) não consegue excluir [produtos](Modeling/objeto?id=Produto) do sistema. | Função. <br><br> Cargo. <br><br> Nível de acesso. <br><br> Privilégio. |

### Micro Empresa

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Microempresa é o pequeno negócio que tem como característica: o rendimento bruto anual de até R\$360 mil. | Micro empresas realizam [controle de estoque](Modeling/verbo?id=Controle-de-Estoque). <br><br> Contrata [fornecedor](Modeling/objeto?id=Fornecedor). | Pequeno negócio. |

### Owner

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Proprietário ou proprietária. <br><br> Dono(a) da [micro empresa](Modeling/objeto?id=Micro-Empresa). | Define papel dos colaboradores. | Dono(a). <br><br> Proprietário(a). <br><br> Gestor(a). <br><br> Sócio(a). |

### Admin

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Administrador(a) <br><br> Pessoa responsável pela administração do [Web App](Modeling/objeto?id=Web-App) e/ou da [Micro Empresa](Modeling/objeto?id=Micro-Empresa) | Realiza tarefas: [dar baixa](Modeling/verbo?id=Baixa-em-Produto) em [produto](Modeling/objeto?id=Produto), [filtrar produtos](Modeling/verbo?id=Filtrar-Produtos), [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto). | Administrador(a). |

### Seller

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| [Vendedor ou vendedora](Modeling/objeto?id=Seller). <br><br> Pessoa que efetua vendas. | Responsável por dar saída de [produtos](Modeling/objeto?id=Produto). <br><br> [Filtra produtos](Modeling/verbo?id=Filtrar-Produtos). <br><br> [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto). | [Vendedor(a)](Modeling/objeto?id=Seller). |

### Bug

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Bug é um jargão da informática que se refere às temidas falhas inesperadas que ocorrem ao executar algum software ou usar um hardware. <br><br> Erro que ocorre no [Web App](Modeling/objeto?id=Web-App). | Trazer informações erradas ao [Dashboard](Modeling/objeto?id=Dashboard). <br><br> Interromper inesperadamente a aplicação. | Erro. <br><br> Falha de sistema. |

### Issue

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Do inglês: questão | Questão levantada pelo [stakeholder](Modeling/objeto?id=Stakeholder). | Questão. |

### Log

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Do inglês: registro | Registro de ações do [usuário](Modeling/objeto?id=usuário) . | Histórico. |

### Produto

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Aquilo que é produzido. <br><br> Resultado da produção. | [Admin](Modeling/objeto?id=Admin) cadastra produto, [consultar produto](Modeling/verbo?id=Consultar-Produtos). | Item. |

### Estoque

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Refere-se às mercadorias, [produtos](Modeling/objeto?id=Produto) (finais ou inacabados) ou outros elementos na posse de um agente econômico. | [Vendedor](Modeling/objeto?id=Seller) armazena [produtos](Modeling/objeto?id=Produto) no estoque. | Armazém. |

### Fornecedor

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Fornecedor é toda pessoa física ou jurídica, pública ou privada, nacional ou estrangeira, bem como os entes despersonalizados, que desenvolvem atividade de produção, montagem, criação, construção, transformação, [importação](Modeling/verbo?id=Importação), [exportação](Modeling/verbo?id=Exportação), distribuição ou comercialização de [produtos](Modeling/objeto?id=Produto) ou prestação de serviços. | Realiza a tarefa de: fornecer [produtos](Modeling/objeto?id=Produto). | Distribuidor. |

### Dashboard

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Painel visual que apresenta, de maneira centralizada, um conjunto informações: indicadores e suas métricas. | [Dashboard](Modeling/objeto?id=Dashboard) utilizada pelo Owner, Admin, [Seller](Modeling/objeto?id=Seller) para facilitar sua tomada de decisão. | Painel. |

### Usuário

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Aquele que, por direito de uso, serve-se de algo ou desfruta de suas utilidades. | Realiza tarefas de: [filtrar produtos](<(Modeling/verbo?id=Filtrar-Produtos)>), [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto), [dar baixa](Modeling/verbo?id=Baixa-em-Produto) em [produto](Modeling/objeto?id=Produto). | Utilizador.<br><br>[Cliente](Modeling/objeto?id=usuário). |

### Navegador

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Programa que permite ao [usuário](Modeling/objeto?id=usuário) da internet consultar páginas de hipertexto e navegar, passando de um ponto a outro da mesma página ou de página diferente, usando os links de hipertexto, além de desfrutar de outros recursos dessa rede de computadores. | [Usuário](Modeling/objeto?id=usuário) acessa o [Web App](Modeling/objeto?id=Web-App) através do navegador | Browser |

### Stakeholder

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Diz respeito às partes interessadas pela solução de software. | Os stakeholders estão satisfeitos com o resultado do desenvolvimento <br><br> Investidores são potenciais stakeholders. | Parte interessada. |

### Desenvolvedor

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| O desenvolvedor é a pessoa responsável por criar a solução de software. | Desenvolvedor resolveu um bug da aplicação. <br><br> Desenvolvedor conversa com [stakeholder](Modeling/objeto?id=Stakeholder). <br><br> Desenvolvedor colocou a aplicação no ar. | Dev. <br><br> Programador. <br><br> Engenheiro de software. |

### Protótipo

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| É um esboço em desenho ou em programa gráfico de como ficará o produto final. | O designer criou o protótipo. <br><br> O [stakeholder](Modeling/objeto?id=Stakeholder) aprovou o protótipo. | Esboço. <br><br> Desenho do software. |

### Público Alvo

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| É segmento da sociedade com determinadas características em comum (idade, sexo, profissão, interesses etc.), ao qual se dirige uma mensagem ou um conjunto de mensagens. | O [público alvo](/Modeling/objeto?id=público-alvo) desse [Web App](Modeling/objeto?id=Web-App) é bem amplo. <br><br> O [Web App](Modeling/objeto?id=Web-App) não atingiu seu [público alvo](/Modeling/objeto?id=público-alvo) | Audiência <br><br> Público. <br><br> Perfil de usuário. |

### Planilha

| Noção | Impacto | Sinônimos |
|:-----:|:-------:|:---------:|
| Planilha é um documento, geralmente formado por células, utilizado para armazenar informações de forma que seja simples a consulta posterior. | Algumas empresas realizam controle de [estoque](Modeling/objeto?id=Estoque) em planilhas. | Documento Excel. <br><br> Spreadsheet. <br><br> Documento de tabelas. |


### Requisito funcional
|                                                                     Noção                                                                     |                                          Impacto                                          |                               Sinônimos                               |
| :-------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------: | :-------------------------------------------------------------------: |
| São especificações de uma [aplicação](Modeling/objeto?id=Web-App)  que ditam como a mesma deve se comportar no âmbito de funcionalidades. | Storyboard é uma ótima técnica para elicitar requisitos funcionais.<br><br> É necessário organizar os requistos funcionais em grau de relevância.| Features.<br><br> Funcionalidades |

### Requisito não funcional
|                                                                     Noção                                                                     |                                          Impacto                                          |                               Sinônimos                               |
| :-------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------: | :-------------------------------------------------------------------: |
| São especificações de uma [aplicação](Modeling/objeto?id=Web-App) que influenciam na experiência do [usuário](Modeling/objeto?id=usuário). | Requisitos funcionais são grandes diferencias em uma [aplicação](Modeling/objeto?id=Web-App) e podem determinar a permanência de um [usuário](Modeling/objeto?id=usuário) na mesma.| - |
