# Estimativa de custos e tempo

**Este artefato foi produzido durante o dia 5 da Design Sprint, para saber mais sobre a metodologia e como ela foi feita, clique aqui: *[Design Sprint](DesignSprint/DesignSprint.md)***

Estimativa de custos tem como objetivo mensurar analiticamente o escopo de um projeto.
Para a estimativa do custo, será levado em consideração apenas o ciclo de produção do software e não o ciclo de vida por completo. Também, o modelo que será utilizado é o de custo construtivo, também conhecido como **COCOMO**.

## Histórico de Revisão

|    Data    | Versão |                         Descrição                         |                                  Autor(es)                                  |
| :--------: | :----: | :-------------------------------------------------------: | :-------------------------------------------------------------------------: |
| 05/09/2020 |  1.0   | Estimativa em equipe para o número de linhas da aplicação | Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio, Gabriel Alves |
| 05/09/2020 |  1.1   |           Abertura do documento de estimativas            |                                Gabriel Davi                                 |
| 06/09/2020 |  1.2   |     Realização dos cálculos de esforço, tempo e custo     |                                Gabriel Davi                                 |
| 09/09/2020 |  1.3   | Correção da rota de hyperlink para página de Design Sprint | Sofia Patrocínio |

## MODELO DE CUSTO CONSTRUTIVO (CONSTRUCTIVE COST MODEL - COCOMO)

COCOMO (COnstructive COst MOdel) é um modelo de estimativa paramétrico que envolve o uso de equações matemáticas para fazer estimativas de esforço, prazo e tamanho da equipe em projetos de software. Suas equações são baseadas em pesquisa e dados históricos e utilizam como entrada a quantidade de linhas de código (ou pontos de função) e a avaliação de outros aspectos relevantes para a estimativa chamados de cost drivers.
O COCOMO pode ser divido em três implementações, a depender do tipo de software que será desenvolvido e qual o grau de confiabilidade se quer chegar na estimativa de um projeto, são eles:

- **COCOMO Básico:** É um modelo estático que calcula o esforço de desenvolvimento de software e seu tempo de desenvolvimento, em função do tamanho de linhas de códigos desenvolvidas.

- **COCOMO Intermediário:** Calcula o esforço de desenvolvimento de software em função do tamanho do programa, que inclui custo, avaliação subjetiva do produto, hardware, pessoal e atributos de projeto.

- **COCOMO Detalhado:** São incorporadas características da versão intermediária com uma avaliação de impacto de custo em cada passo de todo o projeto.

**O modelo COCOMO pode ser aplicado em três classes de projetos:**

- **Modo Orgânico:** projetos simples, relativamente pequenos, com conjuntos de requisitos não tão rígidos, com equipes pequenas e experientes.
- **Modo Semidestacado:** projetos intermediários (em tamanho e complexidade), com alguns requisitos rígidos e outros não tão rígidos, com níveis mistos de experiência nas equipes.
- **Modo Embutido:** projetos com conjunto rígido de restrições operacionais, tanto de hardware, quanto de software.

Devido as particularidades do projeto a equipe o classificou como **Semidestacado**, pois as funções básicas que o software irá realizar será a listagem de produtos por categoria no estoque, adição de um produto no estoque e assim por diante, não havendo assim requisítos tão rígidos ou outras peculiaridades de implementação.

### COCOMO Intermediário

A escolha do tipo de estimativa foi o **COCOMO intermediário**, já que será necessário mais alguns fatores para trazer o projeto para produção, como hospedagem de banco de dados, hospedagem de websites e assim por diante. Isso faz com que seja necessário uma análise mais detalhada para estimativa, mas que devido a simplicidade de sua implementação não se faz necessário o uso de um **COCOMO detalhado**.

Neste modelo, o COCOMO Básico é ampliado com a finalidade de levar em consideração um conjunto de atributos direcionadores do custo que são agrupados em quatro categorias:

- **Atributos do produto:**

  - confiabilidade exigida do software;
  - tamanho do banco de dados;
  - complexidade do produto.

- **Atributos do hardware:**

  - restrições ao tempo de execução;
  - restrições de memória;
  - volatilidade do ambiente de máquina virtual;
  - tempo de turnaround (tempo para completar o ciclo) exigido.

