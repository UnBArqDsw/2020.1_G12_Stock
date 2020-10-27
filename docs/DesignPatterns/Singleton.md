# Aplicação do Singleton
**Para saber mais sobre o padrão acesse: [*Singleton*](Project/Estudos/criacional?id=Singleton.md)**

Estamos utilizando o padrão criacional Singleton para a instância única da aplicação com o banco de dados [Sequelize](Modeling/objeto?id=Sequelize).

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 18/10/2020 | 1.0 | Implementação do padrão Singleton | Gabriel Davi e Pedro Igor |
| 19/10/2020 | 1.1 | Criação do documento e adição do tópico Singleton | Micaella Gouveia |
| 19/10/2020 | 1.2 | Linkagem para github | Micaella Gouveia |

## Banco de Dados

Singleton é um padrão de design criativo que permite garantir que uma classe tenha apenas uma instância, ao mesmo tempo que fornece um ponto de acesso global para essa instância. Utilizamos esse padrão para garantir a instância única do banco de dados com a aplicação.

*Instância única do banco de dados (**[Link para Github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/database/index.js)**)*

<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/padroes/singleton/singleton.png" class="codes-prints" />
</p>