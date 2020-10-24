# Aplicação do Chain of Responsibility
**Para saber mais sobre o padrão acesse: [*Chain of Responsibility*](Project/Estudos/comportamental?id=Cadeia-de-Responsabilidades.md)**

Este padrão está sendo utilizado para fazer a autenticação do [usuário](Modeling/objeto?id=usuário), assim como uma solução para a Hierarquia de [Usuários](Modeling/objeto?id=usuário).


## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 17/10/2020 | 1.0 | Criação do documento e adição da Hierarquia de [Usuários](Modeling/objeto?id=usuário) | Micaella Gouveia |
| 16/10/2020 | 1.1 | Implementação da Autenticação de [Usuários](Modeling/objeto?id=usuário)| Gabriel Davi |
| 17/10/2020 | 1.2 | Adição da Autenticação e léxicos | Micaella Gouveia |
| 20/10/2020 | 1.3 | Adição dos links para github e atualização das imagens de autenticação | Micaella Gouveia |
| 24/10/2020 | 1.4 |Implementação da Hierarquia de [Usuários](Modeling/objeto?id=usuário) | Sofia Patrocínio |
| 24/10/2020 | 1.5 |Adição dos imagens da hierarquia | Micaella Gouveia e Sofia Patrocínio | 


## Autenticação de Usuários
Para assegurar que o [usuário](Modeling/objeto?id=usuário) que tenta entrar na aplicação seja um [usuário](Modeling/objeto?id=usuário) credenciado, fazemos uma autenticação deste [usuário](Modeling/objeto?id=usuário). Utilizamos os middlewares como forma de verificação, eles são acionados antes da solicitação ganhar acesso à rota, e se o [usuário](Modeling/objeto?id=usuário) não possuir esta credencial, ele não ganha o acesso.

*Middleware de autenticação **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/middlewares/Authorization.js))***
<p align="center">
<img src="/assets/padroes/chainResponsibility/auth.png" class="codes-prints" />
</p>

*Rota usando o middleware de Autenticação **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/Collaborator.routes.js))***
<p align="center">
<img src="/assets/padroes/chainResponsibility/routes.png" class="codes-prints" />
</p>

## Hierarquia de Usuários
Para solucionar o problema da Hierarquia de [Usuários](Modeling/objeto?id=usuário), este padrão propõe simplificar esta hierarquia, transformando as diversas classes de [usuários](Modeling/objeto?id=usuário) em uma só, que se diferenciam por um atributo de nível de acesso. Essa atributo será primordial para que o usuário tenha acesso às funcionalidades do sistema. 

Utilizamos os middlewares para fazer essa verificação. Assim como é feita a autenticação do usuário logado no sistema, agora este usuário, para acessar uma funcionalidade, sua solicitação passará por uma cadeia de verificação, confirmando ou não seu acesso.


*Middleware de Verificação de Nível de Acesso **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/middlewares/AccessLevel.js))***
<p align="center">
<img src="/assets/padroes/chainResponsibility/acessLevelMiddleware.png" class="codes-prints" />
</p>

*Rota usando middleware de Nível de Acesso **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/Category.routes.js))***
<p align="center">
<img src="/assets/padroes/chainResponsibility/categoryRouteMiddleware.png" class="codes-prints" />
</p>
