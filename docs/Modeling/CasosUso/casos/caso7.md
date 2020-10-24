# UC07 - Baixa em Produto

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 30/09/2020 | 1.0 | Criação do documento e template | Micaella Gouveia |
| 30/09/2020 | 1.1 | Adição da descrição, atores, pré-requisitos, fluxos e pós condição | Micaella Gouveia |
| 30/09/2020 | 1.2 | Linkagem dos léxicos | Micaella Gouveia |
| 01/10/2020 | 1.3 | Adição do diagrama | Micaella Gouveia |

## Diagrama - UC07
Diagrama produzido com a ferramenta a ferramenta [Draw.io](https://app.diagrams.net/). Ele é composto por:
* Atores
* Casos de uso
* Relacionamentos

### Diagrama (V.0)
![caso 7](../../../assets/diagramas/casosUso/caso7.png)

<a href="https://unbarqdsw.github.io/2020.1_G12_Stock/assets/pdf/diagramas/casosUso/caso7.pdf">Arquivo em PDF</a>

## Descrição
O [usuário](Modeling/objeto?id=usuário) deve dar baixa em produto.

## Atores
* [Usuário](Modeling/objeto?id=usuário)
* Sistema

## Pré-requisitos
O [produto](Modeling/objeto?id=Produto) não deve estar disponível no [estoque](Modeling/objeto?id=Estoque).

## Fluxo de Eventos
### Fluxo Principal
1. O [usuário](Modeling/objeto?id=usuário) deve entrar no Stock com suas credenciais.
2. O [usuário](Modeling/objeto?id=usuário) deve entrar na tela de [Estoque](Modeling/objeto?id=Estoque).
3. O [usuário](Modeling/objeto?id=usuário) deve fazer uma busca pelo [produto](Modeling/objeto?id=Produto) desejado.
4. O [produto](Modeling/objeto?id=Produto) será disponibilizado.
5. O [usuário](Modeling/objeto?id=usuário) deve selecionar o [produto](Modeling/objeto?id=Produto).
6. O [usuário](Modeling/objeto?id=usuário) deve selecionar o botão "Dar baixa".
7. O [usuário](Modeling/objeto?id=usuário) deverá selecionar a quantidade.
8. O Sistema mostrará uma mensagem de confirmação.
9. O [usuário](Modeling/objeto?id=usuário) deve confirmar a ação.
10. A quantidade selecionada do [produto](Modeling/objeto?id=Produto) será retirada do [estoque](Modeling/objeto?id=Estoque).
11. A venda será contabilizada para o colaborador que realizou a baixa.

### Fluxos Alternativos
*Não há fluxos alternativos*

### Fluxos de Exceção
* **FE01**: Produto indisponível
    1. O [usuário](Modeling/objeto?id=usuário) deve entrar no Stock.
    2. O [usuário](Modeling/objeto?id=usuário) deve entrar na tela de [Estoque](Modeling/objeto?id=Estoque).
    3. O [usuário](Modeling/objeto?id=usuário) deve fazer uma busca pelo [produto](Modeling/objeto?id=Produto) desejado.
    6. O [produto](Modeling/objeto?id=Produto) se encontra indisponível.
    7. O Sistema mostrará mensagem de [produto](Modeling/objeto?id=Produto) indisponível.

* **FE02**: Produto não cadastrado
    1. O [usuário](Modeling/objeto?id=usuário) deve entrar no Stock.
    2. O [usuário](Modeling/objeto?id=usuário) deve entrar na tela de [Estoque](Modeling/objeto?id=Estoque).
    3. O [usuário](Modeling/objeto?id=usuário) deve fazer uma busca pelo [produto](Modeling/objeto?id=Produto) desejado.
    6. O [produto](Modeling/objeto?id=Produto) não foi cadastrado.
    7. O Sistema não retornará o [produto](Modeling/objeto?id=Produto) na busca feita.

## Pós-condição
O [produto](Modeling/objeto?id=Produto) será vendido e retirado do [estoque](Modeling/objeto?id=Estoque).

## Referências
* UML — Diagrama de Casos de Uso: <https://medium.com/operacionalti/uml-diagrama-de-casos-de-uso-29f4358ce4d5>. Último acesso em 01/10/2020.