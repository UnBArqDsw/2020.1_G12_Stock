# UC011 - [Feedback](Modeling/verbo?id=feedback)

## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 30/09/2020 | 1.0 | Criação do documento e template | Micaella Gouveia |
| 30/09/2020 | 1.1 | Adição da descrição, atores, pré-requisitos, fluxos e pós condição | Micaella Gouveia |
| 30/09/2020 | 1.2 | Linkagem dos léxicos | Micaella Gouveia |

## Descrição
O  [usuário](Modeling/objeto?id=usuário) deve poder enviar [feedbacks](Modeling/verbo?id=feedback) para o Suporte Técnico.

## Atores
* [Usuário](Modeling/objeto?id=usuário)
* Sistema
* Suporte Técnico

## Pré-requisitos
O  [usuário](Modeling/objeto?id=usuário) não deve estar na tela de [Feedback](Modeling/verbo?id=feedback).

## Fluxo de Eventos
### Fluxo Principal
1. O [usuário](Modeling/objeto?id=usuário) deve entrar no Stock com suas credenciais.
2. O [usuário](Modeling/objeto?id=usuário) deve entrar na tela de [Feedback](Modeling/verbo?id=feedback).
3. O [usuário](Modeling/objeto?id=usuário) deve selecionar o tipo de [feedback](Modeling/verbo?id=feedback).
4. O [usuário](Modeling/objeto?id=usuário) deve escrever seu [feedback](Modeling/verbo?id=feedback).
5. O [usuário](Modeling/objeto?id=usuário) deve selecionar o botão de "Enviar".
6. O Sistema mostrará uma mensagem de sucesso.
7. O Suporte Técnico receberá esse [feedback](Modeling/verbo?id=feedback).

### Fluxos Alternativos
*Não há fluxos alternativos*

### Fluxos de Exceção
* **FE01**: Campo de descrição do [feedback](Modeling/verbo?id=feedback) não preenchido.
    1. O [usuário](Modeling/objeto?id=usuário) deve entrar no Stock com suas credenciais.
    2. O [usuário](Modeling/objeto?id=usuário) deve entrar na tela de [Feedback](Modeling/verbo?id=feedback).
    3. O [usuário](Modeling/objeto?id=usuário) deve selecionar o tipo de [feedback](Modeling/verbo?id=feedback).
    4. O [usuário](Modeling/objeto?id=usuário) não preenche a descrição do [feedback](Modeling/verbo?id=feedback).
    5. O [usuário](Modeling/objeto?id=usuário) deve selecionar o botão de "Enviar".
    6. O Sistema alertará que há campos não preenchidos.



## Pós-condição

O [feedback](Modeling/verbo?id=feedback) será enviado para o Suporte Técnico, e caso precise, entrará em contato com o [Owner](Modeling/objeto?id=Owner) da empresa.
