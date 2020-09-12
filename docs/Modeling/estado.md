# Estados

## Histórico de Revisões

|    Data    | Versão |         Descrição         |           Autor(es)            |
| :--------: | :----: | :-----------------------: | :----------------------------: |
|  08/09/2020 |  0.1   |  Sugestão de Léxicos  | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 09/09/2020 |  0.2   |  Estruturação dos léxicos  | Gabriel Alves | 
| 10/09/2020 |  0.3   |  Revisão e finalização dos léxicos | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 11/09/2020 |  1.0   |  Criação do documento | Gabriel Alves |

### Deploy
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Deploy é um estado que descreve quando uma aplicação está saindo da fase de desenvolvimento para produção. | A aplicação está em deploy <br><br> A aplicação sofreu deploy. | - |

### Prazo de Validade
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- tempo que os [produto](../Modeling/objeto?id=produto) podem ser armazenados mantendo sua qualidade aceitável.|- a validade do [produto](../Modeling/objeto?id=produto) está acabando.|- serventia do [produto](../Modeling/objeto?id=produto), vida útil do [produto](../Modeling/objeto?id=produto), validade do [produto](../Modeling/objeto?id=produto).|

### Estoque baixo
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- O [estoque](../Modeling/objeto?id=Estoque) é dito como [estoque](../Modeling/objeto?id=Estoque) baixo quando há um número relativamente pequeno de [produto](../Modeling/objeto?id=produto) em suas dependências|- O [Vendedor](../Modeling/objeto?id=vendedor) tem que repor o [estoque](../Modeling/objeto?id=Estoque) baixo <br> - A loja está com poucos [produto](../Modeling/objeto?id=produto) no [estoque](../Modeling/objeto?id=Estoque)|- [estoque](../Modeling/objeto?id=Estoque) escasso <br> - [estoque](../Modeling/objeto?id=Estoque) com poucos [produto](../Modeling/objeto?id=produto)|

### Estoque Cheio
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Quando a quantidade de [produtos](../Modeling/objeto?id=produto) disponíveis preenche todo o [estoque](../Modeling/objeto?id=Estoque).|- A loja está com muitos [produto](../Modeling/objeto?id=produto) no [estoque](../Modeling/objeto?id=Estoque) <br>- Todos os [produto](../Modeling/objeto?id=produto) chegaram.|- Estoque lotado <br>- Estoque com muitos [produtos](../Modeling/objeto?id=produto)|

### Estoque Vazio
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Quando não há [produtos](../Modeling/objeto?id=produto) disponíveis no estoque|- A loja está com o estoque esgotado <br>- Não há registro de estoque na aplicação|- Estoque esgotado <br>- [estoque](../Modeling/objeto?id=Estoque) sem [produtos](../Modeling/objeto?id=produto) <br>- [estoque](../Modeling/objeto?id=Estoque) em falta|

### Em produção
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Uma aplicação está em produção quando está no ar em pronto para uso |- O site entra em produção <br>- O site deu problema em produção <br>- O programador consertou o [bug](../Modeling/objeto?id=Bug) em produção|- Aplicação no ar <br>- aplicação que sofreu [deploy](../Modeling/estado?id=deploy)|

### Em desenvolvimento
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
|- Uma aplicação está em desenvolvimento quando [desenvolvedores](../Modeling/objeto?id=desenvolvedor) estão trabalhando na criação das funcionalidades do projeto.|- A aplicação está em desenvolvimento <br>- Acabou a fase de desenvolvimento, agora os [desenvolvedores](../Modeling/objeto?id=desenvolvedor) vão fazer o [deploy](../Modeling/estado?id=deploy)|- em progresso|
