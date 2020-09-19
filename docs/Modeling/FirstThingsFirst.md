# First Things First
O método First Things First é uma técnica de priorização de requisitos que analisa matematicamente o benefício, penalidade, custo e risco relativo de cada requisito para que seja calculada uma ordem de prioridade entre os requisitos. A técnica foi aplicada como um detalhamento do [MoSCoW](Modeling/MOSCOW.md), visto que esta classifica as histórias de usuário em 4 status diferentes.

Sendo assim, foi feita uma filtragem dos requisitos avaliados como "prioritários" na técnica de [MoSCoW](Modeling/MOSCOW.md), isto é, requisitos avaliados como **Must**, **Should** ou **Could** sendo desconsiderados os requisitos avalidados como **Would**. Além disso, a técnica exige que requisitos totalmente dependentes de outros não participem dos cálculos para evitar situações onde um requisito B é avaliado como prioritário, porém depende de um requisito A, que não tem prioridade tão alta, seja implementado em conjunto ou previamente. É possível consultar a tabela dos [Requisitos não avaliados](Modeling/FirstThingsFirst.md?id=Requisitos-Não-Avaliados).

Como a técnica foi aplicada após a criação do [Backlog](Modeling/Backlog.md), foi utilizada a história do usuário correspondente aos requisitos (requisitos funcional e os não funcionais atrelados) na avaliação para melhor entendimento no momento da discussão em grupo.

Foram utilizados os seguintes pesos:

|      Avaliação      | Peso |
|:-------------------:|:----:|
| Benefício Relativo  |   2  |
| Penalidade Relativa |   1  |
| Custo Relativo      |   1  |
| Risco Relativo      |  0.5 |

Cada item da avaliação foi avaliado em um número entre 1 e 5.

O valor é calculado pela fórmula:
```
Valor = Benefício * Peso do Benefício + Penalidade * Peso da Penalidade
```

A prioridade é calculada pela fórmula:
```
Prioridade = Valor% / (Custo% * Peso do Custo + Risco% * Peso do Risco)
```



## Histórico de Revisões

| Data | Versão | Descrição | Autor(es) |
|:----:|:------:|:---------:|:---------:|
| 18/09/2020 | 1.0 | Priorização First Thins First. | Gabriel Alves, Gabriel Davi, Micaella Gouveia, Pedro Igor, Sofia Patrocínio |
| 19/09/2020 | 1.1 | Adição da tabela, introdução e detalhamento da técnica e referências.              | Pedro Igor |
| 19/09/2020 | 1.2 | Adição da tabela de requisitos não avaliados.   | Pedro Igor |  