- **Atributos de pessoal:**

  - capacidade do analista;
  - experiência em aplicações;
  - capacidade do programador;
  - experiência em máquina virtual;
  - experiência com a linguagem de programação.

- **Atributos de projeto:**
  - uso de práticas modernas de programação;
  - uso de ferramentas de software;
  - cronograma exigido de desenvolvimento.

Cada um desses atributos deve ser classificado de acordo com uma escala que varia de “muito baixo” a “extremamente elevado” (em importância e valor). A partir desta classificação determina-se o Multiplicador de Esforço (considerando a Tabela publicada por Boehm (1981)). O produto de todos os resultados de Multiplicadores de Esforços é chamado de Fator de Ajustamento de Esforço.

<table>
    <thead>
        <tr bgcolor="#6c6f73">
            <th>Direcionadores de Custo</th>
            <th>Muito Baixo</th>
            <th>Baixo</th>
            <th>Normal</th>
            <th>Elevado</th>
            <th>Muito Elevado</th>
            <th>Extremamente Elevado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td bgcolor="#9ea0a3" align="center" colspan=7>ATRIBUTOS DO PRODUTO</td>
        </tr>
        <tr>
            <td>Confiabilidade exigida do software</td>
            <td>0.75</td>
            <td>0.88</td>
            <td>1.00</td>
            <td>1.15</td>
            <td>1.40</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Tamanho do banco de dados</td>
            <td>-</td>
            <td>0.94</td>
            <td>1.00</td>
            <td>1.08</td>
            <td>1.16</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Complexidade do produto</td>
            <td>0.70</td>
            <td>0.85</td>
            <td>1.00</td>
            <td>1.15</td>
            <td>1.30</td>
            <td>1.65</td>
        </tr>
        <tr>
            <td bgcolor="#9ea0a3" align="center" colspan=7>ATRIBUTOS DO HARDWARE</td>
        </tr>
        <tr>
            <td>Restrições ao tempo de execução</td>
            <td>-</td>
            <td>-</td>
            <td>1.00</td>
            <td>1.11</td>
            <td>1.30</td>
            <td>1.66</td>
        </tr>
        <tr>
            <td>Restrições de memória</td>
            <td>-</td>
            <td>-</td>
            <td>1.00</td>
            <td>1.06</td>
            <td>1.21</td>
            <td>1.56</td>
        </tr>
        <tr>
            <td>Volatilidade do ambiente de máquina</td>
            <td>-</td>
            <td>0.87</td>
            <td>1.00</td>
            <td>1.15</td>
            <td>1.30</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Tempo de turnaround (tempo para completar o ciclo) exigido</td>
            <td>-</td>
            <td>0.87</td>
            <td>1.00</td>
            <td>1.07</td>
            <td>1.15</td>
            <td>-</td>
        </tr>
        <tr>
            <td bgcolor="#9ea0a3" align="center" colspan=7>ATRIBUTOS DE PESSOAL</td>
        </tr>
        <tr>
            <td>Capacidade do analista</td>
            <td>1.46</td>
            <td>1.19</td>
            <td>1.00</td>
            <td>0.86</td>
            <td>0.71</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Experiência em aplicações</td>
            <td>1.29</td>
            <td>1.13</td>
            <td>1.00</td>
            <td>0.91</td>
            <td>0.82</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Capacidade do programador</td>
            <td>1.42</td>
            <td>1.17</td>
            <td>1.00</td>
            <td>0.86</td>
            <td>0.70</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Experiência em Máquina Virtual</td>
            <td>1.21</td>
            <td>1.10</td>
            <td>1.00</td>
            <td>0.90</td>
            <td>-</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Experiência com a linguagem de programação</td>
            <td>1.14</td>
            <td>1.07</td>
            <td>1.00</td>
            <td>0.95</td>
            <td>-</td>
            <td>-</td>
        </tr>
        <tr>
            <td bgcolor="#9ea0a3" align="center" colspan=7>ATRIBUTO DE PROJETO</td>
        </tr>
        <tr>
            <td>Uso de práticas modernas de programação</td>
            <td>1.24</td>
            <td>1.10</td>
            <td>1.00</td>
            <td>0.91</td>
            <td>0.82</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Uso de ferramentas de software</td>
            <td>1.24</td>
            <td>1.10</td>
            <td>1.00</td>
            <td>0.91</td>
            <td>0.83</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Cronograma exigido de desenvolvimento</td>
            <td>1.23</td>
            <td>1.08</td>
            <td>1.00</td>
            <td>1.04</td>
            <td>1.10</td>
            <td>-</td>
        </tr>
    </tbody>
