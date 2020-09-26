# Questionário

**Este artefato foi produzido durante o dia 1 da Design Sprint, para saber mais sobre a metodologia e como ela foi feita, clique aqui: _[Design Sprint](DesignSprint/DesignSprint.md)_**

O questionário é um método de elicitação de requisitos onde, por meio de perguntas estratégicas, é possível compreender melhor como o público de interesse reage a determinado assunto. Além disso, o questionário permite retirar características chave sobre um domínio quantificando o percentual de pessoas, do público, que se aplicam a determinada característica.<br><br>
As perguntas a seguir foram elaboradas em um dos dias de [Design Sprint](DesignSprint/DesignSprint.md) realizado pelo grupo. As perguntas foram escritas a princípio, individualmente por cada um dos membros do grupo, e discutidas em conjunto logo em seguida, planejando a melhor estratégia. Após o entendimento da finalidade do questionário para o projeto, foi feita a etapa de desenho, em que membro sugeriu perguntas relevantes. Em seguida, discussão em grupo onde foram decididas as melhores perguntas e traçado um objetivo, [protototipação](/Modeling/verbo?id=prototipação), gerando a presente documentação, e teste, enviando o Formulário em grupos específicos.

## Histórico de Revisões

|    Data    | Versão |                                                      Descrição                                                       |                                  Autor(es)                                  |
| :--------: | :----: | :------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------: |
| 04/09/2020 |  1.0   |                                      Adicionado questionário definido em grupo.                                      |          Gabriel Alves, Gabriel Davi, Micaella, Pedro Igor e Sofia          |
| 04/09/2020 |  1.1   | Formatação do questionário, tabela de versões, referências, criação do formulário e explicação breve da metodologia. |                                 Pedro Igor                                  |
| 09/09/2020 |  1.2   |                                   Adição de hyperlink para página de Design Sprint                                   |                              Sofia Patrocínio                               |
| 11/09/2020 |  1.3   |                                                Linkagem dos léxicos.                                                 | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 15/09/2020 |  1.4   |                                        Adição das respostas do questionário.                                         |                     Micaella Gouveia e Sofia Patrocínio                     |
| 15/09/2020 |  1.5   |                                     Levantamento dos requisitos do questionário.                                     |                     Micaella Gouveia e Sofia Patrocínio                     |
| 15/09/2020 |  1.6   |                                               adição de novos léxicos.                                               |                                Gabriel Davi                                 |
| 17/09/2020 |  1.7   |       Adição do léxico de fluxo     | Gabriel Davi |

## Respostas

**Resultado obtido em: 15/09/2020**

**1** - Você trabalha com vendas ou negócios?<br>
![Pergunta 1](../assets/questionario/1.png)<br>

**2** - A empresa a qual trabalha envolve [estoque](Modeling/objeto?id=Estoque) de [produtos](Modeling/objeto?id=Produto)?<br>
![Pergunta 2](../assets/questionario/2.png)

Apesar de termos direcionado nosso questionário à grupos com nosso [público alvo](/Modeling/objeto?id=público-alvo), como grupos de vendas e de áreas como Administração, restringimos no próprio formulário as pessoas que se aplicavam a nosso contexto. Então, **Caso Não**, finaliza o questionário. **Caso Sim**, continua:<br><br>

_Perfil pessoal:_<br><br>

**3** - Qual a sua faixa etária?<br>
![Pergunta 3](../assets/questionario/3.png)

Notamos que nosso [público alvo](/Modeling/objeto?id=público-alvo) se encontra principalmente na faixa etária de 20 a 30 anos. Esse dado é importante para dirercionarmos a "nossa persona" à esse público.<br><br>

**4** - Qual a sua afinidade com a tecnologia? Sendo 10 = Tenho muita afinidade com tecnologia e 1 = Não consigo utilizar tecnologia alguma.<br>

![Pergunta 4](../assets/questionario/4.png)

Em relação à afinidade com tecnologia, podemos concluir que nosso [público alvo](/Modeling/objeto?id=público-alvo) possui uma média alta. Trata-se de um dado fundamental como abordaremos as interfaces e funcionalidades ao [usuário](Modeling/objeto?id=usuário).<br><br>

