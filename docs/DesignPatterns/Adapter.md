# Aplicação do Adapter
**Para saber mais sobre o padrão acesse: [*Adapter*](Project/Estudos/estrutural?id=adapter)**

Para nossa aplicação, decidimos utilizar o padrão estrutural Adapter para a implementação de algumas consultas ao Banco de Dados.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 21/10/2020 | 1.0 | Implementação do padrão Adapter | Pedro Igor |
| 24/10/2020 | 1.1 | Documentação da implementação do Adapter | Pedro Igor |


## StockBase
Aqui o objetivo é criar uma nova camada entre a controller e as models que são gerenciadas pelo [Sequelize](Modeling/objeto?id=Sequelize). Algumas consultas são necessárias durante o desenvolvimento e estas são feitas por uma Controller. Como alternativa à própria Controller solicitar informações a Model, é utilizado um intermediário Base que é útil para a tradução das informações que alimentarão a Controller e posteriormente as Views. No exemplo a seguir, o método decrease da classe Product consulta uma lista de lotes que compõem determinado Lot. Essa consulta é feita chamando o método findAll da classe Lot esta que pode solicitar de diferentes fontes além de diferentes formatos. No entanto, é feita uma adaptação das informações para que alimente o que método decrease solicitou. No exemplo é feita uma consulta SQL que retorna em ordem ascendente de acordo com a data de validade, o que poderia ser facilmente alterado sem que seja feita alteração alguma na classe a ser alimentada.

*Classe Product Base **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/ProductBase.js))***

<p align="center">
<img src="/assets/padroes/decorator/productBase.png" class="codes-prints" />
</p>

*Classe Lot Base **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/LotBase.js))***

<p align="center">
<img src="/assets/padroes/decorator/lotBase.png" class="codes-prints" />
</p>