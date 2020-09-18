# Verbos

## Histórico de Revisões

|    Data    | Versão |             Descrição             |                                  Autor(es)                                  |
| :--------: | :----: | :-------------------------------: | :-------------------------------------------------------------------------: |
| 08/09/2020 |  1.0   |        Sugestão de Léxicos        | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 09/09/2020 |  1.1   |     Estruturação dos léxicos      |                                Gabriel Alves                                |
| 10/09/2020 |  1.2   | Revisão e finalização dos léxicos | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 11/09/2020 |  1.3   |       Criação do documento        |                                Gabriel Alves                                |
| 11/09/2020 |  1.4   |       Linkagem dos léxicos.       | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 17/09/2020 |  1.5   |       Adição do léxico de feedback e fluxo      | Gabriel Davi |

<br>

### Filtrar Produtos

|                                                                  Noção                                                                   |                                                                                                                    Impacto                                                                                                                    | Sinônimos |
| :--------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------: |
| Ação realizada pelo usuário. <br><br>Colaborador filtra [produtos](Modeling/objeto?id=Produto) do [estoque](Modeling/objeto?id=Estoque). | Se o filtro estiver ligado alguns [produtos](Modeling/objeto?id=Produto) não ficarão visíveis. <br> [Filtrar produtos](Modeling/verbo?id=Filtrar-Produtos) economiza tempo do usuário para encontrar o [produto](Modeling/objeto?id=Produto). |     -     |

### Baixa em Produto

|                                                                  Noção                                                                   |                                                      Impacto                                                      |                                                 Sinônimos                                                  |
| :--------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------: | :--------------------------------------------------------------------------------------------------------: |
| Realizar a venda de um [produto](Modeling/objeto?id=Produto). <br><br>Realizar distribuição de um [produto](Modeling/objeto?id=Produto). | É preciso [dar baixa](Modeling/verbo?id=Baixa-em-Produto) nos itens que foram vendidos ou foram para outro setor. | Vender [produto](Modeling/objeto?id=Produto), dar saída de [produto](Modeling/objeto?id=Produto), remover. |

### Importação

|                             Noção                              |                                                                                                   Impacto                                                                                                    |      Sinônimos      |
| :------------------------------------------------------------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-----------------: |
| Aquisição de um bem de um lugar externo para um lugar interno. | Precisa importar a planilha para o computador. <br><br>Precisa importar o [produto](Modeling/objeto?id=Produto) do [fornecedor](Modeling/objeto?id=Fornecedor) para o [estoque](Modeling/objeto?id=Estoque). | Entrada, aquisição. |

### Exportação

|                           Noção                            |                                                       Impacto                                                        | Sinônimos |
| :--------------------------------------------------------: | :------------------------------------------------------------------------------------------------------------------: | :-------: |
| Saída de um bem de um lugar interno para um lugar externo. | Precisa exportar a planilha do computador. <br><br>Precisa exportar o [produto](Modeling/objeto?id=Produto) da loja. |  Saída.   |

### Cadastrar Produto

|                          Noção                          |                                           Impacto                                           |                                                                                                              Sinônimos                                                                                                              |
| :-----------------------------------------------------: | :-----------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
| Usuário cadastra [produto](Modeling/objeto?id=Produto). | Ter um novo [produto](Modeling/objeto?id=Produto) em [estoque](Modeling/objeto?id=Estoque). | Registrar [produto](Modeling/objeto?id=Produto).<br><br>Dar load em [estoque](Modeling/objeto?id=Estoque).<br><br>Adcionar [produto](Modeling/objeto?id=Produto), adição de [produto](Modeling/objeto?id=Produto), adição de itens. |

### Alertar

|           Noção            |                                                                                             Impacto                                                                                             |     Sinônimos      |
| :------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :----------------: |
| Sinalizar algo importante. | Se o estoque estiver vazio ou baixo o [usuário](Modeling/objeto?id=usuário) será avisado.<br><br> Se um [produto](Modeling/objeto?id=Produto) estiver prestes a vencer, o usuário será avisado. | Sinalizar, avisar. |