_Perfil da empresa:_<br><br>

**5** - Qual é o ramo de negócio da empresa a qual trabalha?<br>
![Pergunta 5](../assets/questionario/5.png)

Notamos que há uma diversidade muito grande de ramos de negócios. Essa informação é importante para tornar a [aplicação](Modeling/objeto?id=Web-App) mais acessível possível para todas as categorias.<br><br>

**6** - Quantas pessoas trabalham nesta empresa (contando com [donos](Modeling/objeto?id=Owner) e sócios)?<br>
![Pergunta 6](../assets/questionario/6.png)

Podemos perceber que nosso [público alvo](/Modeling/objeto?id=público-alvo) trata-se de [micro empresas](Modeling/objeto?id=micro-empresa), com apenas o dono ou com poucos funcionários. Com essas respostas, podemos avaliar a necessidade dos [usuários](Modeling/objeto?id=usuário) em relação à quantidade de acessos ao [controle de estoque](/Modeling/verbo?id=controle-de-estoque).<br><br>

**7** - Quais os cargos dessa empresa?(Marque todos os aplicáveis)<br>
![Pergunta 7](../assets/questionario/7.png)

Sobre os cargos existentes nesses negócios, podemos perceber três que se sobrepõem:[ Dono(a)](Modeling/objeto?id=Owner), [Administrador(a)](Modeling/objeto?id=Admin) e [Vendedor(a)](Modeling/objeto?id=Seller). Essa análise valida o nível de [hierarquia](Modeling/objeto?id=Papéis-dos-colaboradores) dentro da [aplicação](Modeling/objeto?id=Web-App) .<br><br>

_Definições do [estoque](Modeling/objeto?id=Estoque):_<br><br>

**8** - Qual a frequência de reposição de [estoque](Modeling/objeto?id=Estoque)?<br>
![Pergunta 8](../assets/questionario/8.png)

Essa informação diz respeito ao [fluxo](Modeling/verbo?id=fluxo) do [estoque](Modeling/objeto?id=Estoque), fundamental para elaboração de gráficos de [controle de estoque](/Modeling/verbo?id=controle-de-estoque) e de vendas.<br><br>

**9** - Qual a quantidade de [produtos](Modeling/objeto?id=Produto) que saem do [estoque](Modeling/objeto?id=Estoque) diariamente (aproximadamente)?<br>
![Pergunta 9](../assets/questionario/9.png)

Esse dado, além de analisar o controle de saída, podemos pensar na melhoria da acurácia tendo maior rastros de vendas, como quando e por quem saiu a [mercadoria](Modeling/objeto?id=Produto).<br><br>

**10** - É possível categorizar cada [produto](Modeling/objeto?id=Produto) desta empresa?<br>
![Pergunta 10](../assets/questionario/10.png)

A categorização é muito importante para o [controle do estoque](/Modeling/verbo?id=controle-de-estoque) e a aplicação de [tags](Modeling/objeto?id=Tag) para separar [produtos](Modeling/objeto?id=Produto) por seções.<br><br>

_Aplicação:_<br><br>

**11** - Está empresa trabalha com [produtos](Modeling/objeto?id=Produto) perecíveis? <br>
![Pergunta 11](../assets/questionario/11.png)

Quase metade do nosso público respondeu que trabalha com [produtos](Modeling/objeto?id=Produto) perecíveis, o que nos mostra uma necessidade de ser possível adicionar data de [vencimento](Modeling/objeto?id=Prazo-de-Validade) dos [produtos](Modeling/objeto?id=Produto) e alertá-los quando está próximo.<br><br>

**12** - Esta empresa já teve prejuízo por não controlar o [estoque](Modeling/objeto?id=Estoque) corretamente? ([Produto](Modeling/objeto?id=Produto) passar da [data de validade](Modeling/objeto?id=Prazo-de-Validade), [produto](Modeling/objeto?id=Produto) não encontrado no [estoque](Modeling/objeto?id=Estoque))<br>
![Pergunta 12](../assets/questionario/12.png)

