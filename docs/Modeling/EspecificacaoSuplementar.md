# Especificação Suplementar

Esta especificação tem por finalidade apresentar os [requisitos não funcionais](/Modeling/objeto?id=requisito-não-funcional) do sistema de [controle de estoque](/Modeling/verbo?id=controle-de-estoque), Stock. Será apresentada uma ambientação do projeto e, em seguida, a exposição de [requisitos suplementares](/Modeling/objeto?id=requisito-não-funcional) distribuídos em usabilidade, confiabilidade, desempenho, compatibilidade, suportabilidade, interfaces, requisitos de licenciamento e observações de copyright e outras.

## Histórico de Revisões
|     Data   | Versão |                  Descrição                | Autor(es)  |
|:----------:|:------:|:-----------------------------------------:|:----------:|
| 21/09/2020 |   1.0  | Criação do documento e adição da técnica. | Pedro Igor |
| 21/09/2020 |   1.1  | Linkagem dos léxicos.                     | Pedro Igor |

## Funcionalidade
A aplicação [web](/Modeling/objeto?id=web-app), Stock deverá ser capaz de gerenciar o [estoque](/Modeling/objeto?id=estoque) de [micro e pequenas empresas](/Modeling/objeto?id=micro-empresa). Um [sócio ou dono](/Modeling/objeto?id=owner) de um negócio terá [privilégios](Modeling/objeto?id=papéis-dos-colaboradores) para criação e adição de funcionários dentro da aplicação que terão os papéis de [cadastrar](/Modeling/verbo?id=cadastrar-produto) [produtos](/Modeling/objeto?id=produto), alimentar [estoque](/Modeling/objeto?id=estoque) e dar [baixa](/Modeling/verbo?id=baixa-em-produto) no [estoque](/Modeling/objeto?id=estoque) ao realizar uma venda. A aplicação permitirá realizar essas ações de forma remota e com atualização instantânea. Além disso, será possível fazer buscas por [produtos](/Modeling/objeto?id=produto), analisar o [histórico](/Modeling/objeto?id=log) de [fluxo](/Modeling/verbo?id=fluxo) de [estoque](/Modeling/objeto?id=estoque), [consultar gráficos](/Modeling/verbo?id=consultar-gráfico) a respeito desse [fluxo](/Modeling/verbo?id=fluxo) e [exportar](/Modeling/verbo?id=exportação) e [importar](/Modeling/verbo?id=importação) documentos de [planilhas](/Modeling/objeto?id=planilha).

## Usabilidade
A aplicação deve ser simples para qualquer [perfil](/Modeling/objeto?id=público-alvo) de [usuário](/Modeling/objeto?id=usuário) que a utilizará.

### Facilidade de uso
Os [usuários](/Modeling/objeto?id=usuário) deverão ter facilidade em utilizar a aplicação não sendo necessário treinamento algum. O programa deve ser didático o suficiente, de forma que direcione o [usuário](/Modeling/objeto?id=usuário) por meio de passos simples, a execução mais correta de uma tarefa.

## Confiabilidade
A aplicação deve saber resolver ou dar feedback útil de falhas durante a execução.

### Tratamento de falhas e excessões
O sistema deve estar preparado para tratar falhas. Algumas excessões podem ser lançadas na execução do programa ou durante a utilização de determinada funcionalidade, excessões que não foram previstas no período de [implementação](/Modeling/estado?id=em-desenvolvimento) e testes. O sistema deve informar ao [usuário](/Modeling/objeto?id=usuário) que a ação não foi realizada com sucesso e que é necessário tentar novamente. O sistema deve ser capaz de reverter ações que foram iniciadas mas não foram finalizadas.

## Desempenho
O tempo de resposta de cada ação deve ser curto.

### Tempo de resposta
O tempo de resposta deverá ser o mínimo possível. As consultas por [produtos](/Modeling/objeto?id=produto) devem retornar informações sobre aquele [produto](/Modeling/objeto?id=produto) de forma quase que instantânea. As ações realizadas no [estoque](/Modeling/objeto?id=estoque) devem ser atualizadas instantaneamente na base de dados para que não haja inconsistências entre o que está [armazenado](/Modeling/verbo?id=armazenar) na base e o que realmente está disponível fisicamente.

## Compatibilidade

A aplicação deve ser compatível com qualquer [navegador](/Modeling/objeto?id=navegador) [web](/Modeling/objeto?id=web-app) assim como [PWA](/Modeling/objeto?id=pwa), para utilização de qualquer, ou a maioria, dos dispositivos móveis.

## Suportabilidade
A manutenção da aplicação deve ser possível em um tempo curto.

### Facilidade de Manutenção
A linguagem de programação utilizada deve ser de simples entendimento.

### Linguagem de Programação Única
Como a aplicação é multiplataforma, [web](/Modeling/objeto?id=web-app) e mobile, é importante a utilização de linguagem que não necessite a escrita do mesmo código duas vezes. Uma vez implementada a funcionalidade, esta esteja disponível para todas as plataformas que irão utilizá-las.

## Interfaces
As interfaces deverão ser intuitivas.

### Interfaces com o Usuário
As interfaces de navegação entre funcionalidades deverão ser de simples utilização.

### Interfaces de software
As informações a respeito de funcionalidades deverão ser apresentadas de forma organizada.

## Requisitos de Licenciamento

A utilização do software está restrita ao gerenciamento de [estoque](/Modeling/objeto?id=estoque) desenvolvido, não sendo garantida operacionalidade para qualquer outro fim.

## Observações legais, de Copyright e Outras

Os [usuários](/Modeling/objeto?id=usuário) da aplicação Stock estarão sujeitos a lei de direitos autorais. Assim, parte do código fonte do software pode ser utilizado desde que aplicação e documentação oficiais sejam devidamente referenciadas.


## Referências
- Especificação Suplementar – Sistema de Treinamento de Pilotos- STP - UNIFEI. Disponível em: <https://ice.unifei.edu.br/ramos/SiteTpit/DocsSTP/EspecSupl-STP.doc>. Último acesso em 21/09/2020
- Requisitos de Software Tinder. Especificação Suplementar. Disponível em: <https://requisitos-tinder.github.io/Tinder-2018-1/modelagem/EspSuplementar/EspSuplementar/>. Último acesso em 21/09/2020