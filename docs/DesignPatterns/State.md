# Aplicação do State
**Para saber mais sobre o padrão acesse: [*State*](Project/Estudos/comportamental?id=State.md)**

Para a mudança de estados de variáveis utilizamos o padrão comportamental State no Frontend da aplicação.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 25/10/2020 | 1.0 | Implementação do padrão State | Gabriel Davi |
| 26/10/2020 | 1.1 | Criação do documento e adição do tópico State | Micaella Gouveia |
| 26/10/2020 | 1.1 | Adição dos prints e links para github | Micaella Gouveia |
| 26/10/2020 | 1.2 |             Revisão texto             | Sofia Patrocínio |

## useState
O framework React possui o useState, que é um hook específico do React que altera o estado interno de uma variável sem precisar implementar lógicas complexas. 

Um dos exemplos na aplicação é auxiliado com o uso do useContext, que possibilita a criação de variáveis globais que podem ser alteradas dentro de todo o escopo que for determinado, tirando a necessidade de passar as informações por meio das props. O useContext é responsável em criar essas variáveis globais e utiliza o useState para que essas variáveis possam ser alteradas.

*Provider dos contexts em que possui a declaração das variáveis globais (**[Link para Github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Frontend/tree/devel/src/Contexts/AuthContext.js)**)*

<p align="center">
<img src="/assets/padroes/state/authContextState.png" class="codes-prints" />
</p>

*Rota Index determinando espaço de atuação dos contexts(**[Link para Github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Frontend/tree/devel/src/Routes/index.js)**)*

<p align="center">
<img src="/assets/padroes/state/indexProviderState.png" class="codes-prints" />
</p>

*Utilização do useState dos contexts para alterar document e password(**[Link para Github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Frontend/tree/devel/src/Pages/AuthPages/Login/index.js)**)*

<p align="center">
<img src="/assets/padroes/state/setState.png" class="codes-prints" />
</p>