</table>

#### Calculo da Estimativa do Esforço

O resultado do esforço representa o valor de **Pessoas/Mês**
O modelo COCOMO Intermediário usa a seguinte equação para a estimativa do esforço:

    E = a x S^b x fae

onde:

- **E:** é o esforço aplicado (em pessoas-mês).
- **S:** é o número (estimado) de linhas de código para o projeto (em milhares).
- **a:** é um coeficiente fornecido pela Tabela.
- **b:** é um expoente fornecido pela Tabela.
- **fae:** é o Fator de Ajustamento do Esforço (multiplicação de cada um dos Multiplicadores de Esforço fornecidos pela Tabela).

Tabela para os valores dos coeficientes "a" e "b" de acordo com o tipo do projeto, a mesma tabela utilizada no COCOMO básico:

| Projeto de Software | a    |  b   |  c   |  d   |
| :-----------------: | :--- | :--: | :--: | :--: |
|      Orgânico       | 2.40 | 1.05 | 2.50 | 0.38 |
|    Semidestacado    | 3.00 | 1.12 | 2.50 | 0.35 |
|      Embutido       | 3.60 | 1.20 | 2.50 | 0.32 |

.

#### Calculo da Estimativa do Tempo

Representa a **quantidade de meses prevista para a conclusão do projeto**:

    T = c x E^d

onde:

- **E:** é o esforço aplicado (em pessoas-mês).
- **T:** é o tempo de desenvolvimento (em meses cronológicos).
- **S:** é o número estimado de linhas de código em milhares (KLOC)\* .
- **a:** é um coeficiente fornecido pela Tabela.
- **b:** é um expoente fornecido pela Tabela.
- **c:** é um coeficiente fornecido pela Tabela.
- **d:** é um expoente fornecido pela Tabela.

## Resultados

### Pesos de classificação de acordo com a tabela