## Requisitos Não Avaliados
<div class="ritz grid-container" dir="ltr">
  <table class="waffle" cellspacing="0" cellpadding="0">
    <tbody>
      <tr style='height:20px;'>
        <td class="s0" dir="ltr">Desejo</td>
        <td class="s0" dir="ltr">Para que eu possa</td>
        <td class="s0" dir="ltr">Requisitos</td>
        <td class="s0" dir="ltr">MOSCOW</td>
        <td class="s0" dir="ltr">Motivo</td>
        <td class="s0" dir="ltr">Dependência</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Dar feedbacks ao suporte da aplicação</td>
        <td class="s1" dir="ltr">Relatar qualquer erro encontrado ou sugestões de novas funcionalidades</td>
        <td class="s1" dir="ltr">RF27</td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s2">Avaliado como Would no MOSCOW</td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Remover itens do controle de estoque</td>
        <td class="s1" dir="ltr">Controlar vendas e remoções do estoque</td>
        <td class="s1" dir="ltr">RF07</td>
        <td class="s1" dir="ltr">Must</td>
        <td class="s3" dir="ltr">Depende de &quot;Cadastrar itens no meu controle de estoque&quot;.</td>
        <td class="s4" dir="ltr">RF03</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Dar baixa em um produto pelo aplicativo mobile</td>
        <td class="s1">Vender ou remover produtos mais facilmente</td>
        <td class="s1">RF18, RNF03, RNF05</td>
        <td class="s1" dir="ltr">Should</td>
        <td class="s3" dir="ltr">Depende de &quot;Cadastrar itens no meu controle de estoque&quot; e &quot;Possuir uma
          versão mobile do aplicativo do estoque&quot;.</td>
        <td class="s4" dir="ltr">RF03, RF17,RNF03, RNF05</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Definir a quantidade mínima de determinado produto</td>
        <td class="s1">Ser notificado quando um item estiver em baixa no estoque</td>
        <td class="s1">RF19</td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;Cadastrar itens no meu controle de estoque&quot;.</td>
        <td class="s4" dir="ltr">RF03</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Ter uma lista de produtos solicitados por clientes que não estão disponíveis no estoque</td>
        <td class="s1">Adquirir esses produtos e disponibinizá-los no estoque</td>
        <td class="s1">RF22</td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no MOSCOW</td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Cadastrar um produto adicionando seu valor de fábrica</td>
        <td class="s1" dir="ltr">Visualizar uma margem de lucro satisfatória</td>
        <td class="s1" dir="ltr">RF32</td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no MOSCOW</td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Filtrar a minha busca por uma categoria no controle de estoque</td>
        <td class="s1">Acessar com facilidade os produtos relacionados a esta categoria</td>
        <td class="s1">RF05</td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;Consultar itens presentes no meu estoque&quot;.</td>
        <td class="s4" dir="ltr">RF04, RNF01, RNF03, RNF05</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Filtrar a busca de um produto por nome e/ou preço</td>
        <td class="s1">Acessar com facilidade as informações sobre este produto</td>
        <td class="s1">RF12</td>
        <td class="s1" dir="ltr">Should</td>
        <td class="s3" dir="ltr">Depende de &quot;Consultar itens presentes no meu estoque&quot;.</td>
        <td class="s4" dir="ltr">RF04, RNF01, RNF03, RNF05</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Gostaria de, no momento da listagem, poder filtrar os produtos pela data de adição</td>
        <td class="s1">Ter um melhor controle dos produtos que estão mais tempo parados no meu estoque</td>
        <td class="s1">RF13</td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;Consultar itens presentes no meu estoque&quot;.</td>
        <td class="s4" dir="ltr">RF04, RNF01, RNF03, RNF05</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Consultar produtos que mais saem do meu estoque</td>
        <td class="s1">Saber quais produtos devo comprar em maior quantidade</td>
        <td class="s1">RF26, RNF01</td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no MOSCOW</td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">No momento da listagem, poder filtrar os produtos pela data de vencimento</td>
        <td class="s1">Ter um melhor controle dos produtos que estão para vencer</td>
        <td class="s1">RF29</td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;Consultar itens presentes no meu estoque&quot;.</td>
        <td class="s4" dir="ltr">RF04, RNF01, RNF03, RNF05</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Ser alertado que um ou mais produtos estão com quantidades mínimas no estoque</td>
        <td class="s1">Reabastecer itens quando estiver em baixa no estoque</td>
        <td class="s1">RF20</td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Depende de &quot;Definir a quantidade mínima de determinado produto&quot;.</td>
        <td class="s4" dir="ltr">RF19</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Ser alertado caso um produto ultrapasse o seu prazo de validade</td>
        <td class="s1">Organizar meu estoque, retirando este produto vencido</td>
        <td class="s1">RF21</td>
        <td class="s1" dir="ltr">Should</td>
        <td class="s5" dir="ltr">Depende de &quot;Cadastrar itens no meu controle de estoque&quot;.</td>
        <td class="s4" dir="ltr">RF03</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Gerar gráficos que marcam o periodo por quantidade total de produto</td>
        <td class="s1" dir="ltr">Fazer uma análise melhor do crescimento geral do meu estoque</td>
        <td class="s1" dir="ltr">RF24, RNF02</td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Consultar um log de remoção e adição de itens ao estoque.</td>
        <td class="s4" dir="ltr">RF10, RNF01</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Gerar gráficos que marcam a quantidade de produtos por categoria</td>
        <td class="s1" dir="ltr">Saber a quantidade de produtos por categorias</td>
        <td class="s1" dir="ltr">RF24, RNF02</td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no MOSCOW</td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1" dir="ltr">Visualizar a margem de lucro dos meus produtos </td>
        <td class="s1" dir="ltr">Precificar da melhor forma os produtos</td>
        <td class="s1" dir="ltr">RF33</td>
        <td class="s1" dir="ltr">Would</td>
        <td class="s3">Avaliado como Would no MOSCOW</td>
        <td class="s1" dir="ltr">-</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s1">Filtrar para consulta um log de remoção e adição de itens ao estoque de forma temporal</td>
        <td class="s1">Consultar o fluxo de estoque em um período específico</td>
        <td class="s1">RF11, RNF01</td>
        <td class="s1" dir="ltr">Could</td>
        <td class="s3" dir="ltr">Consultar um log de remoção e adição de itens ao estoque.</td>
        <td class="s4" dir="ltr">RF10, RNF01</td>
      </tr>
    </tbody>
  </table>
</div>

