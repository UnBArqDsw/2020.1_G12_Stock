# Projeto Banco de Dados
**Este artefato foi produzido durante o dia 2 da Diagrams Sprint, para saber mais sobre a metodologia e como ela foi feita, clique aqui: _[Diagrams Sprint](Modeling/Diagrams/Diagrams.md)_**

O Projeto de banco de dados tem por finalidade modelar todo o banco de dados do sistema com suas respectivas tabelas e relacionamento. Nesse documento é apresentado por um MER (Modelo Entidade Relacionamento), DER (Diagrama Entidade Relacionamento), DL (Diagrama Lógico) e o seu respectivo Dicionário de Dados.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 23/09/2020 | 1.0 | Criação das classes e seus atributos | Gabriel Alves, Gabriel Davi, Micaella Gouviea, Pedro Igor e Sofia Patrocínio |
| 25/09/2020 | 1.1 | Criação dos diagramas relacionamento e lógico | Gabriel Alves |
| 25/09/2020 | 1.2 | Corrige alguns erros de digitação e linka o documento a navbar | Pedro Igor |

## Modelo Entidade Relacionamento (MER)

### Entidades

**COMPANY** (name, document, telephone, email, photo, maxQtdCollaborator, registerDate)

**BRANCH** (idBranch, name)

**PRODUCT** (idProduct, name, unitQtd, unitMeasure, salePrice)

**LOT** (idLot, entryDate, dueDate, qtdProdutos, description, purchasePrice)

**CATEGORY** (idCategory, name, description)

**COLLABORATOR** (idCollaborator, name, document, acessLevel, photo, password)

**ACCESS_LEVEL** (idAccessLevel, name)

**FEEDBACK** (idFeedback, type, description, document, annex)

**TYPE_FEEDBACK** (idTypeFeedback, name)

### Relacionamentos

**COMPANY** - stocks - **PRODUCT**<br>
Uma COMPANY pode estocar nenhum ou vários PRODUCTS e um PRODUCT pode ser estocado por uma e no máximo uma COMPANY. <br>
**Cardinalidade -> 1:n**

**COMPANY** - belongs - **BRANCH**<br>
Uma COMPANY pertence a uma e somente uma BRANCH e uma BRANCH pode possuir nenhuma ou várias COMPANYS.<br>
**Cardinalidade -> n:1**

**COMPANY** - has - **COLLABORATOR**<br>
Uma COMPANY possui um ou vários COLLABORATOR e um COLLABORATOR pertence a uma e somente uma COMPANY.<br>
**Cardinalidade -> 1:n**

**LOT** - composes - **PRODUCT**<br>
Um LOT pode compor um e no máximo um PRODUCT e um PRODUCT pode ser composto por nenhum ou vários LOTs.<br>
**Cardinalidade -> n:1**

**PRODUCT** - belongs - **CATEGORY**<br>
Um PRODUCT pode pertencer a um ou a várias CATEGORYS e uma CATEGORY pode ser de nenhum ou vários PRODUCTS.<br>
**Cardinalidade -> n:m**

**COLLABORATOR** - fills - **LOT**<br>
Um COLLBORATOR pode popular nenhum ou vários LOTS e um LOT pode ser populado por um e apenas um COLLABORATOR.<br>
**Cardinalidade -> 1:n**

**COLLABORATOR** - registers - **PRODUCT**<br>
Um COLLABORATOR pode registrar nenhum ou vários PRODUCTS e um PRODUCT pode ser registrado por um e apenas um COLLABORATOR.<br>
**Cardinalidade -> 1:n**

**COLLABORATOR** - decreases - **LOT**<br>
Um COLLBORATOR pode decrementar nenhum ou vários LOTS e um LOT pode ser decrementado por um ou vários COLLBORATORS.<br>
**Cardinalidade -> n:m**

**FEEDBACK** - has - **TYPE_FEEDBACK**<br>
Um FEEDBACK pode possuir um e no máximo um tipo de FEEDBACK e um tipo de FEEDBACK pode possuir nenhum ou vários FEEDBACKS.<br>
**Cardinalidade -> n:1**

**COLLABORATOR** - sends - **FEEDBACK**<br>
Um COLLABORATOR pode enviar nenhum ou vários FEEDBACKS e um FEEDBACK pode ser enviado por um e apenas um COLLABORATOR.<br>
**Cardinalidade -> 1:n**

**COLLABORATOR** - has - **ACCESS_LEVEL**<br>
Um COLLABORATOR pode ter um e somente um ACCESS_LEVEL e um nível de ACCESS_LEVEL pode ter nenhum ou vários COLLABORATORS.<br>
**Cardinalidade -> n:1**

## Diagrama Entidade Relacionamento (DER)

![Diagrama Entidade Relacionamento](../../assets/img/bancoDados/Modelo_STOCK.png)

## Diagrama Lógico

![Diagrama Entidade Relacionamento](../../assets/img/bancoDados/LOGICO_STOCK.png)