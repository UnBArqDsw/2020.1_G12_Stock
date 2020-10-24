# UC05 - Cadastro de Produto

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 30/09/2020 | 1.0 | Criação do documento e template | Micaella Gouveia |
| 30/09/2020 | 1.1 | Adição da descrição, atores, pré-requisitos, fluxos e pós condição | Micaella Gouveia |
| 30/09/2020 | 1.2 | Linkagem dos léxicos | Micaella Gouveia |
| 01/10/2020 | 1.3 | Adição do diagrama | Micaella Gouveia |
| 24/10/2020 | 1.4 | Atualização do diagrama conforme padrões implementados (Diagrama V.1)| Micaella Gouveia e Sofia Patrocínio|

## Diagrama - UC05
Diagrama produzido com a ferramenta a ferramenta [Draw.io](https://app.diagrams.net/). Ele é composto por:
* Atores
* Casos de uso
* Relacionamentos

### Diagrama (V.1)

![caso 5](../../../assets/diagramas/casosUso/v1/caso5V1.png)

<a href="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/pdf/diagramas/casosUso/v1/caso5V1.pdf">Arquivo em PDF</a>

### Diagrama (V.0)

![caso 5](../../../assets/diagramas/casosUso/caso5.png)

<a href="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/pdf/diagramas/casosUso/caso5.pdf">Arquivo em PDF</a>

## Descrição
O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve [cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto) no [estoque](Modeling/objeto?id=Estoque).

## Atores
* [Usuário Owner](Modeling/objeto?id=Owner)
* [Usuário Admin](Modeling/objeto?id=Admin)
* Sistema

## Pré-requisitos
O [produto](Modeling/objeto?id=Produto) não deve estar cadastrado no [estoque](Modeling/objeto?id=Estoque).

## Fluxo de Eventos
### Fluxo Principal
1. O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve entrar no Stock com suas credenciais.
2. O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve entrar na tela de [Estoque](Modeling/objeto?id=Estoque).
3. O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve selecionar o botão "Novo [Produto](Modeling/objeto?id=Produto)".
4. O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve preencher as informações do novo [produto](Modeling/objeto?id=Produto).
5. O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve selecionar o botão "Adicionar".
6. O  novo [produto](Modeling/objeto?id=Produto) será cadastrado no [estoque](Modeling/objeto?id=Estoque).

### Fluxos Alternativos
*Não existem fluxos alternativos*

### Fluxos de Exceção
* **FE01**: [Produto](Modeling/objeto?id=Produto) já cadastrado
    1. O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve entrar no Stock com suas credenciais.
    2. O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve entrar na tela de [Estoque](Modeling/objeto?id=Estoque).
    3. O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve selecionar o botão "Novo [Produto](Modeling/objeto?id=Produto)".
    4. O [usuário Owner](Modeling/objeto?id=Owner)/[Admin](Modeling/objeto?id=Admin) deve preencher as informações do novo [produto](Modeling/objeto?id=Produto).
    5. O [produto](Modeling/objeto?id=Produto) já está cadastrado.
    6. O Sistema enviará uma mensagem de [produto](Modeling/objeto?id=Produto) já cadastrado.

## Pós-condição
 O  novo [produto](Modeling/objeto?id=Produto) será cadastrado no [estoque](Modeling/objeto?id=Estoque).

## Referências
* UML — Diagrama de Casos de Uso: <https://medium.com/operacionalti/uml-diagrama-de-casos-de-uso-29f4358ce4d5>. Último acesso em 01/10/2020.