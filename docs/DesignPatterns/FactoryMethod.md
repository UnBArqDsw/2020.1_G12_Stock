# Aplicação do Factory Method
**Para saber mais sobre o padrão acesse: [*Factory Method*](Project/Estudos/criacional?id=Factory-Method.md)**

Para nossa aplicação, decidimos utilizar o padrão criacional Factory Method para duas ocasiões: Hierarquia dos [Usuários](Modeling/objeto?id=usuário) e [Produtos](Modeling/objeto?id=Produto) Perecíveis/Não Perecíveis.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 14/10/2020 | 1.0 | Implementação do Factory Method | Micaella Gouveia e Sofia Patrocínio |
| 17/10/2020 | 1.1 | Criação do documento e adição da Hierarquia de [Usuários](Modeling/objeto?id=usuário) | Micaella Gouveia |
| 17/10/2020 | 1.2 | Adição dos [produtos](Modeling/objeto?id=Produto) perecíveis/não perecíveis e adição dos léxicos| Micaella Gouveia |
| 26/10/2020 | 1.3 |        Revisão texto             | Sofia Patrocínio |

## Hierarquia de Usuários
Nossa ideia inicial era fazer uma fábrica de colaboradores, podendo ele ser [Seller](Modeling/objeto?id=Seller), [Admin](Modeling/objeto?id=Admin) ou [Owner](Modeling/objeto?id=Owner). Criamos então uma classe abstrata Collaborator que possuiria todos os atributos compartilhados entre as classes, e cada classe concreta, [Seller](Modeling/objeto?id=Seller), [Admin](Modeling/objeto?id=Admin) e [Owner](Modeling/objeto?id=Owner), possuiria seus métodos específicos. 


*Classe Abstrata Collaborator*

<p align="center">
<img src="/assets/padroes/factoryMethod/collaborator.png" class="codes-prints" />
</p>

*Trecho da classe Seller*

<p align="center">
<img src="/assets/padroes/factoryMethod/seller.png" class="codes-prints" />
</p>

*Trecho da classe Admin*

<p align="center">
<img src="/assets/padroes/factoryMethod/admin.png" class="codes-prints" />
</p>

*Trecho da classe Owner*

<p align="center">
<img src="/assets/padroes/factoryMethod/owner.png" class="codes-prints" />
</p>


*Este código está disponível no repositório do Backend da aplicação na branch [*147-user-factory-method*](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/commit/83b291205906be740c160b63d0b75e28257d0a3a)*


Nas imagens já conseguimos ver um dos problema ao utilizar esse padrão. A codificação dos atributos de cada classe se repete, triplicando código. 

Outro problema que encontramos foi que o banco [Sequelize](Modeling/objeto?id=Sequelize) não permite salvar classes abstratas, forçando salvar cada classe concreta no banco, prejudicando uma das funcionalidades da aplicação que é a troca de nível de acesso. Ao salvar cada classe no banco, para fazer essa troca, teríamos que duplicar o [usuário](Modeling/objeto?id=usuário) em outra tabela e apagar na tabela atual, fugindo do que foi planejado. 



### Solução Proposta
Ao analisar a invialibilidade do uso do Factory Method para a Hierarquia de [Usuários](Modeling/objeto?id=usuário), buscamos outros padrões que poderiam melhor se encaixar em nosso contexto. A melhor solução que encontramos foi o padrão comportamental Chain of Responsibility. 

Ele será detalhado em: [**Chain of Responsibility**](DesignPatterns/ChainResponsibility.md)

## Produtos Perecíveis/Não Perecíveis
Nossa ideia inicial era utilizar o padrão criacional Factory Method para a separação dos [produtos](Modeling/objeto?id=Produto) perecíveis e não perecíveis. Teríamos uma fábrica de produtos, podendo ser ele divido em perecível ou não perecível. A classe abstrata [produtos](Modeling/objeto?id=Produto) compartilharia seus atributos e métodos comuns e cada classe concreta possuiria seus próprios métodos.

Assim como não foi possível implementar esse padrão para a Hierarquia de [Usuários](Modeling/objeto?id=usuário), não foi possível neste caso também pela mesma razão anterior, no [Sequelize](Modeling/objeto?id=Sequelize) não é possível salvar classes abstratas, sendo inviável salvar as classes concretas no banco. 

Este caso não chegou a ser implementado pois quando o problema foi detectado no caso da Hierarquia de [Usuários](Modeling/objeto?id=usuário), já conseguimos analisar sua inviabilidade para este caso também.

### Solução Proposta
Ao entender que essa padrão não seria o adequado para o caso dos [produtos](Modeling/objeto?id=Produto) perecíveis/não perecíveis, pesquisamos outros padrões que poderiam se encaixar, porém decidimos que por enquanto, aplicar um padrão para fazer essa diferenciação não é a melhor opção. Optamos em seguir o plano original, que é criar o [produto](Modeling/objeto?id=Produto), que possui um atributo de perecidade.