## First Things First
<div class="ritz grid-container" dir="ltr">
  <table class="waffle" cellspacing="0" cellpadding="0">
    <tbody>
      <tr style='height:20px;'>
        <td class="s0" dir="ltr">Requisitos</td>
        <td class="s0" dir="ltr">Desejo</td>
        <td class="s1 softmerge" dir="ltr">
          <div class="softmerge-inner" style="width: 121px; left: -1px;">Benefício Relativo</div>
        </td>
        <td class="s1 softmerge" dir="ltr">
          <div class="softmerge-inner" style="width: 141px; left: -1px;">Penalidade Relativa</div>
        </td>
        <td class="s1" dir="ltr">Valor Total</td>
        <td class="s1" dir="ltr">Valor %</td>
        <td class="s1 softmerge" dir="ltr">
          <div class="softmerge-inner" style="width: 97px; left: -1px;">Custo Relativo</div>
        </td>
        <td class="s1" dir="ltr">Custo %</td>
        <td class="s1 softmerge" dir="ltr">
          <div class="softmerge-inner" style="width: 97px; left: -1px;">Risco Relativo</div>
        </td>
        <td class="s1" dir="ltr">Risco %</td>
        <td class="s1" dir="ltr">Prioridade</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr">RF28</td>
        <td class="s2" dir="ltr">Fazer o pedido de cadastro da minha empresa</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3">15</td>
        <td class="s3">7,575757576</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">1,923076923</td>
        <td class="s3">1,375661376</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF03</td>
        <td class="s2">Cadastrar itens no meu controle de estoque</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3">15</td>
        <td class="s3">7,575757576</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">3,846153846</td>
        <td class="s3">1,171171171</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF30</td>
        <td class="s2">Editar o nível de acesso de um colaborador</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">11</td>
        <td class="s3">5,555555556</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">2,272727273</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">1,077212806</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF04, RNF01, RNF03, RNF05</td>
        <td class="s2">Consultar itens presentes no meu estoque</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3">15</td>
        <td class="s3">7,575757576</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">1,019607843</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF25</td>
        <td class="s2">Cadastrar valor de cada produto</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">10</td>
        <td class="s3">5,050505051</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">2,272727273</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,9792843691</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr">RF06</td>
        <td class="s2" dir="ltr">No momento do cadastro de um item, adicionar tags aos produtos</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">8</td>
        <td class="s3">4,04040404</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">2,272727273</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">3,846153846</td>
        <td class="s3">0,962962963</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr">RF01</td>
        <td class="s2" dir="ltr">Realizar o login na aplicação</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3">15</td>
        <td class="s3">7,575757576</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">3,846153846</td>
        <td class="s3">0,8666666667</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF31</td>
        <td class="s2">Adicionar ou remover um colaborador da aplicação</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">14</td>
        <td class="s3">7,070707071</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,8425925926</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr">RF02</td>
        <td class="s2" dir="ltr">Criar contas para meus funcionários com diferentes níveis de acessos</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">10</td>
        <td class="s3">5,050505051</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,6797385621</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF15, RNF01</td>
        <td class="s2">Que a atualização dos dados seja feita assim que houver alguma modificação no controle do estoque
        </td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">14</td>
        <td class="s3">7,070707071</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">9,090909091</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,5465465465</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF23</td>
        <td class="s2">Cadastrar mesmo produto separados por diferentes lotes</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">11</td>
        <td class="s3">5,555555556</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,5209471767</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr">RF08, RNF02</td>
        <td class="s2" dir="ltr">Importar uma planilha em excel com dados do meu estoque na aplicação</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">10</td>
        <td class="s3">5,050505051</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,5205205205</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF17, ,RNF03, RNF05</td>
        <td class="s2">Possuir uma versão mobile do aplicativo do estoque</td>
        <td class="s3" dir="ltr">5</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">12</td>
        <td class="s3">6,060606061</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">9,090909091</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,4684684685</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF09, RNF02</td>
        <td class="s2">Gerar planilhas de análise do estoque</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">1</td>
        <td class="s3">9</td>
        <td class="s3">4,545454545</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,4684684685</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr">RF14, RNF02</td>
        <td class="s2" dir="ltr">Visualizar gráficos baseados no fluxo de estoque</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">11</td>
        <td class="s3">5,555555556</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">9,090909091</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,4294294294</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2">RF10, RNF01</td>
        <td class="s2">Consultar um log de remoção e adição de itens ao estoque</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">10</td>
        <td class="s3">5,050505051</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">9,090909091</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">5,769230769</td>
        <td class="s3">0,4217356042</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s2" dir="ltr">RF24, RNF02</td>
        <td class="s2" dir="ltr">Gerar gráficos que marcam a quantidade de produtos por funcionários</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3" dir="ltr">2</td>
        <td class="s3">8</td>
        <td class="s3">4,04040404</td>
        <td class="s3" dir="ltr">3</td>
        <td class="s3">6,818181818</td>
        <td class="s3" dir="ltr">4</td>
        <td class="s3">7,692307692</td>
        <td class="s3">0,378870674</td>
      </tr>
      <tr style='height:20px;'>
        <td class="s4"></td>
        <td class="s4"></td>
        <td class="s5">73</td>
        <td class="s5">52</td>
        <td class="s5">198</td>
        <td class="s5">100</td>
        <td class="s5">44</td>
        <td class="s5">100</td>
        <td class="s5">52</td>
        <td class="s5">100</td>
        <td class="s4"></td>
      </tr>
    </tbody>
  </table>
</div>

## Referências
 - First Things First: <https://www.processimpact.com/articles/prioritizing.pdf>. Último acesso em 19/09/2020