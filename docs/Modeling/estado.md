# Estados

## Histórico de Revisões

|    Data    | Versão |         Descrição         |           Autor(es)            |
| :--------: | :----: | :-----------------------: | :----------------------------: |
|  08/09/2020 |  1.0   |  Sugestão de Léxicos  | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 09/09/2020 |  1.1   |  Estruturação dos léxicos  | Gabriel Alves | 
| 10/09/2020 |  1.2   |  Revisão e finalização dos léxicos | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 11/09/2020 |  1.3   |  Criação do documento | Gabriel Alves |
| 11/09/2020 |  1.4   |  Linkagem dos léxicos. | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |

### Deploy
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Deploy é um estado que descreve quando uma aplicação está saindo da fase de desenvolvimento para produção. | A aplicação está em deploy <br><br> A aplicação sofreu deploy. | - |

### Estoque baixo
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| O [estoque](Modeling/objeto?id=Estoque) é dito como estoque baixo quando há um número relativamente pequeno de [produtos](Modeling/objeto?id=Produto) em suas dependências. | O [vendedor](Modeling/objeto?id=Seller) tem que repor o [estoque](Modeling/objeto?id=Estoque) baixo. <br><br> A loja está com poucos [produtos](Modeling/objeto?id=Produto) no [estoque](Modeling/objeto?id=Estoque). | [Estoque](Modeling/objeto?id=Estoque) escasso. <br><br> [Estoque](Modeling/objeto?id=Estoque) com poucos [produtos](Modeling/objeto?id=Produto). |

### Estoque Cheio
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Quando a quantidade de [produtos](Modeling/objeto?id=Produto) disponíveis preenche todo o [estoque](Modeling/objeto?id=Estoque).|A loja está com muitos [produtos](Modeling/objeto?id=Produto) no [estoque](Modeling/objeto?id=Estoque). <br><br> Todos os [produtos](Modeling/objeto?id=Produto) chegaram.| Estoque lotado. <br><br> Estoque com muitos [produtos](Modeling/objeto?id=Produto). |

### Estoque Vazio
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Quando não há [produtos](Modeling/objeto?id=Produto) disponíveis no [estoque](Modeling/objeto?id=Estoque). | A loja está com o [estoque](Modeling/objeto?id=Estoque) esgotado. <br><br> Não há registro de [estoque](Modeling/objeto?id=Estoque) na aplicação. |[Estoque](Modeling/objeto?id=Estoque) esgotado. <br><br> [Estoque](Modeling/objeto?id=Estoque) sem [produtos](Modeling/objeto?id=Produto). <br><br> [Estoque](Modeling/objeto?id=Estoque) em falta. |

### Em produção
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Uma aplicação está em produção quando está no ar em pronto para uso. | O site entra em produção. <br><br> O site deu problema em produção. <br><br> O programador consertou o [bug](Modeling/objeto?id=Bug) em produção. | Aplicação no ar. <br><br> Aplicação que sofreu [deploy](Modeling/estado?id=Deploy)|

### Em desenvolvimento
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Uma aplicação está em desenvolvimento quando [desenvolvedors](Modeling/objeto?id=Desenvolvedor) estão trabalhando na criação das funcionalidades do projeto.| A aplicação está em desenvolvimento <br><br> Acabou a fase de desenvolvimento, agora os [desenvolvedores](Modeling/objeto?id=Desenvolvedor) vão fazer o [deploy](Modeling/estado?id=Deploy)| Em progresso. <br><br> Em implementação. <br><br> Em homologação.|