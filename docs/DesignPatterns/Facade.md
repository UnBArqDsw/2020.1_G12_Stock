# Aplicação do Facade
**Para saber mais sobre o padrão acesse: [*Facade*](Project/Estudos/estrutural?id=Facade.md)**

Para a nossa aplicação estamos utilizando o padrão estrutural Facade para a criação das rotas.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 19/10/2020 | 1.0 | Criação do documento e adição do tópico Routes | Micaella Gouveia |
| 19/10/2020 | 1.1 | Implementação do padrão Facade | Gabriel Davi e Pedro Igor |
| 23/10/2020 | 1.2 | Adição de mais exemplos de Facades | Micaella Gouveia |

## Routes

Facade pode ser reconhecida em uma classe que possui uma interface simples, mas delega a maior parte do trabalho para outras classes. No nosso caso, criamos fachadas para nossas rotas, em que cada classe possui suas rotas específicas. Um index de rotas chamará todas essas fachadas.

*Index de rotas recebe fachadas (**[Link para Github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/index.routes.js)**)*

<p align="center">
<img src="/assets/padroes/facade/routeFacade.png" class="codes-prints" />
</p>


*Rotas do Collaborator (**[Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/Collaborator.routes.js)**)*

<p align="center">
<img src="/assets/padroes/facade/collaboratorRouteFacade.png" class="codes-prints" />
</p>

*Rotas do Belongs (**[Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/Belongs.routes.js)**)*

<p align="center">
<img src="/assets/padroes/facade/belongsRouteFacade.png" class="codes-prints" />
</p>


*Rotas do Category (**[Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/Category.routes.js)**)*

<p align="center">
<img src="/assets/padroes/facade/categoryRouteFacade.png" class="codes-prints" />
</p>


*Rotas do Lot (**[Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/Lot.routes.js)**)*

<p align="center">
<img src="/assets/padroes/facade/lotRouteFacade.png" class="codes-prints" />
</p>


*Rotas do Produto (**[Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/Product.routes.js)**)*

<p align="center">
<img src="/assets/padroes/facade/productRouteFacade.png" class="codes-prints" />
</p>