<table>
    <thead>
        <tr bgcolor="#6c6f73">
            <th>Direcionadores de Custo</th>
            <th>Muito Baixo</th>
            <th>Baixo</th>
            <th>Normal</th>
            <th>Elevado</th>
            <th>Muito Elevado</th>
            <th>Extremamente Elevado</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td bgcolor="#9ea0a3" align="center" colspan=7>ATRIBUTOS DO PRODUTO</td>
        </tr>
        <tr>
            <td>Confiabilidade exigida do software</td>
            <td>0.75</td>
            <td>0.88</td>
            <td  class="selected" bgcolor="#ccc">1.00</td>
            <td>1.15</td>
            <td>1.40</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Tamanho do banco de dados</td>
            <td>-</td>
            <td>0.94</td>
            <td class="selected" bgcolor="#ccc">1.00</td>
            <td>1.08</td>
            <td>1.16</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Complexidade do produto</td>
            <td>0.70</td>
            <td>0.85</td>
            <td class="selected" bgcolor="#ccc">1.00</td>
            <td>1.15</td>
            <td>1.30</td>
            <td>1.65</td>
        </tr>
        <tr>
            <td bgcolor="#9ea0a3" align="center" colspan=7>ATRIBUTOS DO HARDWARE</td>
        </tr>
        <tr>
            <td>Restrições ao tempo de execução</td>
            <td>-</td>
            <td>-</td>
            <td class="selected" bgcolor="#ccc">1.00</td>
            <td>1.11</td>
            <td>1.30</td>
            <td>1.66</td>
        </tr>
        <tr>
            <td>Restrições de memória</td>
            <td>-</td>
            <td>-</td>
            <td class="selected" bgcolor="#ccc">1.00</td>
            <td>1.06</td>
            <td>1.21</td>
            <td>1.56</td>
        </tr>
        <tr>
            <td>Volatilidade do ambiente de máquina</td>
            <td>-</td>
            <td class="selected" bgcolor="#ccc">0.87</td>
            <td>1.00</td>
            <td>1.15</td>
            <td>1.30</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Tempo de turnaround (tempo para completar o ciclo) exigido</td>
            <td>-</td>
            <td>0.87</td>
            <td class="selected" bgcolor="#ccc">1.00</td>
            <td>1.07</td>
            <td>1.15</td>
            <td>-</td>
        </tr>
        <tr>
            <td bgcolor="#9ea0a3" align="center" colspan=7>ATRIBUTOS DE PESSOAL</td>
        </tr>
        <tr>
            <td>Capacidade do analista</td>
            <td>1.46</td>
            <td>1.19</td>
            <td class="selected" bgcolor="#ccc">1.00</td>
            <td>0.86</td>
            <td>0.71</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Experiência em aplicações</td>
            <td>1.29</td>
            <td>1.13</td>
            <td >1.00</td>
            <td class="selected" bgcolor="#ccc">0.91</td>
            <td>0.82</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Capacidade do programador</td>
            <td>1.42</td>
            <td>1.17</td>
            <td >1.00</td>
            <td class="selected" bgcolor="#ccc">0.86</td>
            <td>0.70</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Experiência em Máquina Virtual</td>
            <td class="selected" bgcolor="#ccc">1.21</td>
            <td>1.10</td>
            <td>1.00</td>
            <td>0.90</td>
            <td>-</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Experiência com a linguagem de programação</td>
            <td>1.14</td>
            <td>1.07</td>
            <td >1.00</td>
            <td  class="selected" bgcolor="#ccc">0.95</td>
            <td>-</td>
            <td>-</td>
        </tr>
        <tr>
            <td bgcolor="#9ea0a3" align="center" colspan=7>ATRIBUTO DE PROJETO</td>
        </tr>
        <tr>
            <td>Uso de práticas modernas de programação</td>
            <td>1.24</td>
            <td>1.10</td>
            <td >1.00</td>
            <td  class="selected" bgcolor="#ccc">0.91</td>
            <td>0.82</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Uso de ferramentas de software</td>
            <td>1.24</td>
            <td>1.10</td>
            <td>1.00</td>
            <td  class="selected" bgcolor="#ccc">0.91</td>
            <td>0.83</td>
            <td>-</td>
        </tr>
        <tr>
            <td>Cronograma exigido de desenvolvimento</td>
            <td>1.23</td>
            <td>1.08</td>
            <td>1.00</td>
            <td>1.04</td>
            <td  class="selected" bgcolor="#ccc">1.10</td>
            <td>-</td>
        </tr>
    </tbody>
</table>

Com isso, o resultado do peso que será utilizado equivale a multiplicação dos fatores selecioandos. Sendo assim, será usado um fae = 0.71

## Estimativa de Quantidade de Linhas de Códigos

Foi feito uma reunião com a equipe de desenvolvimento para estimar a quantidade de linhas de código que a aplicação pode tomar separado por telas e funcionalidades principais.

### Backend

Total: 950 linhas

- Crud de estoque

  - Listagem de produtos - 150 linhas
  - Cadastro de estoque - 200 linhas
  - Adição de produto no estoque - 100 linhas
  - Remoção de produto no estoque - 100 linhas
  - Atualizar estoque - 120 linhas

- Crud de usuários

  - Registro de usuário - 100 linhas
  - Atualização de dados cadastrais - 65 linhas
  - Remoção de usuário - 25 linhas
  - Autenticação do usuário - 65 linhas

- Middleware
  - Verificação de token - 20 linhas

### Frontend

Total: 1820 linhas

- Tela de login - 150 linhas
- Tela de cadastro -170 linhas
- Tela de perfil do usuário - 200 linhas
- Tela inical da aplicação (Dashboard) - 400 linhas
- Tela de lista de estoque - 300 linhas (socket e responsividade)
- Tela de cadastro de estoque - 150 linhas
- Tela de atualização dos produtos no estoque - 200 linhas
- Tela de admnistração (Listagem de usuário, alterar um usuário ,cadastrar um funcionario) - 250 linhas

Com isso, o total de linhas estimados para a aplicação foi de 2770 linhas de código. Como é possível uma falha na estimativa, os cálculos irão considerar um intervalo entre 2270 e 2770 linhas de código.

## Estimativa de Esforço

Como dito na introdução, nosso projeto é do tipo Semidestacado, portanto os valores serão **a = 3.00** e **b = 1.12**

Para 2770 linhas de código (2.77 Kloc)

E = a x S^b x fae

    E = 3.00 x 2.77^1.12 * (0,71)

    E = 6.7 pessoas/mes

