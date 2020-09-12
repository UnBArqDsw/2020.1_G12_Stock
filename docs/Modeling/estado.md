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
| Tempo que os produtos podem ser armazenados mantendo sua qualidade aceitável.| A validade do produto está acabando. | Serventia do produto, vida útil do produto, validade do produto.|

### Estoque baixo
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| O estoque é dito como estoque baixo quando há um número relativamente pequeno de produtos em suas dependências. | O vendedor tem que repor o estoque baixo. <br><br> A loja está com poucos produtos no estoque. | Estoque escasso. <br><br> Estoque com poucos produtos. |

### Estoque Cheio
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Quando a quantidade de produtos disponíveis preenche todo o estoque.|A loja está com muitos produtos no estoque. <br><br> Todos os produtos chegaram.| Estoque lotado. <br><br> Estoque com muitos produtos. |

### Estoque Vazio
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Quando não há produtos disponíveis no estoque. | A loja está com o estoque esgotado. <br><br> Não há registro de estoque na aplicação. |Estoque esgotado. <br><br> Estoque sem produtos. <br><br> Estoque em falta. |

### Em produção
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Uma aplicação está em produção quando está no ar em pronto para uso. | O site entra em produção. <br><br> O site deu problema em produção. <br><br> O programador consertou o bug em produção. | Aplicação no ar. <br><br> Aplicação que sofreu [deploy](Modeling/estado?id=Deploy)|

### Em desenvolvimento
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Uma aplicação está em desenvolvimento quando desenvolvedores estão trabalhando na criação das funcionalidades do projeto.| A aplicação está em desenvolvimento <br><br> Acabou a fase de desenvolvimento, agora os desenvolvedores vão fazer o [deploy](Modeling/estado?id=Deploy)| Em progresso|