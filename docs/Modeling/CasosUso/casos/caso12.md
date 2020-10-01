# UC012 - Alerta ao Usuário

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 30/09/2020 | 1.0 | Criação do documento e template | Micaella Gouveia |
| 30/09/2020 | 1.1 | Adição da descrição, atores, pré-requisitos, fluxos e pós condição | Micaella Gouveia |
| 30/09/2020 | 1.2 | Linkagem dos léxicos | Micaella Gouveia |

## Descrição
O [usuário](Modeling/objeto?id=usuário) deve receber alertas caso algum [produtos](Modeling/objeto?id=Produto) ultrapasse seu prazo de validade.

## Atores
* [Usuário](Modeling/objeto?id=usuário)
* Sistema

## Pré-requisitos
O produto não deve estar ter seu lote cadastrado no [estoque](Modeling/objeto?id=Estoque).

## Fluxo de Eventos
### Fluxo Principal
1. O [usuário](Modeling/objeto?id=usuário) deve entrar no Stock com suas credenciais.
2. O Sistema alertará o [usuário](Modeling/objeto?id=usuário) no ícone de Alertas.
3. O [usuário](Modeling/objeto?id=usuário) deve selecionar o ícone de Alertas.
4. O [usuário](Modeling/objeto?id=usuário) deve poder visualizar suas notificações, podendo ser alertas de prazo de validade ou de quantidade mínima de [produto](Modeling/objeto?id=Produto).

### Fluxos Alternativos
*Não há fluxos alternativos*

### Fluxos de Exceção
*Não há fluxos de exceção*

## Pós-condição
 A [usuário](Modeling/objeto?id=usuário) saberá se algum [produto](Modeling/objeto?id=Produto) passou do prazo de validade ou atingiu sua quantidade mínima.

## Referências
* UML — Diagrama de Casos de Uso: <https://medium.com/operacionalti/uml-diagrama-de-casos-de-uso-29f4358ce4d5>. Último acesso em 01/10/2020.