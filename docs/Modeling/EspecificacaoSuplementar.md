# Especificação Suplementar

Esta especificação tem por finaliadade apresentar os requisitos não funcionais do sistema de controle de estoque Stock. Será apresentada uma ambientação do projeto e em segui exposição de requisitos suplementares distribuídos em .

## Histórico de Revisões
|     Data   | Versão |                  Descrição                | Autor(es)  |
|:----------:|:------:|:-----------------------------------------:|:----------:|
| 21/09/2020 |   1.0  | Criação do documento e adição da técnica. | Pedro Igor |

## Funcionalidade
A aplicação web, Stock deverá ser capaz de gerenciar o estoque de micro e pequenas empresas. Um sócio ou dono de um negócio terá privilégios para criação e adição de funcionários dentro da aplacação que terão os papéis de cadastrar produtos, alimentar estoque e dar baixa no estoque ao realizar uma venda. A aplicação permitirá realizar essas ações de forma remota e com atualização instantânea. Além disso, será possível fazer buscas por produtos, analisar o histórico de fluxo de estoque, consultar gráficos a respeito desse fluxo e exportar e importar documentos de planilhas.

## Usabilidade
A aplicação deve ser simples para qualquer perfil de usuário que a utilizará.

### Facilidade de uso
Os usuários deverão ter facilidade em utilizar a aplicação não sendo necessário treinamento algum. O programa deve ser didático o suficiente, de forma que direcione o usuário por meio de passos simples, a execução mais correta de uma tarefa.

## Confiabilidade
A aplicação deve saber resolver ou dar feedback útil de falhas durante a execução.

### Tratamento de falhas e excessões
O sistema deve estar preparado para tratar falhas. Algumas excessões podem ser lançadas na execução do programa ou durante a utilização de determinada funcionalidade, excessões que não foram previstas no período de implementação e testes. O sistema deve informar ao usuário que a ação não foi realizada com sucesso e que é necessário tentar novamente. O sistema deve ser capaz de reverter ações que foram iniciadas mas não foram finalizadas.

## Desempenho
O tempo de resposta de cada ação deve ser curto.

### Tempo de resposta
O tempo de respostas deverá ser o mínimo possível. As consultas por produtos devem retornar informações sobre aquele produto de forma quase que instantânea. As ações realizadas no estoque devem ser atualizadas instantâneamente no base de dados para que não haja inconsistências entre o que está armazenado na base e o que realmente está disponível fisicamente.

## Compatibilidade

A aplicação deve ser compatível com qualquer navegador web assim como pwa, para utilização mobile de qualquer, ou a maioria, dos dispositivos móveis.

## Suportabilidade
A manutenção da aplicação deve ser possível em um tempo curto.

### Facilidade de Manutenção
A linguagem de programação utilizada deve ser de simples entendimento.

### Linguagem de Programação Única
Como a aplicação é multiplataforma (web e mobile), é importante a utilização de linguagem que não necessite a escrita do mesmo código duas vezes. Uma vez implementada a funcinalidade esteja disponível para todas as plataformas que irão utilizá-las.

## Interfaces
As interfaces deverão ser intuitivas.

### Interfaces com o usuário
As interfaces de navegação entre funcionalidades deverão ser de simples utilização.

### Interfaces de software
As informações a respeito de funcionalidades deverão ser apresentadas de forma organizada.

## Requisitos de Licenciamento

A utilização do software está restrita ao gerenciamento de estoque desenvolvido, não sendo garantida operacionalidade para qualquer outro fim.

## Observações legais, de Copyright e Outras

Os usuários da aplicação Stock estarão sujeitos a lei de direitos autorais. Assim, parte do software pode ser utilizado desde que aplicação e documentação oficiais sejam devidamente referenciadas.


## Referências
Especificação Suplementar – Sistema de Treinamento de Pilotos- STP - UNIFEI <https://ice.unifei.edu.br/ramos/SiteTpit/DocsSTP/EspecSupl-STP.doc>. Último acesso em 21/09/2020