### Armazenar

|                             Noção                             |                                            Impacto                                             | Sinônimos |
| :-----------------------------------------------------------: | :--------------------------------------------------------------------------------------------: | :-------: |
| Manter ou conservar em [estoque](Modeling/objeto?id=Estoque). | O [usuário](Modeling/objeto?id=usuário) poderá encher o [estoque](Modeling/objeto?id=Estoque). | Estocar.  |

### Dar Entrada

|                                                                                                                                   Noção                                                                                                                                    |                                                                                                                     Impacto                                                                                                                     |                    Sinônimos                    |
| :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :---------------------------------------------: |
| Realizada pelo [usuário](Modeling/objeto?id=usuário). <br><br> [Usuário](Modeling/objeto?id=usuário) dá entrada do [produto](Modeling/objeto?id=Produto) no [estoque](Modeling/objeto?id=Estoque) quando o [fornecedor](Modeling/objeto?id=Fornecedor) realizar a entrega. | Se o [estoque](Modeling/objeto?id=Estoque) estiver cheio, o usuário irá [Alertar](Modeling/verbo?id=Alertar) o [Admin](Modeling/objeto?id=Admin) ou [Owner](Modeling/objeto?id=Owner) que não cabe mais [produtos](Modeling/objeto?id=Produto). | Comprar [produtos](Modeling/objeto?id=Produto). |

### Consultar produto

|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Realizada pelo [usuário](Modeling/objeto?id=usuário). <br><br> [Usuário](Modeling/objeto?id=usuário) [consulta produtos](Modeling/verbo?id=Consultar-Produto) disponíveis no [estoque](Modeling/objeto?id=Estoque). | Mostrará informações sobre o [produto](Modeling/objeto?id=Produto). | Conferir [produto](Modeling/objeto?id=Produto). <br><br> Acompanhar [produto](Modeling/objeto?id=Produto).|


### Controle de Estoque

|                       Noção                       |                                                                          Impacto                                                                          |                                                Sinônimos                                                 |
| :-----------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------------------------------------------: | :------------------------------------------------------------------------------------------------------: |
| Realizada pelo [Admin](Modeling/objeto?id=Admin). | O [Admin](Modeling/objeto?id=Admin) controlará melhor o [estoque](Modeling/objeto?id=Estoque) com o auxílio do [Dashboard](Modeling/objeto?id=Dashboard). | Gestão de [estoque](Modeling/objeto?id=Estoque), gerenciamento de [estoque](Modeling/objeto?id=Estoque). |

### Prototipação

|                           Noção                            |              Impacto               |             Sinônimos              |
| :--------------------------------------------------------: | :--------------------------------: | :--------------------------------: |
| Ato de gerar um [protótipo](Modeling/objeto?id=protótipo). | O designer prototipou a aplicação. | Criar um protótipo.<br>Prototipar. |

### Feedback
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Feedbak é o ato de disponibilizar uma opinião ou análise sobre determinado objeto ou situação | [Stakeholders](Modeling/objeto.md?id=stakeholder) dão seu feedback sobre o [produto](Modeling/objeto.md?id=produto). <br><br> [desenvolvedores](Modeling/objeto?id=desenvolvedor) melhoram seus [aplicativos](Modeling/objeto?id=web-app) basedado no feedback de seus clientes. | Dar feedback. <br><br>  |

### Fluxo
|   Noção   |   Impacto   |   Sinônimos    |
|  :-----:  |  :-------:  |  :---------:   |
| Fluxo indica um equilíbrio dinâmico de um sisteme ou ambiente, no qual possuimo entrada e saida de elementos de seu meio | Um negócio possui um fluxo de produto, ou de caixa <br><br>  [aplicativos](Modeling/objeto?id=web-app) possuem fluxos de usabilidade. | Entrada e saida.  |