# Objeto

## Histórico de Revisões

|    Data    | Versão |         Descrição         |           Autor(es)            |
| :--------: | :----: | :-----------------------: | :----------------------------: |
|  08/09/2020 |  0.1   |  Sugestão de Léxicos  | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 09/09/2020 |  0.2   |  Estruturação dos léxicos  | Gabriel Alves | 
| 10/09/2020 |  0.3   |  Revisão e finalização dos léxicos | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 11/09/2020 |  1.0   |  Criação do documento | Gabriel Alves |

### PWA
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Progressive [Web App](../Modeling/objeto?id=web-app) <br> - termo usado para denotar [aplicativos da web](objetos?id=Web-App) que usam as últimas tecnologias da web.|- Realizar consultas <br> - [usuário](../Modeling/objeto?id=usuário), [[cadastrar produto](../Modeling/verbo?id=cadastrar-produto)](../Modeling/verbo?id=cadastrar-produto)|- [Web App](../Modeling/objeto?id=web-app)|

### Web App
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- designa sistemas de informática projetados para utilização através de um [navegador](../Modeling/objeto?id=navegador), através da internet ou aplicativos desenvolvidos utilizando tecnologias web|- Realizar consultas <br> - [usuário](../Modeling/objeto?id=usuário), [cadastrar produto](../Modeling/verbo?id=cadastrar-produto)|- [PWA](../Modeling/objeto?id=pwa)|

### Tag
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- termo associado com uma informação.|- [Produto](../Modeling/objeto?id=produto) identificado com uma tag <br> - [Issue](../Modeling/objeto?id=issue), marcado com uma tag|- Identificador|

### Papéis dos Colaboradores
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Papéis desempenhados pelos membros da [micro empresa](../Modeling/objeto?id=micro-empresa). <br> - Hierarquia de trabalho <br> - Grau de permissão no [Web App](../Modeling/objeto?id=web-app) |- [admin](../Modeling/objeto?id=admin), supervisiona os [Seller](../Modeling/objeto?id=seller). <br> - [Seller](../Modeling/objeto?id=seller), não consegue excluir [Produto](../Modeling/objeto?id=produto)  do sistema. |- Função <br> - Cargo|

### Micro Empresa
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- microempresa, é o pequeno negócio que tem como característica: o rendimento bruto anual de até R$360 mil|- Micro empresas realizam [controle de estoque](../Modeling/verbo?id=controle-de-estoque). <br> - Contrata [fornecedores](../Modeling/objeto?id=fornecedor) |- Pequeno negócio |

### Owner
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Proprietário ou proprietária <br> - Dono da [micro empresa](../Modeling/objeto?id=micro-empresa) |- Define papel dos colaboradores|- Dono(a) <br> - Proprietário(a) <br> Gestor(a)|

### Admin
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Administrador(a) <br> - Pessoa responsável pela administração do [Web app](../Modeling/objeto?id=web-app) e/ou da [micro empresa](../Modeling/objeto?id=micro-empresa)|- Realiza tarefas: dar [baixa em produto](../Modeling/verbo?id=baixa-em-produto) , [filtrar produtos](../Modeling/verbo?id=filtrar-produtos), [cadastrar produto](../Modeling/verbo?id=cadastrar-produto)s|- Administrador(a)|

### Seller
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- [vendedor](../Modeling/objeto?id=vendedor) ou [Vendedora](../Modeling/objeto?id=vendedor) <br> - Pessoa que faz uma venda|- Responsável por dar saída de produto <br> - Filtra Produtos <br> - [cadastrar produto](../Modeling/verbo?id=cadastrar-produto)s|- [Vendedor(a)](../Modeling/objeto?id=vendedor)|

### Bug
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Bug é um jargão da informática que se refere às temidas falhas inesperadas que ocorrem ao executar algum software ou usar um hardware <br> - Erro que ocorre no [Web app](../Modeling/objeto?id=web-app)|- Trazer informações erradas ao [dashboar](../Modeling/objeto?id=dashboard) <br> - interromper nesperadamente a aplicação|- Erro <br> - Falha de sistema|

### Issue
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Do inglês: questão|- Questão levantada pelo [stakeholder](../Modeling/objeto?id=stakeholder)|- Questão|

### Log
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Do inglês: registro|- Registro de ações do [usuário](../Modeling/objeto?id=usuário)|- histórico|

### Produto
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- aquilo que é produzido <br> - resultado da produção.|- [admin](../Modeling/objeto?id=admin) Cadastra produto, [consultar produtos](../Modeling/verbo?id=consultar-produtos)|- item|

### Estoque
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- refere-se às mercadorias, [Produto](../Modeling/objeto?id=produto)  (finais ou inacabados) ou outros elementos na posse de um agente económico|- [vendedor](../Modeling/objeto?id=vendedor), armazena [Produto](../Modeling/objeto?id=produto)  no [estoque](../Modeling/objeto?id=Estoque)|- Armazém|

### Fornecedor
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Fornecedor é toda pessoa física ou jurídica, pública ou privada, nacional ou estrangeira, bem como os entes despersonalizados, que desenvolvem atividade de produção, montagem, criação, construção, transformação, [importação](../Modeling/verbo?id=importação), [exportação](../Modeling/verbo?id=exportação), distribuição ou comercialização de [Produto](../Modeling/objeto?id=produto)  ou prestação de serviços.|- Realiza a tarefa de: fornecer [Produto](../Modeling/objeto?id=produto) |- distribuidor|

### Dashboard
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- painel visual que apresenta, de maneira centralizada, um conjunto informações: indicadores e suas métricas|- Dashboard utilizada pelo [owner](../Modeling/objeto?id=owner), [admin](../Modeling/objeto?id=admin), [Seller](../Modeling/objeto?id=seller) para facilitar sua tomada de decisão| - painel|

### Vendedor
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Pessoa responsável em vender os [Produto](../Modeling/objeto?id=produto) |- Realiza as tarefas: [cadastrar produto](../Modeling/verbo?id=cadastrar-produto) , consultar [Produto](../Modeling/objeto?id=produto) , [baixa em produto](../Modeling/verbo?id=baixa-em-produto) |-|

### Usuário
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- aquele que, por direito de uso, serve-se de algo ou desfruta de suas utilidades.|- Realiza tarefas de: filtrar [Produto](../Modeling/objeto?id=produto) , [cadastrar produto](../Modeling/verbo?id=cadastrar-produto) , dar [baixa em produto](../Modeling/verbo?id=baixa-em-produto) |- utilizador|

### Navegador
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- programa que permite a [usuário](../Modeling/objeto?id=usuário) da internet consultar páginas de hipertexto e navegar, passando de um ponto a outro da mesma página ou de página diferente, usando os links de hipertexto, além de desfrutar de outros recursos dessa rede de computadores|- [usuário](../Modeling/objeto?id=usuário) acessa o [Web App](../Modeling/objeto?id=web-app) através do navegador|- browser|

### Stakeholder
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Diz respeito às partes interessadas pela solução de software.|- Os stakeholders estão satisfeitos com o resultado do desenvolvimento <br> - Investidores são potenciais stakeholders.|- Parte interessada|

### Desenvolvedor
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|O desenvolvedor é a pessoa responsável por criar a solução de software.|- Desenvolvedor resolveu um [bug](../Modeling/objeto?id=bug) da aplicação <br>- Desenvolvedor conversa com [stakeholder](../Modeling/objeto?id=stakeholder). <br>- Desenvolvedor colocou a aplicação no ar|- Dev <br>- Programador<br>- Engenheiro de software|
