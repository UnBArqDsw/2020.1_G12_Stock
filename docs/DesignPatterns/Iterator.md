# Aplicação do Iterator
**Para saber mais sobre o padrão acesse: [*Iterator*](Project/Estudos/comportamental?id=Iterator.md)**

Para nossa aplicação estamos utilizando uma abstração do padrão Iterator. 

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 19/10/2020 | 1.0 | Criação do documento e adição do tópico Iterator | Micaella Gouveia |
| 22/10/2020 | 1.1 | Implementação do padrão Iterator | Pedro Igor |
| 23/10/2020 | 1.2 | Adição dos exemplos de uso do Iterator | Micaella Gouveia |

Sua implementação não está seguindo totalmente o padrão estabelecido, porém a linguagem JavaScript utiliza abstrações do padrão por meio de loops, que são utilizados por meio dos comandos *for*, *do while* e *while*.

*Loop para relacionar produto com suas várias categorias **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/BelongsBase.js))***
<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/padroes/iterator/belongsCreateIterator.png" class="codes-prints" />
</p>

*Loop para retornar todos os lots de um produto específico **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/LotBase.js))***
<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/padroes/iterator/lotBasefindAllIterator.png" class="codes-prints" />
</p>

*Loop para retornar a quantidade total de produtos em todos os seus lots **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/ProductBase.js))***
<p align="center">
<img src="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/padroes/iterator/productBaseUpdateIterator.png" class="codes-prints" />
</p>
