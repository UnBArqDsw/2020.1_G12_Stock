# UC02 - Login do Usuário

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 30/09/2020 | 1.0 | Criação do documento e template | Micaella Gouveia |
| 30/09/2020 | 1.1 | Adição da descrição, atores, pré-requisitos, fluxos e pós condição | Micaella Gouveia |
| 30/09/2020 | 1.2 | Linkagem dos léxicos | Micaella Gouveia |
| 01/10/2020 | 1.3 | Adição do diagrama | Micaella Gouveia |

## Diagrama - UC02
Diagrama produzido com a ferramenta a ferramenta [Draw.io](https://app.diagrams.net/). Ele é composto por:
* Atores
* Casos de uso
* Relacionamentos

![caso 2](../../../assets/diagramas/casosUso/caso2.png)

## Descrição
O [usuário](Modeling/objeto?id=usuário) cadastrado deve fazer o Login na aplicação.

## Atores
* [Usuário](Modeling/objeto?id=usuário)
* Sistema

## Pré-requisitos
1. O [usuário](Modeling/objeto?id=usuário) deve possuir um cadastro na aplicação.
2. O [usuário](Modeling/objeto?id=usuário) não deve estar logado na aplicação.

## Fluxo de Eventos
### Fluxo Principal
1. O [usuário](Modeling/objeto?id=usuário) que não está logado entra no Stock.
2. O [usuário](Modeling/objeto?id=usuário) seleciona o botão "Entrar".
3. O Sistema valida suas credenciais.
4. O [usuário](Modeling/objeto?id=usuário) passa a estar logado na aplicação.

### Fluxos Alternativos
* **FA01**: 
    1. O [usuário Owner](Modeling/objeto?id=Owner) que não está logado entra no Stock.
    2. O [usuário Owner](Modeling/objeto?id=Owner) seleciona o botão "Portal do Gestor".
    3. O Sistema valida suas credenciais.
    4. O [usuário Owner](Modeling/objeto?id=Owner) passa a estar logado na aplicação.
* **FA02**:
    1. O [usuário Admin](Modeling/objeto?id=Admin) que não está logado entra no Stock.
    2. O [usuário Admin](Modeling/objeto?id=Admin) seleciona o botão "Portal do Gestor".
    3. O Sistema valida suas credenciais.
    4. O [usuário Admin](Modeling/objeto?id=Admin) passa a estar logado na aplicação.

### Fluxos de Exceção
* **FE01**: Conta Bloqueada
    1. O [usuário](Modeling/objeto?id=usuário) que não está logado entra no Stock.
    2. O [usuário](Modeling/objeto?id=usuário) seleciona o botão "Entrar".
    3. O Sistema verifica que o [usuário](Modeling/objeto?id=usuário) foi bloqueado pelo [usuário Owner](Modeling/objeto?id=Owner).
    4. O Sistema manda uma mensagem de bloqueio do [usuário](Modeling/objeto?id=usuário).
* **FE01**: Empresa Removida
    1. O [usuário](Modeling/objeto?id=usuário)  que não está logado entra no Stock.
    2. O [usuário](Modeling/objeto?id=usuário)  seleciona o botão "Portal do Gestor".
    3. O Sistema verifica que a empresa cadastrada foi removida
    4. O Sistema manda uma mensagem de remoção da empresa.
* **FE03**: Credenciais inválidas
    1. O [usuário](Modeling/objeto?id=usuário) que não está logado entra no Stock.
    2. O [usuário](Modeling/objeto?id=usuário) seleciona o botão "Entrar".
    3. O Sistema não valida as credenciais.
    4. O Sistema manda uma mensagem de credenciais inválidas.
    
## Pós-condição
O [usuário](Modeling/objeto?id=usuário) pode entrar na sua conta do Stock.

## Referências
* UML — Diagrama de Casos de Uso: <https://medium.com/operacionalti/uml-diagrama-de-casos-de-uso-29f4358ce4d5>. Último acesso em 01/10/2020.