Para 2270 linhas de código (2.27 Kloc)

    E = 3.00 x 2.27^1.12 * (0,71)

    E = 5.33 pessoas/mes

## Estimativa de Tempo

Utiliza o resultado calculado do esforço para calcular o tempo, pois estão diretamente relacionados, também utiliza o coeficiente **c = 2.50** e **d = 0.35** da tabela (Para projeto semidestacado):

Para 2770 linhas de código (2.77 Kloc)

    T = c x E^d

    T = 2.50 x 6.7^0.35

    T = 4.86 meses

Para 2270 linhas de código (2.27 Kloc)

    T = 2.50 x 8.91^0.35

    T = 4.49 meses

## Estimativa de preço

Os valores alcançados pelas estimativas foram bastantes rasoáveis de acordo com a realidade do projeto, que possui 5 desenvolvedores e um semestre de aproximadamente 6 meses para desenvolver a aplicação. Por isso, serão levados em conta para esse cálculo 5 quantidade de pessoas e 5 meses de desenvolvimento, o que está dentro da margem estipulada.

### Infra estrutura

Todos os valores usados para os cálculos foram pesquisados e podem ser conferidos na sessão de referências do documento.

|  Produto  |            Finalidade            |       Valor        |     Quantidade      | Total         | Fornecedor |
| :-------: | :------------------------------: | :----------------: | :-----------------: | ------------- | ---------- |
| Internet  | Desenvolvimento de gerenciamento |     R\$ 119,99     | 5 pessoas x 5 meses | R\$ 2.999,75  | Claro Net  |
| Notebook  | Desenvolvimento de gerenciamento |     R\$ 3.500      |          5          | R\$ 17.500,00 | Diversos   |
|    Luz    | Desenvolvimento de gerenciamento | R\$ 0,3020 R\$/Kwh |      3.000 Kwh      | R\$ 906,00    | CEB        |
| **Total** |        **R\$ 21.405,75**         |

### Desenvolvedores

Consideramos que os desenvolvedores irão trabalhar 4 horas por dia, 5 dias por semana.

| Quantidate | Preço da hora | Tempo de projeto |     Total     |
| :--------: | :-----------: | :--------------: | :-----------: |
|     5      |  R\$ 30,00/h  |     5 meses      | R\$ 60.000,00 |

## Conclusão

Com isso, estipula-se que o valor total do projeto seja estimado em **R\$ 81,405.75** reais.

## Referências

SILVA FILHO, Antonio Mendes da. **Custo de Software: Planejamento e Gestão**. Disponível em: <http://www.periodicos.uem.br/ojs/index.php/EspacoAcademico/article/view/22604/12254>. Último acesso 04/09/2020

**A monitoria**. Disponível em: <https://github.com/2019-2-arquitetura-desenho/wiki>. Último acesso 05/09/2020

**COCOMO** Disponível em: <http://vivenciandoti.blogspot.com/2016/07/o-que-e-cocomo-ii.html#:~:text=COCOMO%20(COnstructive%20COst%20MOdel)%20%C3%A9,equipe%20em%20projetos%20de%20software.&text=Este%20n%C3%BAmero%20pode%20ser%20derivado,fun%C3%A7%C3%A3o%20n%C3%A3o%20ajustados%20do%20projeto.>. Último acesso 05/09/2020

**Internet Claro** Disponível em: <https://www.claro.com.br/internet/banda-larga>. Último acesso 06/09/2020

**CEB ENERGIA** Disponível em: <http://www.aneel.gov.br/home?p_p_id=101&p_p_lifecycle=0&p_p_state=maximized&p_p_mode=view&_101_struts_action=%2Fasset_publisher%2Fview_content&_101_returnToFullPageURL=http%3A%2F%2Fwww.aneel.gov.br%2Fhome%3Fp_auth%3DjMK88uBU%26p_p_id%3D3%26p_p_lifecycle%3D1%26p_p_state%3Dnormal%26p_p_state_rcv%3D1&_101_assetEntryId=14837763&_101_type=content&_101_groupId=656877&_101_urlTitle=aneel-estabelece-novo-valor-para-encargo-de-capacidade-emergencial-da-cb-1&inheritRedirect=true>. Último acesso 06/09/2020

<style>
    .selected {
        color: #fff
    }
</style>
