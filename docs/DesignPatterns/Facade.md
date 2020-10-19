# Aplicação do Facade
**Para saber mais sobre o padrão acesse: [*Facade*](Project/Estudos/estrutural?id=Facade.md)**

Para a nossa aplicação estamos utilizando o facade para a criação das rotas.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 19/10/2020 | 1.0 | Criação do documento e adição do tópico Routes | Micaella Gouveia |
| 19/10/2020 | 1.1 | Linkagem para github | Micaella Gouveia |

## Routes

Facade pode ser reconhecida em uma classe que possui uma interface simples, mas delega a maior parte do trabalho para outras classes. No nosso caso, criamos fachadas para nossas rotas, em que cada classe possui suas rotas específicas. Um index de rotas chamará todas essas fachadas.

*Index de rotas recebe fachada CollaboratorRoutes (**[Link para Github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/index.routes.js)**)*

<p align="center">
<img src="/assets/padroes/facade/routeFacade.png" class="codes-prints" />
</p>


*Fachada de Rotas do Collaborator (**[Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/Collaborator.routes.js)**)*

<p align="center">
<img src="/assets/padroes/grasp/collaboratorRoutes.png" class="codes-prints" />
</p>