A maioria das empresas já tiveram prejuízo pelo mau controle do [estoque](Modeling/objeto?id=Estoque), o que significa que não utilizam/utilizaram ferramentas adequedas.<br><br>

**13** - Quais ferramentas de [controle de estoque](Modeling/verbo?id=Controle-de-Estoque) são utilizadas ou já foram utilizadas nesta empresa? (marque todas as aplicáveis)?<br>
![Pergunta 13](../assets/questionario/13.png)
A grande maioria faz controle manual dos seu [estoque](Modeling/objeto?id=Estoque), gastando mais tempo e com uma precisão menor.<br><br>

**14** - Quais problemas você já encontrou ao fazer [controle de estoque](Modeling/verbo?id=Controle-de-Estoque)? (opcional)<br>
![Pergunta 14](../assets/questionario/14.png)
Entre os problemas encontrados, é muito comum a falta de assertividade no controle: quantidade de [produto](Modeling/objeto?id=Produto) em [estoque](Modeling/objeto?id=Estoque) não bater com valor real. Além disso, podemos perceber que há problemas em separar os [produtos](Modeling/objeto?id=Produto) por categorias e dificuldade em achá-los. Há também dificuldade em controlar o [prazo de vencimento](Modeling/objeto?id=Prazo-de-Validade) dos [produtos](Modeling/objeto?id=Produto).<br><br>

## Requisitos Levantados

## Requisitos Levantados

|                                     Id                                     |                                              Nome                                               |
| :------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------: |
|   [#RF02](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |                    [Hierarquia](Modeling/objeto?id=Papéis-dos-colaboradores)                    |
|   [#RF03](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | [Adição de itens](Modeling/verbo?id=Cadastrar-Produto) ao [estoque](Modeling/objeto?id=Estoque) |
|   [#RF04](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |                   [Consulta de estoque](Modeling/verbo?id=Consultar-Produto)                    |
|   [#RF05](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |                 [Filtro por categoria](<(Modeling/verbo?id=Filtrar-Produtos)>)                  |
|   [#RF06](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |            [Tags](Modeling/objeto?id=Tag) nos [produtos](Modeling/objeto?id=Produto)            |
|   [#RF07](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    | [Remoção de itens](Modeling/verbo?id=Baixa-em-Produto) do [estoque](Modeling/objeto?id=Estoque) |
|   [#RF08](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)    |             [Cadastrar produtos](Modeling/verbo?id=Cadastrar-Produto) por planilhas             |
|   [#RF010](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)   |                                       Histórico de vendas                                       |
|   [#RF011](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)   |                                      Históricos Temporais                                       |
|   [#RF013](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)   |                      [Filtro](Modeling/verbo?id=Filtrar-Produtos) por data                      |
|   [#RF014](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)   |                                      Plotagem de gráficos                                       |
|   [#RF015](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)   |                Atualização instantânea de [estoque](Modeling/objeto?id=Estoque)                 |
|   [#RF021](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)   |           Notificação de [prazo de vencimento](Modeling/objeto?id=Prazo-de-Validade)            |
|   [#RF023](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)   |                          Cadastro de diferentes lotes do mesmo produto                          |
|   [#RF024](Elicitation/RequisitosElicitados.md?id=requisitos-funcionais)   |                             Personalização da geração dos gráficos                              |
| [#RNF04](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |                           Interface intuitiva e de fácil compreensão                            |
| [#RNF05](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |                           Suporte para múltiplos acessos simultâneos                            |
| [#RNF06](Elicitation/RequisitosElicitados.md?id=requisitos-não-funcionais) |                                 Linguagem de fácil entendimento                                 |

## Referências

- Google Forms enviado aos participantes: <https://docs.google.com/forms/d/e/1FAIpQLScm1jD2vjcqu5CZ3nuQBD3bgh19VgtuL2rltMG5WlqtbM0qcA/viewform?usp=sf_link> Último acesso em 04/09/2020.
