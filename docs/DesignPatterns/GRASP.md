#  Aplicação do GRASP
**Para saber mais sobre o padrão acesse: [*GRASP*](Project/Estudos/GRASP.md)**

Utilizaremos alguns dos métodos GRASPs em nosso projeto, dentre eles está o Controller, Especialista e Polimorfismo.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 19/10/2020 | 1.0 | Criação do documento e adição do tópico Controller | Micaella Gouveia |
| 19/10/2020 | 1.1 | Adição do tópico Polimorfismo e Especialista | Micaella Gouveia |
| 22/10/2020 | 1.2 | Implementação dos padrões grasps | Gabriel Davi e Pedro Igor |
| 23/10/2020 | 1.3 | Adição dos exemplos de uso | Micaella Gouveia |  

## Controllers
Para a implementação das rotas da aplicação, estamos utilizando controllers, que são responsáveis em receber e tratar os dados das requisições. Todas as nossas requisições serão tratadas por suas controllers específicas.

*Exemplo do uso da Controller (**[Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/controllers/CollaboratorController.js)**)*

<p align="center">
<img src="/assets/padroes/grasp/collaboratorController.png" class="codes-prints" />
</p>

*Routes importando Controller (**[Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/routes/Collaborator.routes.js)**)*

<p align="center">
<img src="/assets/padroes/grasp/collaboratorRoutes.png" class="codes-prints" />
</p>


## Polimorfismo
Em algumas classes, criamos classes que lidam com abstrações de métodos. Temos o exemplo da classe Base que possui os métodos relacionados ao [Sequelize](Modeling/objeto?id=Sequelize). Esse tipo de abstração torna o código menos acoplado e mais coeso. No caso do JavaScript, não é possível criar classes abstratas, então utilizamos o nome de classe, porém com conceitos e utilizações de classes abstratas.

*Exemplo de Prolimorfismo na Classe Base **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/Base.js))***

<p align="center">
<img src="/assets/padroes/decorator/decoratorBase.png" class="codes-prints" />
</p>

*Collaborator herdando da Classe Base **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/CollaboratorBase.js))***

<p align="center">
<img src="/assets/padroes/decorator/collaboratorBase.png" class="codes-prints" />
</p>

## Especialista
Podemos evidenciar o uso do Especialista nos métodos de autenticação do usuário. Funções utilizadas para autenticação do usuário foram criadas e destinadas ao Collaborator. Ele será o especialista em gerar o token e verificar credenciais.

*Collaborator especilista da autenticação **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/models/Collaborator.js))***
<p align="center">
<img src="/assets/padroes/grasp/collaboratorEspecialista.png" class="codes-prints" />
</p>

*Uso dos métodos especialistas de Collaborator **([Link para github](https://github.com/UnBArqDsw/2020.1_G12_Stock_Backend/blob/devel/src/app/StockBase/CollaboratorBase.js))***
<p align="center">
<img src="/assets/padroes/grasp/collaboratorEspecialistaBase.png" class="codes-prints" />
</p>