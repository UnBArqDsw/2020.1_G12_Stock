# Projeto Banco de Dados
**Este artefato foi produzido durante o dia 2 da Diagrams Sprint, para saber mais sobre a metodologia e como ela foi feita, clique aqui: _[Diagrams Sprint](Modeling/Diagrams/Diagrams.md)_**

O Projeto de banco de dados tem por finalidade, modelar todo o banco de dados do sistema com suas respectivas tabelas e relacionamento. Nesse documento é apresentado por um MER Modelo Entidade Relacionamento, DER Diagrama Entidade Relacionamento, DL Diagrama Lógico e o seu respectivo Dicionário de Dados.

## Histórico de Revisões
| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 23/09/2020 | 1.0 | Criação das classes e seus atributos | Gabriel Alves, Gabriel Davi, Micaella Gouviea, Pedro Igor e Sofia Patrocínio |

## Modelo Entidade Relacionamento (MER)

### Entidades

COMPANY (name, document, branch, telephone, email, photo, maxQtdCollaborator, registerDate)

BRANCH(id, name)

PRODUCT (id, name, category, unitQtd, unitMeasure, salePrice)

LOT (id, entryDate, dueDate, qtdProdutos, description, purchasePrice)

CATEGORY (id, name, description)

COLLABORATOR (id, name, document, acessLevel, photo)

ACESS_LEVEL (id, name)

FEEDBACK (id, type, description, document, annex)

TYPE_FEEDBACK (id, name)

